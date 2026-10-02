# AI Video Upscaler+ for Windows

<p align="center">
<img src="https://mlapplications.com/uploads/aivideoupscaler_icon.png" width="128" alt="AI Video Upscaler+ icon">
</p>

<h2 align="center">Free AI Video Upscaling & Frame Interpolation for Windows</h2>

<p align="center">
<a href="https://mlapplications.com/ai_videoupscaler_plus.html">Official Website</a> ·
<a href="https://apps.microsoft.com/detail/9P54F81N7R30">Microsoft Store</a>
</p>

**AI Video Upscaler+** is a free Windows application for AI-powered video enhancement. It can increase video resolution up to **8K**, increase frame rate to **45 or 60 FPS**, and combine resolution upscaling and frame interpolation in the same workflow.

The application runs AI models locally using **ONNX Runtime and Microsoft DirectML/D3D12 acceleration**, supporting compatible **Intel, AMD and NVIDIA** graphics hardware.

**No subscription. No watermark. No cloud video processing.**

## Features

- AI video upscaling to 2K, 4K and 8K
- AI frame interpolation to 45 or 60 FPS
- 30 FPS → 60 FPS workflows
- Resolution upscaling + frame interpolation together
- Real-ESRGAN for super-resolution
- RIFE for frame interpolation
- Optional GFPGAN face restoration
- DirectML/D3D12 GPU acceleration
- Compatible Intel, AMD and NVIDIA graphics hardware
- Local processing
- Background processing and Windows notifications
- Batch processing
- Projects library
- No subscription
- No watermark

## AI models

| Model | Purpose |
|---|---|
| **Real-ESRGAN** | AI super-resolution |
| **RIFE** | AI frame interpolation |
| **GFPGAN** | Optional face restoration |

## Processing workflow

```text
Input video
    |
    v
Video decoding / preprocessing
    |
    +---------------------+
    |                     |
    v                     v
Real-ESRGAN              RIFE
Resolution AI       Frame-rate AI
    |                     |
    +----------+----------+
               |
               v
        Optional GFPGAN
        face restoration
               |
               v
        Post-processing
               |
               v
         Video encoding
               |
               v
         Enhanced video
```

## Example

```text
SOURCE
640 x 480 / 30 FPS
       |
       | AI upscaling + AI frame interpolation
       v
OUTPUT
3840 x 2160 / 60 FPS
```

AI processing cannot recover information that was never captured. Results depend on source quality, compression, motion, focus and model/settings.

## GPU architecture

```text
AI Video Upscaler+
        |
        v
   ONNX Runtime
        |
        v
DirectML execution provider
        |
        v
Compatible D3D12 GPU
   /      |      \
 Intel   AMD    NVIDIA
```

The application is designed for compatible DirectML/D3D12 hardware. Performance varies substantially between GPUs, drivers, video resolutions, frame rates and AI models.

## Screenshots

![Main workflow](https://mlapplications.com/aivideoupscaler_screenshots/FirstScreenshot.webp)

![Workflow](https://mlapplications.com/aivideoupscaler_screenshots/Screenshot_workflow.webp)

![Target resolution and FPS](https://mlapplications.com/aivideoupscaler_screenshots/Screenshot_Targets.webp)

![GFPGAN](https://mlapplications.com/aivideoupscaler_screenshots/Screenshot_GFPGAN.webp)

![Batch processing](https://mlapplications.com/aivideoupscaler_screenshots/Screenshot_Batch.webp)

![Notification](https://mlapplications.com/aivideoupscaler_screenshots/Screenshot_popup.webp)

## Official resources

- Website: https://mlapplications.com/
- Application page: https://mlapplications.com/ai_videoupscaler_plus.html
- Microsoft Store: https://apps.microsoft.com/detail/9P54F81N7R30
- Icon: https://mlapplications.com/uploads/aivideoupscaler_icon.png

## Documentation

- [Architecture](docs/ARCHITECTURE.md)
- [AI Upscaling](docs/UPSCALING.md)
- [Frame Interpolation](docs/FRAME_INTERPOLATION.md)
- [DirectML and GPU Support](docs/DIRECTML.md)
- [Performance Testing](docs/PERFORMANCE.md)
- [Privacy and Local Processing](docs/PRIVACY.md)
- [FAQ](docs/FAQ.md)
- [Discovery Topics](docs/KEYWORDS_AND_DISCOVERY.md)
- [Launch Checklist](docs/LAUNCH_CHECKLIST.md)

## Repository scope

This repository contains public technical documentation and high-level workflow information.

**AI Video Upscaler+ is proprietary software.** Its source code, proprietary implementation, packaged application, private development assets and unpublished model modifications are not included here.

## About

AI Video Upscaler+ is developed by **mlapplications.com** for Windows.
