# Awesome Edge MLOps [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of tools for shipping, updating and monitoring machine learning models on phones, embedded boards and other edge devices.

Server-side MLOps is well covered elsewhere. This list is about what happens after a model leaves the server: getting it onto devices, running it there, updating it safely, and knowing how it behaves in the field.

## Contents

- [Model delivery and rollout](#model-delivery-and-rollout)
- [Device software updates](#device-software-updates)
- [On-device runtimes](#on-device-runtimes)
- [Conversion and optimization](#conversion-and-optimization)
- [Monitoring and drift](#monitoring-and-drift)
- [Benchmarks](#benchmarks)
- [Retired services](#retired-services)
- [Related lists](#related-lists)

## Model delivery and rollout

*Getting model versions onto devices, choosing which devices get which version, and taking a bad one back.*

- [AWS IoT Greengrass V2](https://docs.aws.amazon.com/greengrass/v2/developerguide/what-is-iot-greengrass.html) - AWS edge runtime and deployment service for IoT devices, with staged rollouts and rollback of failed deployments.
- [Azure IoT Edge](https://github.com/Azure/iotedge) - Runs containerized workloads on edge devices, managed from Azure IoT Hub.
- [Edge Impulse](https://www.edgeimpulse.com/) - Platform for building, optimizing and deploying ML models to edge devices.
- [FleetML](https://github.com/fleetml/fleetml) - Self-hosted rollouts for on-device models: canary and rolling deployments with automatic rollback, A/B tests and drift detection, for Android, iOS and Linux.
- [KubeEdge](https://github.com/kubeedge/kubeedge) - Kubernetes-native edge computing framework (CNCF).
- [Open Horizon](https://github.com/open-horizon/anax) - LF Edge project for autonomous deployment of containerized workloads to edge nodes.
- [Play for On-device AI](https://developer.android.com/google/play/on-device-ai) - Delivers models to Android apps through Google Play as AI packs, with optional device targeting (beta).

## Device software updates

*Over-the-air updaters for the device itself. Often used alongside a model delivery tool.*

- [balena](https://www.balena.io/) - Container-based fleet management and OTA updates for Linux devices.
- [Eclipse hawkBit](https://github.com/eclipse-hawkbit/hawkbit) - Back-end framework for rolling out software updates to constrained edge devices.
- [Mender](https://github.com/mendersoftware/mender) - Over-the-air software updater for embedded Linux, with an open-source server.
- [RAUC](https://github.com/rauc/rauc) - Safe and secure A/B software updates for embedded Linux.
- [SWUpdate](https://github.com/sbabic/swupdate) - Software update framework for embedded systems.

## On-device runtimes

*Libraries that run the model on the device.*

- [Core ML](https://developer.apple.com/documentation/coreml) - Apple's on-device inference framework for iOS, macOS and other Apple platforms.
- [ExecuTorch](https://github.com/pytorch/executorch) - PyTorch's runtime for mobile, embedded and edge devices.
- [llama.cpp](https://github.com/ggml-org/llama.cpp) - LLM inference in C/C++, widely used on laptops, phones and boards.
- [LiteRT](https://github.com/google-ai-edge/LiteRT) - Google's on-device framework, the successor to TensorFlow Lite.
- [MediaPipe](https://github.com/google-ai-edge/mediapipe) - Cross-platform ML solutions for live and streaming media.
- [MLC LLM](https://github.com/mlc-ai/mlc-llm) - LLM deployment engine built on ML compilation, targeting phones, browsers and GPUs.
- [MNN](https://github.com/alibaba/MNN) - Lightweight inference engine from Alibaba.
- [ncnn](https://github.com/Tencent/ncnn) - High-performance inference framework optimized for mobile platforms.
- [ONNX Runtime](https://onnxruntime.ai/) - Cross-platform inference for ONNX models, including mobile and edge builds.
- [OpenVINO](https://github.com/openvinotoolkit/openvino) - Toolkit for optimizing and running models on Intel hardware.
- [TensorFlow Lite Micro](https://github.com/tensorflow/tflite-micro) - Runs models on microcontrollers and other low-power devices.
- [TensorRT](https://github.com/NVIDIA/TensorRT) - NVIDIA's SDK for high-performance inference, including Jetson devices.

## Conversion and optimization

*Making a model small and fast enough for the device, and in the right format.*

- [Apache TVM](https://github.com/apache/tvm) - Open machine learning compiler framework.
- [coremltools](https://github.com/apple/coremltools) - Converts and optimizes models for Core ML.
- [LiteRT Torch](https://github.com/google-ai-edge/litert-torch) - Converts PyTorch models to LiteRT.
- [NNCF](https://github.com/openvinotoolkit/nncf) - Neural network compression (quantization, pruning) for OpenVINO.
- [NVIDIA Model Optimizer](https://github.com/NVIDIA/Model-Optimizer) - Quantization, pruning and distillation for NVIDIA inference stacks.
- [Olive](https://microsoft.github.io/Olive/) - Microsoft's model optimization toolchain for ONNX Runtime.
- [ONNX](https://github.com/onnx/onnx) - Open standard model format for moving models between frameworks and runtimes.
- [Optimum](https://github.com/huggingface/optimum) - Hugging Face tools for exporting and optimizing models for specific runtimes and hardware.
- [Qualcomm AI Hub Models](https://github.com/qualcomm/ai-hub-models) - Models optimized for Qualcomm devices, with export and profiling scripts.

## Monitoring and drift

*Knowing how a model behaves after it ships. Most of these run server-side on telemetry sent from devices.*

- [Alibi Detect](https://github.com/SeldonIO/alibi-detect) - Algorithms for outlier, adversarial and drift detection.
- [Evidently](https://github.com/evidentlyai/evidently) - Open-source ML and LLM observability framework with data drift reports.

## Benchmarks

- [MLPerf Mobile](https://github.com/mlcommons/mobile_app_open) - MLCommons' benchmark app for on-device inference performance.

## Retired services

*Useful context if you are migrating.*

- [Firebase ML custom model hosting](https://firebase.google.com/docs/ml/manage-hosted-models) - Deprecated; shuts down on June 15, 2027.
- [SageMaker Edge Manager](https://docs.aws.amazon.com/sagemaker/latest/dg/edge-eol.html) - Reached end of life on April 26, 2024.

## Related lists

- [awesome-mlops](https://github.com/kelvins/awesome-mlops) - MLOps tools in general.
- [awesome-tinyml](https://github.com/AI-in-Transportation-Lab/awesome-tinyml) - Machine learning on microcontrollers.

## Contributing

Suggestions are welcome. Read the [contributing guidelines](CONTRIBUTING.md) first.
