[README.md](https://github.com/user-attachments/files/31801395/README.md)
# Edge AI Experiments

A collection of hands-on experiments exploring Edge AI, on-device machine learning, embedded systems, and resource-constrained computing.

As an Electronics and Communication Engineering student, I enjoy experimenting with how AI can run beyond powerful desktops and cloud servers. This repository documents my practical attempts, observations, and lessons learned while deploying AI models on consumer hardware.

---

# About this Repository

This repository serves as a collection of personal experiments focused on Edge AI and embedded computing.

## Current Experiment

# Experiment 01: Running Local LLMs on Android using Termux + Ollama

## Objective

To investigate the feasibility of running open-source Large Language Models (LLMs) locally on an Android smartphone without relying on cloud-based APIs, while evaluating the practical hardware limitations of a mid-range mobile device.

## Device Specifications

| Component | Specification |
|-----------|---------------|
| Device | Redmi Note 9 Pro Max |
| SoC | Qualcomm Snapdragon 720G (8 nm) |
| CPU | Octa-core (2× Kryo 465 Gold @ 2.3 GHz + 6× Kryo 465 Silver @ 1.8 GHz) |
| GPU | Adreno 618 |
| RAM | 6 GB LPDDR4X |
| Environment | Android + Termux |

## Software Used

- Termux
- Ollama
- Linux command-line utilities

## Models Tested

| Model | Status | Notes |
|-------|:------:|------|
| TinyLlama | ✅ Successfully Ran | Fastest and most responsive |
| Gemma 1B | ✅ Successfully Ran | Better response quality |
| Qwen 3.5 2B | ✅ Successfully Ran | Highest quality tested |
| 3B Models | ⚪ Not Tested | Compatibility unknown |
| 3.5B Models | ⚪ Not Tested | Compatibility unknown |
| 4B Models | ❌ Failed | Hardware limitations |

## Methodology

1. Installed Termux.
2. Configured the Linux environment.
3. Installed Ollama.
4. Downloaded and executed lightweight LLMs.
5. Compared startup time, responsiveness and usability.
6. Explored the maximum practical model size supported by the device.

## Observations

### TinyLlama
- Fast startup
- Lowest memory usage
- Smooth user experience

### Gemma 1B
- Better responses than TinyLlama
- Slightly slower inference

### Qwen 3.5 2B
- Best response quality among tested models
- Highest resource usage
- Largest model successfully tested

### Model Size Limitations

- Successfully ran models up to the 2B class.
- 4B parameter models failed to run due to memory and hardware limitations.
- 3B and 3.5B models have not yet been tested.

## Challenges

- Limited 6 GB RAM
- CPU-only inference
- Thermal throttling during extended use
- Storage usage increased with multiple downloaded models

## Key Learnings

- Edge AI deployment
- Offline LLM inference
- Linux workflows using Termux
- Ollama model management
- Hardware resource constraints
- Trade-offs between model size and performance

## Future Work

- Benchmark token generation speed
- Test 3B and 3.5B models
- Compare quantized models
- Measure RAM, CPU and battery usage
- Evaluate newer Snapdragon devices

## Conclusion

This experiment demonstrated that a mid-range Android smartphone can successfully run lightweight open-source LLMs entirely offline using Termux and Ollama. Although larger models exceeded the hardware limits, the project provided valuable practical experience in Edge AI, mobile computing and resource-constrained machine learning.
