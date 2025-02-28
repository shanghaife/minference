.. _models_llm_vicuna-v1.3:

========================================
vicuna-v1.3
========================================

- **Context Length:** 2048
- **Model Name:** vicuna-v1.3
- **Languages:** en
- **Abilities:** chat
- **Description:** Vicuna is an open-source LLM trained by fine-tuning LLaMA on data collected from ShareGPT.

Specifications
^^^^^^^^^^^^^^


Model Spec 1 (ggmlv3, 7 Billion)
++++++++++++++++++++++++++++++++++++++++

- **Model Format:** ggmlv3
- **Model Size (in billions):** 7
- **Quantizations:** q2_K, q3_K_L, q3_K_M, q3_K_S, q4_0, q4_1, q4_K_M, q4_K_S, q5_0, q5_1, q5_K_M, q5_K_S, q6_K, q8_0
- **Model ID:** TheBloke/vicuna-7B-v1.3-GGML

Execute the following command to launch the model, remember to replace ``${quantization}`` with your
chosen quantization method from the options listed above::

   xinference launch --model-name vicuna-v1.3 --size-in-billions 7 --model-format ggmlv3 --quantization ${quantization}


Model Spec 2 (ggmlv3, 13 Billion)
++++++++++++++++++++++++++++++++++++++++

- **Model Format:** ggmlv3
- **Model Size (in billions):** 13
- **Quantizations:** q2_K, q3_K_L, q3_K_M, q3_K_S, q4_0, q4_1, q4_K_M, q4_K_S, q5_0, q5_1, q5_K_M, q5_K_S, q6_K, q8_0
- **Model ID:** TheBloke/vicuna-13b-v1.3.0-GGML

Execute the following command to launch the model, remember to replace ``${quantization}`` with your
chosen quantization method from the options listed above::

   xinference launch --model-name vicuna-v1.3 --size-in-billions 13 --model-format ggmlv3 --quantization ${quantization}


Model Spec 3 (ggmlv3, 33 Billion)
++++++++++++++++++++++++++++++++++++++++

- **Model Format:** ggmlv3
- **Model Size (in billions):** 33
- **Quantizations:** q2_K, q3_K_L, q3_K_M, q3_K_S, q4_0, q4_1, q4_K_M, q4_K_S, q5_0, q5_1, q5_K_M, q5_K_S, q6_K, q8_0
- **Model ID:** TheBloke/vicuna-33B-GGML

Execute the following command to launch the model, remember to replace ``${quantization}`` with your
chosen quantization method from the options listed above::

   xinference launch --model-name vicuna-v1.3 --size-in-billions 33 --model-format ggmlv3 --quantization ${quantization}


Model Spec 4 (pytorch, 33 Billion)
++++++++++++++++++++++++++++++++++++++++

- **Model Format:** pytorch
- **Model Size (in billions):** 33
- **Quantizations:** 4-bit, 8-bit, none
- **Model ID:** lmsys/vicuna-33b-v1.3

Execute the following command to launch the model, remember to replace ``${quantization}`` with your
chosen quantization method from the options listed above::

   xinference launch --model-name vicuna-v1.3 --size-in-billions 33 --model-format pytorch --quantization ${quantization}


Model Spec 5 (pytorch, 13 Billion)
++++++++++++++++++++++++++++++++++++++++

- **Model Format:** pytorch
- **Model Size (in billions):** 13
- **Quantizations:** 4-bit, 8-bit, none
- **Model ID:** lmsys/vicuna-13b-v1.3

Execute the following command to launch the model, remember to replace ``${quantization}`` with your
chosen quantization method from the options listed above::

   xinference launch --model-name vicuna-v1.3 --size-in-billions 13 --model-format pytorch --quantization ${quantization}


Model Spec 6 (pytorch, 7 Billion)
++++++++++++++++++++++++++++++++++++++++

- **Model Format:** pytorch
- **Model Size (in billions):** 7
- **Quantizations:** 4-bit, 8-bit, none
- **Model ID:** lmsys/vicuna-7b-v1.3

Execute the following command to launch the model, remember to replace ``${quantization}`` with your
chosen quantization method from the options listed above::

   xinference launch --model-name vicuna-v1.3 --size-in-billions 7 --model-format pytorch --quantization ${quantization}

