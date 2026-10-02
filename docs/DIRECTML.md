# ONNX Runtime + Microsoft DirectML

AI Video Upscaler+ uses **ONNX Runtime** for neural-network inference and Microsoft's **DirectML/D3D12** acceleration path for compatible Windows GPU hardware.

```text
Application
    |
    v
ONNX Runtime
    |
    v
DirectML
    |
    v
Direct3D 12
    |
    v
GPU
```

The application is designed for compatible graphics hardware from:

- Intel
- AMD
- NVIDIA

DirectML support does not mean identical performance across GPUs. Compatibility and speed depend on GPU architecture, driver, Windows version, model, memory and workload.

The application should be described as supporting **compatible DirectML/D3D12 hardware**, rather than guaranteeing every GPU model.
