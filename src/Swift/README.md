This module utilizes the **Swift framework** to perform zero-shot inference, supervised fine-tuning, and instruction fine-tuning on the **MiniCPM-V-8B** MLLM. Swift is an open-source framework under the [modelscope](https://github.com/modelscope/ms-swift/?tab=readme-ov-file) community, designed to support fine-tuning of the MiniCPM-V-8B.

1. The `video_prompt_data` directory contains 12 types of multimodal datasets suitable for the Swift framework, each divided into training, validation, and test sets.

2. The `examples` directory contains scripts for performing zero-shot inference, supervised fine-tuning, instruction fine-tuning, and testing of MiniCPM.

   Example script executions for MiniCPM-2.6-V-8B:

   ```bash
   # Perform zero-shot inference
   bash examples/bash/run_zero_infer.sh
     
   # Perform supervised fine-tuning
   bash examples/bash/run_sft_infer.sh
     
   # Perform instruction fine-tuning
   bash examples/bash/run_instruct.sh
     
   # Perform inference after instruction fine-tuning
   bash examples/bash/run_instruct_infer.sh
   ```


