# Parallelization and Scaling


---
# Parallelization Strategies

---
## Data Parallelism

---
## Pipeline Parallelism

---
## Model Sharding

---
## Tensor Parallelism

---
## Sequence Parallelism

---
## Context Parallelism

---
## Expert Parallelism

---
# Frameworks

---
## Native Pytorch

---
## Megatron-LM

---
## NeMo

- NVidia supported
- Requires 

---
## Modalities

---
## Another One (TODO)

---
## HuggingFace Accelerate, PyTorch Lightning, 

---
## Also Existing

- DeepSpeed (original model sharding from MicroSoft)
- GPTNeoX :shrug:
- OSLO

---
# Measuring Performance

Metrics:
- Hardware FLOP/s
    - Depends on e.g. checkpointing or activation recomputation
    - Good for comparing to theoretical/reference performance of the hardware.
- Tokens / GPU / second
    - Can not compare models of different sizes.
    - Good for comparing a single model on different number of GPUs.
- Model FLOP/s Utilization
    - Good for comparing frameworks and clusters.
