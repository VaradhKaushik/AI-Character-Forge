# AI Video Game Character Generator

## Overview
This project harnesses the power of Stable Diffusion, DreamBooth, and LoRa technologies to generate highly customizable and unique video game characters. Developed as part of the CS 6140 course by Alexander Seljuk, Girish Kumar Adari, and Varadh Kaushik, this system aids creatives in generating detailed character images, boosting creativity and offering a vast array of character design possibilities.

## Features
- **Custom Character Generation**: Create video game characters with unique visual traits and attributes.
- **Advanced Fine-Tuning**: Utilizes DreamBooth and LoRa for precise model tuning and enhancement.
- **High Flexibility**: Suitable for a wide range of games and character styles.

## Technical Details
### Technology Stack
- **Stable Diffusion**: For base character image generation.
- **DreamBooth**: For fine-tuning the general-purpose model to recognize and generate new specific characters.
- **LoRa (Low Rank Adaptation)**: Applied for lightweight and efficient model fine-tuning, focusing on enhancing specific aspects of the generated characters.

### Dataset
The dataset consists of 31,800 images collected from 12 different video games, with deep labeling using tools like DeepDanBooru and Blip for accurate attribute classification.

### Model Architecture
- **Base Model**: Stable Diffusion v1.5, generating detailed base images.
- **DreamBooth Adaptation**: Enhances the model's ability to generate new, specific characters without losing general capabilities.
- **LoRa Adaptation**: Provides targeted improvements with minimal computational resources, suitable for single character enhancements.

## Installation
```bash
git clone https://github.com/VaradhKaushik/Ai-character-generation.git
cd Ai-character-generation
pip install -r requirements.txt
```

## Future Scope
- The next step is to try different models with this approach.
- Fine-tune the model on a high-resolution dataset.
- Comibne LoRA and our DreamBooth trained model.
- Try training style, clothing, concept LoRAs and compare results.
- Explore the use of LyCORIS for model fine-tuning.

## References
- https://huggingface.co/runwayml/stable-diffusion-v1-5
- https://github.com/ShivamShrirao/diffusers/tree/main/examples/dreambooth
- https://huggingface.co/blog/stable_diffusion
- https://huggingface.co/docs/diffusers/training/lora?installation=PyTorch
- https://github.com/huggingface/diffusers/tree/main/examples/text_to_image
- https://civitai.com/models/4468?modelVersionId=57618
- https://github.com/AUTOMATIC1111/stable-diffusion-webui
- https://huggingface.co/openai/clip-vit-base-patch32
- https://github.com/KichangKim/DeepDanbooru

## Team Members
Alexander Seljuk, Varadh Kaushik, Girish Adari Kumar
