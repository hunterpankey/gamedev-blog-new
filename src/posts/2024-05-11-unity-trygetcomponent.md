---
layout: post
title: "Unity's TryGetComponent Method"
excerpt: "A better way to get components on your game objects in Unity"
author: hunter-pankey
date: 2024-05-11T00:35:00-04:00
draft: false
tags: 
  - unity
  - dev
  - gamedev
  - scripting
seo:
  title:
  description:
  image: 2024/05/trygetcomponent/header.png
images: # relative to /src/assets/images/
  feature:
  thumb: 2024/05/trygetcomponent/header.png
  align: # object-center (default) - other options at https://tailwindcss.com/docs/object-position
  height: # optional. Default = h-48 md:h-1/3
---
Starting in Unity 2019.2, GameObjects now have a [TryGetComponent()][trygetcomponent] method that attempts to get a component on the game object and return it (via an out parameter), as well as returning a boolean for whether the operation was successful. One should basically never use the old [GameObject.GetComponent()][getcomponent] method now that TryGetComponent() is available. (I'm sure a good use case could be coerced from some scenario, but for most cases, this new one'll do much better.)

Basically, instead of doing:


```csharp
Rigidbody rb = this.GetComponent<Rigidbody>();

if(rb != null)
{
  // do whatever ole thing with the Rigidbody
}
```

This can be kinda cleaned up into the following:


```csharp
if(this.TryGetComponent<Rigidbody>(out Rigidbody rb))
{
  // do whatever you were gonna do with the Rigidbody using the rb variable
}
```

They both accomplish basically the same thing, but the second is a little more concise.

Note: There's a similar pattern when raycasting with [Physics.Raycast()][physics-raycast] and similar methods:

```csharp
if(Physics.Raycast(position, direction, out RaycastHit hit, distance, layerMask))
{
  // hit was successful, use hit variable here
}
```

[trygetcomponent]: https://docs.unity3d.com/ScriptReference/Component.TryGetComponent.html
[getcomponent]: https://docs.unity3d.com/ScriptReference/Component.GetComponent.html
[physics-raycast]: https://docs.unity3d.com/2019.2/Documentation/ScriptReference/Physics.Raycast.html