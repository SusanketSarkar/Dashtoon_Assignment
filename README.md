# Style Transfer with Dashtoon
Assignment submission for Dashtoon by **Susanket Sarkar**

## Introduction
Style transfer is an artistic technique that involves transforming the visual style of an image in the manner of another image. This assignment focuses on implementing style transfer using neural networks, specifically the VGG19 model. The goal is to generate images that combine the content of a base image with the artistic style of a reference image.

![Heading Image 1](path/to/base_image_1)

## Problem Statement
The task is to develop a Python script for style transfer between travel and adventure images (base images) and artworks by Paul Klee (style images). The implementation utilizes the VGG19 neural network and L-BFGS optimization to generate images that blend the content of the travel images with the artistic style of Paul Klee's paintings.

## Implementation Steps

### 1. Image Preprocessing
Images are loaded and preprocessed using the VGG19 preprocessing function. The base image and style image paths are specified.

### 2. VGG19 Model Setup
The VGG19 model is loaded with pre-trained ImageNet weights, excluding the top classification layers. Content and style layers are selected for feature extraction.

### 3. Content and Style Loss Functions
Loss functions for content and style are defined based on the Mean Squared Error and Gram matrices, respectively.

### 4. Gradient Calculation
The gradients of the generated image with respect to the total loss are computed.

### 5. L-BFGS Optimization
The L-BFGS optimization algorithm is used to minimize the total loss, updating the generated image.

### 6. Result Visualization
The final stylized image is deprocessed to its original format and displayed alongside the base and style images.

## Usage
To run the style transfer on your own images, follow these steps:
1. Specify the paths for the base and style images in the `base_image_path` and `style_image_path` variables.
2. Run the `Run_StyleTransfer` function, providing the base and style image paths as arguments.
3. The function will return the final stylized image, which can be visualized using Matplotlib.

## Example Results
Three examples of style transfer are provided, showcasing the transformation of travel and adventure images with Paul Klee's artistic style.

### Example 1
- Base Image: ![Base Image 1](path/to/base_image_1)
- Style Image: ![Style Image 1](path/to/style_image_1)
- Final Image: ![Final Image 1](path/to/final_image_1)

### Example 2
- Base Image: ![Base Image 2](path/to/base_image_2)
- Style Image: ![Style Image 2](path/to/style_image_2)
- Final Image: ![Final Image 2](path/to/final_image_2)

### Example 3
- Base Image: ![Base Image 3](path/to/base_image_3)
- Style Image: ![Style Image 3](path/to/style_image_3)
- Final Image: ![Final Image 3](path/to/final_image_3)

## Conclusion
The style transfer script successfully blends the content of travel images with the artistic style of Paul Klee, creating visually appealing and unique compositions. Experiment with different base and style images to explore the versatility of the style transfer technique.
