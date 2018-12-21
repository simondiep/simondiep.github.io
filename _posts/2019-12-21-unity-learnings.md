---
layout: post
title: "Unity Game Dev Learnings"
date: 2018-12-21 11:50:00 -0500
categories:
  - thoughts
  - tech
---

I've started building my own Unity games recently. Things have been pretty smooth until my latest project, [unity-idle-fighter](https://github.com/simondiep/unity-idle-fighter).

I've struggled with a few different concepts and have learned quite a bit. Here are some of my takeaways:

- Coding

  - The concept of a Scriptable Object makes a lot of sense. Being able to reuse a template for static data is perfect for this game.

- Editor

  - Figuring out animations was time-consuming, mainly due to the lack of support for prefab animations
    - Import spritesheet as asset
    - Set to multiple images and slice up with Unity Editor
    - Create an empty GameObject and click on it
    - Open the Animation Tab
    - Click Create new animmation in that tab - this will create two prefabs (AnimationClip and AnimatorController)
    - Drag your spritesheet into the Tab
    - Open the Animator Tab
    - Drag and drop your AnimationClip into the default state

- Building into a deliverable

  - 50% time spent building game, 50% time troubleshooting issues when creating a WebGL build
  - Avoid using any Classes that rely on the UnityEditor namespace, as these classes will only work in the editor
    - Specifically AnimatorController, use AnimatorOverrideController instead
  - How things show up on screen differ from the Unity Editor preview and the actual WebGL build, mainly due to camera and canvas settings
    - The overlay (Canvas) vs the images (in Camera view) are in completely different areas on the Editor and don't look like they would fit together, but they do
    - I still haven't fully understood this, and resorted to getting it working for a fixed resolution of 1280x800
  - Most of my time spent learning was how to interact with the Unity Editor and not actual coding

- General
  - The [official website](https://unity3d.com/learn/tutorials) has good examples
  - [Brackeys](https://www.youtube.com/user/Brackeys/videos) does a great job at explaining how to do specific things with Unity
  - It was difficult to search for answers to specific Unity problems via Google
  - StackOverflow and Unity forums have a lot of open Unity questions without answers

In summary, when you embark on a non-beginner Unity game, prepare to run into a lot of Editor-specific obstacles that are not code-related.
