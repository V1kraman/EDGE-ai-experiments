# EDGE-ai-experiments
Running open-source Large Language Models locally on an Android smartphone using Termux to explore on-device AI inference, hardware limitations, and performance.
### Observations

#### TinyLlama

- Fastest startup time and inference among all tested models.
- Consumed the least amount of memory.
- Ideal for lightweight conversations and experimentation.

#### Gemma 1B

- Produced noticeably better responses than TinyLlama.
- Slightly slower inference while remaining comfortably usable on the device.

#### Qwen 3.5 2B

- Delivered the best response quality of the tested models.
- Required significantly more system resources.
- Represented the upper limit of practical inference on my hardware while maintaining usability.

#### Model Size Limitations

During testing, I attempted to explore larger language models to understand the hardware limits of my device.

- Models up to approximately **2.5 billion parameters** were runnable.
- I was **unable to successfully run 4B parameter models** due to hardware resource limitations, primarily available RAM.
- Models in the **3B to 3.5B** range were **not tested**, so their feasibility on this device remains unknown.

This experiment highlighted how rapidly memory and computational requirements increase as model size grows, making hardware constraints a significant factor for on-device AI.
