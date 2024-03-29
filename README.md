# Image Caption Generator

The Image Caption Generator is a fascinating deep learning application that utilizes the power of transformers to generate textual captions for images. It combines Computer Vision and Natural Language Processing (NLP) techniques to understand the contents of an image and generate relevant and coherent captions. The project is built using the Python programming language and leverages the popular libraries like Streamlit, Hugging Face Transformers, PyTorch, and PIL.

## How it Works:

1. **Streamlit Interface:** The project provides an intuitive and user-friendly interface created with Streamlit, a web application framework. Users can upload an image through the file uploader on the webpage.

2. **Image Processing:** The uploaded image is processed using the PIL (Python Imaging Library) module to ensure it is in the RGB format, as required by the VisionEncoderDecoderModel.

3. **Transformers & Hugging Face:** The core of the image caption generation relies on transformers, a type of deep learning model architecture based on self-attention mechanisms. Hugging Face's Transformers library is used to load the pre-trained VisionEncoderDecoderModel and the ViTFeatureExtractor.

4. **Feature Extraction:** The ViTFeatureExtractor is used to extract visual features from the image. The image's pixel values are passed through the feature extractor, which transforms the image into a format suitable for the transformer model.

5. **Generating Captions:** The loaded VisionEncoderDecoderModel is responsible for generating the captions. The transformer model takes the visual features as input and generates a sequence of tokens representing the caption. The process involves beam search with a specified number of beams to improve the quality of the captions.

6. **Displaying the Results:** The generated caption is displayed below the uploaded image on the webpage. The caption is shown in a large and bold font, making it visually appealing to the user.

## Output Images:

<div style="display: flex;">
<img src="https://github.com/sdrahmath/Image-Caption-Generator/blob/main/outputs/Screenshot_1.jpg" alt="Image 1" width="350" height="350">
<img src="https://github.com/sdrahmath/Image-Caption-Generator/blob/main/outputs/Screenshot_2.jpg" alt="Image 1" width="350" height="350">
</div>


## Libraries and Technologies Used:

1. **Streamlit:** Streamlit is a Python library used for building interactive web applications with minimal code. It allows data scientists and developers to turn data scripts into shareable web apps effortlessly.

2. **Hugging Face Transformers:** The Transformers library from Hugging Face provides easy access to pre-trained transformer-based models for NLP and computer vision tasks. It enables rapid prototyping and integration of transformer models into applications.

3. **PyTorch:** PyTorch is an open-source machine learning library that provides a flexible and efficient framework for building deep learning models. It is widely used for training and deploying neural networks.

4. **PIL (Python Imaging Library):** PIL is a library that adds image processing capabilities to Python. It is used in this project to handle image operations, such as converting the image to RGB format.

## How to Use:

1. Clone this repository to your local machine.
2. Install the required libraries listed in the `requirements.txt` file.
3. Run the Streamlit app using the command `streamlit run app.py`.
4. Access the web application in your browser at the provided local address.

## Conclusion:

The Image Caption Generator project showcases the synergy between Computer Vision and Natural Language Processing. By combining the power of transformers with a user-friendly interface created using Streamlit, this application makes it easy for users to generate captions for their images. It can be used in various scenarios, including enhancing accessibility for visually impaired individuals, aiding content creators, and facilitating better image understanding in AI systems.
