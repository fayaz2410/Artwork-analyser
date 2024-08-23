# Artwork emotion analysis

 This Flask application allows users to input an image URL, which is then processed to generate a descriptive caption and analyze the emotional tone of that caption using pre-trained models hosted on Hugging Face.

# Features

 **Image Captioning:** Automatically generates a descriptive caption for any given image using the Salesforce BLIP Image Captioning model.

 **Sentiment Analysis:** Analyzes the sentiment of the generated caption using the CardiffNLP Twitter RoBERTa sentiment model, classifying it as Happy, Neutral, or Sad.

# Prerequisites

 Python 3.x: Make sure you have Python installed. You can download it from python.org.

 Flask: Web framework used to build this application.

 Requests: Library for making HTTP requests.

 Pillow: Library for image processing.

 Hugging Face API Key: Access token for Hugging Face models.

# Installation


1. **Clone the Repository**


    ```bash

    git clone -b master https://github.com/fayaz2410/artwork-emotion-analysis.git
   
    cd artwork-emotion-analysis

2. **Create a Virtual Environment (Optional but recommended):**
   
   ```bash
   
   python3 -m venv venv

   source venv/bin/activate  # On Windows use `venv\Scripts\activate`

3. **Install Dependencies:**
     
    ```bash
    
     pip install -r requirements.txt

4. **Set Up Environment Variables:**

    Replace the placeholder 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 with your actual Hugging Face API key in the app.py file.

5. **Run the Application:**
     
    ```bash

    python app.py

6. **Access the Application:**

    Open your browser and go to http://0.0.0.0:5000/ or http://localhost:5000/.

7. **Usage**

   Enter an Image URL: On the homepage, paste the URL of the image you want to analyze.

   Get the Caption and Emotion: The application will generate a descriptive caption for the image and analyze its emotional tone.

   View Results: The caption and detected emotion will be displayed on the same page along with the image.

8. **Files and Directories**

   app.py: Main Flask application file.

   templates/: Contains HTML templates for rendering web pages.

   index.html: The main template for the homepage.

   requirements.txt: Lists all the Python dependencies required to run the application.

9. **API Models Used**

    Image Captioning: Salesforce/blip-image-captioning-large

    Sentiment Analysis: cardiffnlp/twitter-roberta-base-sentiment

10. **Deployment**

     The application can be deployed on any platform that supports Flask applications. Ensure that you have properly set up the environment variables and installed the required dependencies.

11. **Troubleshooting**

     Invalid API Key: Ensure that your Hugging Face API key is correctly set.

     Missing Dependencies: Run pip install -r requirements.txt to ensure all dependencies are installed.

12. **Acknowledgments**

    Hugging Face for providing the powerful models used in this application.

    Flask, for being an excellent and lightweight web framework



   
   
