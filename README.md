# Hybrid Autoregressive-Diffusion Model for Real-Time Streaming Sign Language Production

This repository contains the code for the HybridSign model.



## About

Earlier Sign Language Production (SLP) models typically relied on autoregressive methods that generate output tokens one by one, which inherently provide temporal alignment. Although techniques like Teacher Forcing can prevent model collapse during training, they still cannot solve the problem of error accumulation during inference, since ground truth is unavailable at that stage. In contrast, more recent approaches based on diffusion models leverage step-by-step denoising to enable high-quality generation. However, the iterative nature of these models and the requirement to denoise entire sequences limit their applicability in real-time tasks like SLP. To address it, we apply a hybrid approach combining autoregressive and diffusion models to SLP for the first time, leveraging the strengths of both models in sequential dependency modeling and output refinement. To capture fine-grained body movements, we design a Multi-Scale Pose Representation module that separately extracts detailed features from distinct body parts and integrates them via a Multi-Scale Fusion module. Furthermore, we introduce a Confidence-Aware Causal Attention mechanism that utilizes joint-level confidence scores to dynamically guide the pose generation process, improving accuracy and robustness. Extensive experiments on the PHOENIX14T and How2Sign datasets demonstrate the effectiveness of our method in both generation quality and real-time streaming efficiency.



## TODO
- [ ] Release Paper
- [ ] Release Code
