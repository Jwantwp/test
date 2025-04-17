This module provides support for zero-shot inference and supervised fine-tuning tasks for the **LLaVA series** of MLLMs. It includes four models: **LLaVA-OV-7B**, **LLaVA-OV-72B**, **LLaVA-Video-7B**, and **LLaVA-Video-72B**.

1. The `data` directory contains 12 types of multimodal datasets suitable for zero-shot inference and supervised fine-tuning tasks on the LLaVA series models. These datasets are divided into two categories: **LLaVA-OV** and **LLaVA-Video**.

2. The `examples` directory contains two subdirectories: **supervised fine-tuning ** and **zero-shot inference**. These subdirectories allow you to perform zero-shot inference and supervised fine-tuning on the LLaVA series of MLLMs.

   - Example executions for zero-shot inference with LLaVA models:

     ```bash
     # Perform zero-shot inference for LLaVA-OV-7B
     bash examples/zero_shot/run_zero_llavaov_7b.sh
     
     # Perform zero-shot inference for LLaVA-OV-72B
     bash examples/zero_shot/run_zero_llavaov_72b.sh
     
     # Perform zero-shot inference for LLaVA-Video-7B
     bash examples/zero_shot/run_zero_llavavideo_7b.sh
     
     # Perform zero-shot inference for LLaVA-Video-72B
     bash examples/zero_shot/run_zero_llavavideo_72b.sh
     ```

   - Example executions for supervised fine-tuning of the LLaVA series models:

     ```bash
     # Perform supervised fine-tuning for LLaVA-OV-7B
     bash examples/sft/run_total_llavaov_7b.sh
     
     # Perform supervised fine-tuning for LLaVA-OV-72B
     bash examples/sft/run_total_llavaov_72b.sh
     
     # Perform supervised fine-tuning for LLaVA-Video-7B
     bash examples/sft/run_total_llavavideo_7b.sh
     
     # Perform supervised fine-tuning for LLaVA-Video-72B
     bash examples/sft/run_total_llavavideo_7b.sh
     ```
