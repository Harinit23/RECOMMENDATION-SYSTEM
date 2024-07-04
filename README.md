This project aims to transcribe audio to text using a speech recognition model and then identify and scrape product-related information from e-commerce websites based on the transcribed text. Here is a step-by-step summary:

1. Importing Libraries:
   Torch: For handling tensor operations and utilizing the Wav2Vec2 model.
   Librosa: For audio processing.
   NumPy: For numerical operations.
   Soundfile and scipy.io.wavfile: For reading audio files.
   IPython.display.Audio: For playing audio in Jupyter Notebooks.
   Transformers: For loading the Wav2Vec2 model and tokenizer.
   TextBlob: For natural language processing tasks.
   NLTK: For tokenization.
   Requests and BeautifulSoup: For web scraping.
2. Downloading NLTK Data:
   Download necessary NLTK data for tokenization.
3. Loading Wav2Vec2 Model and Tokenizer:
   Load the Wav2Vec2 tokenizer and model from Hugging Face.
4. Reading and Playing Audio File:
   Read the audio file cosmetic.wav.
   Play the audio file.
5. Transcribing Audio to Text:
   Process the audio file using Librosa.
   Tokenize the audio input and get the model's predictions.
   Decode the predictions to get the transcription.
   Print the transcribed text.
6. Lowercasing Transcription:
   Convert the transcribed text to lowercase for uniformity.
7. Identifying Product-related Words:
   Define a list of product-related words.
   Extract noun phrases from the transcription using TextBlob.
   Match extracted noun phrases with the product-related words list.
   Print matched product-related words.
8. Web Scraping for Product Information:
   Define a function to scrape product URLs from Flipkart based on product categories.
   Construct the search URL and fetch the webpage content.
   Parse the HTML to extract product links.
   Print the product URLs.
9. Main Execution:
   Extract product-related words from the transcribed text.
   Clean the extracted words to remove spaces.
   Scrape product information for each category from Flipkart.
Note:
   The scraping function is set up to scrape from Flipkart, but the output message refers to Amazon, which can be corrected.
   Ensure that all the necessary libraries are installed and imported correctly.
   Handle edge cases and potential errors, such as missing audio files or HTTP request failures.
   This project demonstrates a complete pipeline from audio transcription to web scraping for product information,
        showcasing practical applications of machine learning and natural language processing in e-commerce.






