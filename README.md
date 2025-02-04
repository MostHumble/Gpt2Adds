# GPT Addition Experiment  
Exploring GPT-2's ability to learn addition by analyzing attention maps and testing different training approaches.  

## Attention scores

For example, the attention scores of the "=" token (when predicting the next token, i.e., 3) show that it focuses heavily on the "2" from "23" and the "1" from "12," while almost completely ignoring the "3" and "2" from the respective operands.  

![attention_map](https://github.com/user-attachments/assets/7b208cd5-a0cc-40d1-9de7-696aa9022857)

## Left vs Right Padding

Left padding converges much slower, and to a worse state than right padding

Left padding:

![download](https://github.com/user-attachments/assets/aba93f9f-8232-455e-8e52-2f956699308a)

Right padding:

![download](https://github.com/user-attachments/assets/8d3913e6-e496-4d2d-b6e8-f3a1a833d174)

Current hypothesis is that it's due to the 'absolute' positionnal embedding.

