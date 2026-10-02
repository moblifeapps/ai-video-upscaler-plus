# Architecture

This document describes the public, high-level architecture without exposing proprietary implementation details.

## Inference path

```text
AI model
   |
   v
ONNX Runtime
   |
   v
DirectML execution provider
   |
   v
Direct3D 12
   |
   v
Compatible GPU
```

## Video workflow

```text
Input -> Decode -> Preprocess
                 |
        +--------+--------+
        |                 |
        v                 v
   Real-ESRGAN          RIFE
   Super-resolution   Interpolation
        |                 |
        +--------+--------+
                 |
          Optional GFPGAN
                 |
          Post-process
                 |
              Encode
                 |
              Output
```

Resolution enhancement and frame interpolation can be combined. The exact internal order is an implementation detail and may change between releases.

The public documentation intentionally does not expose proprietary source code, private optimization code, credentials, signing material or unpublished model modifications.
