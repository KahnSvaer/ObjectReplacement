# Object Detection and Replacement Project

## Overview
This project utilizes AI models to detect objects in images and replace them with new content. The system performs the following tasks:

- Detects objects using a zero-shot detection model (Grounding DINO).
- Generates segmentation masks using Segment Anything (SAM).
- Replaces the detected objects with new content via Stable Diffusion XL inpainting, driven by text prompts.

## Requirements
- Python 3.x
- Libraries: `torch`, `transformers`, `diffusers`, `cv2`, `PIL`, `requests`, `numpy`

## Installation
1. Clone the repository.
2. Install the dependencies using:
    ```bash
    pip install diffusers transformers accelerate torch -U
    ```
3. Login to HuggingFace Hub:
    ```bash
    from huggingface_hub import login
    login(token="your_huggingface_token")
    ```
4. Use the script to process images.

## Usage
Run the script and provide an image URL and desired labels. The system will detect objects, generate masks, and replace the objects in the image based on the prompt.

## Result
![ObjectReplacementResult](https://github.com/user-attachments/assets/87191f69-fc22-43e1-a96b-27e117e229bd)


## License
This project is licensed under the [MIT License](./LICENSE). See the LICENSE file for more details.

------
