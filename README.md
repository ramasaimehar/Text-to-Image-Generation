# Text-to-Image-Generation
This project is a Streamlit web app for generating images using OpenAI's DALL·E 2 model. Users input a text prompt and select an image size (256x256, 512x512, 1024x1024). Upon clicking "See Magic🪄", the app generates and displays the image. Users can download the image via a provided download button. The app includes custom CSS for improved UI.

## Overview

This project demonstrates the creation of a "Text to Image" application using Python, OpenAI, and Streamlit. The following technologies and services are used:

- `Streamlit` as a server and handling front end.
- OpenAI API key from `OpenAI`.
- `DALL.E-2` model for text-to-image generation. 
- `AWS EC2` for deployment (24/7 running).

## Steps

1. Create free accounts on [OpenAI](https://platform.openai.com/account/api-keys) and [AWS](https://console.aws.amazon.com/).
2. Create a Streamlit App.
3. Create an EC2 instance on AWS.
4. Git clone this repository on the EC2 instance.
5. Install the requirements.
6. Use the `OPENAI_API_KEY` in your code (avoid using static values, use global variables).
7. Run the script on the EC2 instance.

## Usage

To use this project:

1. Clone the repository.
2. Open a terminal in the working directory.
3. Run the following command to install the required dependencies:
    ```
    pip install -r requirements.txt
    ```
4. Set the `OPENAI_API_KEY` (replace `-------API KEY--------` with your actual API key):
    ```
   OPENAI_API_KEY="-------API KEY--------"
    ```
5. The `App.py` file contains the Streamlit application.
6. Run the script with the following command:
    ```
    python3 streamlit run App.py
    ```
7. To stop the running application:
   - Get the process ID of the running process:
     ```
     ps -ef 
     ```
   - Kill the process using its ID:
     ```
     kill [PROCESS_ID]
     ```




