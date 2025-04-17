This module leverages the **LLaMA-Factory** framework, which encompasses **zero-shot inference**, **supervised fine-tuning**, and **instruction fine-tuning** for LLMs, alongside **zero-shot inference**, **supervised fine-tuning**, and **instruction fine-tuning** for two MLLMs . The models include: 

- LLMs: **Qwen2-0.5B**，**Qwen2-1.5B**，**Qwen2-7B**, **Llama3-8B**, **Llama3.1-8B**，**Llama3.2-1B**，**Llama3-3B**，**Internlm2.5-8B**
- MLLMs: **Qwen2-VL-7B**, **Qwen2-VL-72B**

1. The `data` directory includes datasets formatted for zero-shot inference, supervised fine-tuning, and instruction fine-tuning for both LLMs and MLLMs.

   - For LLMs, the datasets required for zero-shot inference are located in the `data/dataset` directory, while datasets for supervised fine-tuning and instruction fine-tuning are located in the `data/llm_dataset` directory.

   - For MLLMs, datasets for both supervised fine-tuning and instruction fine-tuning can be found in the `data` directory. Detailed dataset information is available in the `data_info.json` file.

2. The `examples` directory contains scripts for running inference tasks on both LLMs and MLLMs.

   **Zero-Shot inference Scripts**

   - The scripts for zero-shot inference with LLMs and MLLMs are located in the `examples/Zero_shot` directory. This directory contains two subdirectories, `llm` and `mllm`, which include scripts for zero-shot inference of LLMs and MLLMs, respectively.

   - Example executions for zero-shot inference with LLMs (Qwen2 series, Llama3 series, and Internlm):

     ```bash
     # Execute zero-shot inference for Qwen2-7B
     python Zero-shot/llm/python/Qwen-2_7B_inference.py
     
     # Execute zero-shot inference for Llama3-8B
     python Zero-shot/llm/python/llama-3_8B_inference.py
     
     # Execute zero-shot inference for Internlm2.5-8B
     python Zero-shot/llm/python/Internlm_2_5_8B_inference.py
     ```

   - Example executions for zero-shot inference with MLLMs (Qwen2-VL-7B, Qwen2-VL-72B):

     ```bash
     # Execute zero-shot inference for Qwen2-VL-7B and Qwen2-VL-72B
     bash Zero-shot/mllm/bash/run_zero_qwen_all.sh
     ```

   **Supervised Fine-Tuning and Instruction Fine-Tuning Scripts**

   - For LLMs, the supervised fine-tuning and instruction fine-tuning scripts are located in the `examples/train_bash/llm` directory. This directory contains two executable scripts for fine-tuning, along with test scripts for evaluating the models post-fine-tuning, located in the `examples/test_bash/llm` directory.

   - Example executions for supervised fine-tuning and instruction fine-tuning for LLM:

     ```bash
     # Execute supervised fine-tuning for LLMs
     bash train_bash/llm/llms_all_sft.sh
     
     # Execute instruction fine-tuning for LLMs
     bash train_bash/llm/llms_all_instruct.sh
     ```

   - Example test script executions for evaluating the performance of LLMs post-fine-tuning:

     ```bash
     # Test the Qwen2-7B model after supervised fine-tuning
     bash test_bash/llm/sft/qwen2_7B_sft.sh
     
     # Test the Qwen2-7B model after instruction fine-tuning
     bash test_bash/llm/It/qwen2_7B_It.sh
     ```

   - For MLLMs, the supervised fine-tuning and instruction fine-tuning scripts are located in the `examples/train_bash/mllm` directory. This directory includes both supervised fine-tuning (sft) and instruction fine-tuning (It) subdirectories.

   - Example executions for MLLMs fine-tuning:

     ```bash
     # Execute supervised fine-tuning and inference for Qwen2-VL-7B
     bash train_bash/mllm/sft/bash/run_total_7b.sh
     
     # Execute supervised fine-tuning and inference for Qwen2-VL-72B
     bash train_bash/mllm/sft/bash/run_total_72b.sh
     
     # Execute instruction fine-tuning for Qwen2-VL-7B
     bash train_bash/mllm/It/bash/run_total_7b_instruct.sh
     
     # Execute inference after instruction fine-tuning for Qwen2-VL-7B
     bash train_bash/mllm/It/bash/run_total_7b_instruct_infer.sh
     
     # Execute instruction fine-tuning for Qwen2-VL-72B
     bash train_bash/mllm/It/bash/run_total_72b_instruct.sh
     
     # Execute inference after instruction fine-tuning for Qwen2-VL-72B
     bash train_bash/mllm/It/bash/run_total_72b_instruct_infer.sh
     ```


