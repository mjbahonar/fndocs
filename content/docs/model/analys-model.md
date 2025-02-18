---
title: Analyze 
weight: 10
---

## What do we have
Now that we have finished tuning, let's see what we have. Every 1000 steps, a **checkpoint** is created. The last checkpoint represents the fully tuned model. For example, the folder `checkpoint-15000` contains the final model. The folder structure looks like this:


```
project fine-tunning
│
└─── checkpoint-15000
│   │   model.safetensors
│   │   optimizer.bin
│   │   pytorch_lora_weights.safetensors
│   │   random_states_0.pkl
│   │   scheduler.bin
│   └───subfolder1
└
```

The key files in this directory are those with the `.safetensors` extension:  

- `model.safetensors`  
- `pytorch_lora_weights.safetensors` 



|  | model.safetensors|torch_lora_weights.safetensors |
|--|--|--|
| **size** |as size the base model  |	small|
| **description**|the original model with tunned model combined in|	only the tunned model|


