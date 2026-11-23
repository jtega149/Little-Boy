# Little Boy

Little Boy is an inference engine built entirely from scratch. This repository serves as a detailed explanation of the architecture behind the engine, to help others learn more about how LLM's are handled at the hardware level.


## Generate build instructions & build

```bash
cmake -S . -B build -G Ninja -DCMAKE_BUILD_TYPE=Release && cmake --build build
```