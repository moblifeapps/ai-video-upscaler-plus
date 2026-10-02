# AI Video Upscaling

AI Video Upscaler+ uses **Real-ESRGAN** for AI super-resolution.

Typical workflows include:

- 480p -> 1080p
- 720p -> 1080p
- 720p -> 4K
- 1080p -> 4K
- supported targets up to 8K

4K UHD is **3840 x 2160**.

AI super-resolution is different from ordinary resizing: the model estimates plausible visual detail instead of simply stretching existing pixels.

AI cannot literally recover information that was never recorded. Very low-resolution, blurred or heavily compressed footage can still contain artifacts after enhancement.
