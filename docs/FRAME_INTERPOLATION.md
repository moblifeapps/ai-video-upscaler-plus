# AI Frame Interpolation

AI Video Upscaler+ uses **RIFE** to generate intermediate frames.

For example:

```text
30 FPS
A -------- B -------- C

60 FPS
A ---- A' ---- B ---- B' ---- C
```

`A'` and `B'` are generated intermediate frames.

Supported targets include **45 FPS and 60 FPS**. A common workflow is **30 FPS -> 60 FPS**.

Frame interpolation is useful for both old footage and modern video recorded at 24, 25 or 30 FPS.

It can be combined with resolution upscaling, for example:

```text
1080p / 30 FPS
      |
      +-- AI resolution enhancement
      +-- AI frame interpolation
      |
      v
4K / 60 FPS
```

Complex motion, occlusions, reflections, transparency and scene cuts can be challenging for interpolation models.
