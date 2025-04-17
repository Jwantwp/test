This module is designed for the **VideoLLaMA2-7B** multimodal model, primarily focusing on **zero-shot inference** and **supervised fine-tuning** tasks for the VideoLLaMA2-7B model.

1. The dataset used for supervised fine-tuning of the VideoLLaMA2-7B model is consistent with the dataset utilized within the **LLaMA-Factory** framework.

2. The `examples` directory contains scripts for performing both zero-shot inference and supervised fine-tuning on the VideoLLaMA2-7B model.

   Below are examples for executing zero-shot inference and supervised fine-tuning for the VideoLLaMA2-7B model:

   ```bash
   # Execute zero-shot inference
   bash examples/bash/infer_zero_shot.sh
   
   # Perform supervised fine-tuning
   bash examples/bash/run_sft.sh
   ```


