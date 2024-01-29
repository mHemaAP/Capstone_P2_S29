# Capstone_P2_S29
This is the repository covers the part2 (S29) of the Capstone

In part2, we perform the training in the following steps:
#### Stage1
-- Step 1: Generate image embeddings for the images from Coco 2017 dataset. (This is because the original llava 150k dataset has referred to Coco dataset). We use a CLIP model to generate these embeddings. 

#### Stage2
-- Step 2: We use the image embeddings obtained from step 1 to train our image projector layer from scratch, as mentioned in the guidelines above for image File: S29_stage2.ipnyb

Courtesy - Image projector layer code referenced from open source code: https://github.com/sshh12/multi_token/blob/81ee75cd4435ebd5c7c7c3cf42c136c4053320fb/multi_token/modalities/projectors.py

-- Step 3: We use the now trained projection model and fine tune it along woth Phi-2 model, as mentioned in training guidelines for image. File: S29_stage1.ipnyb

We now use these trained models to implement the multimodal chat GPT application in Hugging Face Spaces

The application implemented using basic gradio interface on huggingface: HF Link: https://huggingface.co/spaces/HemaAM/Multimodal_GPT

