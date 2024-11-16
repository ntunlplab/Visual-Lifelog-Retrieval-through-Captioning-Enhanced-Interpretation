# Visual-Lifelog-Retrieval-through-Captioning-Enhanced-Interpretation

## Data Description
This repository contains detailed image captions generated by various advanced AI models. The dataset is based on the NTCIR-14 Lifelog-3 lifelog image dataset and provides rich, descriptive captions for each image. Each image is represented with multiple captioning outputs and a structured breakdown of interpretations.

## Data Structure
The dataset is organized as a dictionary where the keys represent image file paths, and the values are JSON objects containing multiple captioning outputs and contextual summaries. Each entry includes:

- **id**: A unique identifier for the image.
- **Idefics2**: Caption generated by the Idefics2 model based on single caption method.
- **LLaVA-Next**: Caption generated by the LLaVA-Next-7B model based on single caption method.
- **Internlm-xcomposer2**: Caption generated by the Internlm-xcomposer2-7B model based on single caption method.
- **Video-LLaVA**: Caption generated by the Video-LLaVA model based on collective caption method.
- **Large-World-Model**: Caption generated by the Large-World-Model based on collective caption method.
- **GPT4-0613**:Caption generaged by GPT4-vision-turbo-0613 based on merged caption method.
  - **fine-grained**: Fine-grained caption generated by GPT4-turbo-vision based on merged method.
  - **coarse-grained**: Coarse-grained caption generated by GPT4-turbo-vision based on merged method.
  - **Experience-summary**: Summary of the experience depicted in the images generated by GPT4-turbo-vision based on merged method.

### Example Data Entry
```json
"../imageData/2018_05_03/B00001382_21I6X0_20180503_072333E.JPG": {
    "id": "u1_20180503_0617_i01",
    "Idefics2": "A person is holding a keyboard and water bottle.",
    "LLaVA-Next": "The image captures a moment of quiet solitude, as a person sits in a room, engrossed in the digital world. The individual, clad in a vibrant red sweater, is holding a smartphone in their hands, their fingers dancing over the screen. The phone is connected to a laptop, suggesting a work or study session in progress.\n\nThe room around them is a testament to their lifestyle, with a desk and a chair visible in the background. A backpack rests on the floor, perhaps holding more tools of their trade. A water bottle stands nearby, a silent reminder of the importance of hydration amidst long hours of screen time.\n\nThe time on the phone reads 06:17, hinting at the early morning hours. The person seems to be in the midst of a productive session, perhaps working on a project or studying for an exam. The image paints a picture of modern life, where technology plays a significant role in our daily routines.",
    "Internlm-xcomposer2": "At 06:17, a person is in their living room, holding a smartphone with a white cord attached to it. They are wearing a red sweater and a watch on their wrist.",
    "Video-LLaVA": "At 06:17, a person is holding a large piece of meat, which is wrapped in plastic. The meat appears to be a type of salmon, and the person is holding it up to the camera. The person is standing in a kitchen, and there are several other items visible in the background, including a sink, a refrigerator, and a microwave. The person seems to be proudly displaying the meat, possibly showcasing its size or quality.",
    "Large-World-Model": "The video shows a person using a toaster oven to make coffee. They place a cup of coffee on a plate and close the toaster oven. Then, they open the door of the oven and place a plate of food in it. The video also shows a hand holding a cup of coffee in a kitchen.",
    "GPT4-0613": {
        "fine-grained": "Person holding a cellphone with a charging cable connected.",
        "coarse-grained": "Morning routine in a residential setting, involving smartphone usage and preparing smoked salmon in the kitchen.",
        "Experience-summary": "The individual started their morning by handling their phone and preparing smoked salmon in a well-lit kitchen."
    }
}

## Download Link
https://drive.google.com/file/d/1bQjHri5YNmx4Z7n0CxmuZX5rrBLCEx1X/view?usp=sharing

## Contact

For any questions or issues, please open an issue in the repository or contact the author at [yfshih@nlg.csie.ntu.edu.tw].
