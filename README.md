# Mini Projects: Sentiment Analysis and English-to-Urdu Translator

This repository contains two mini projects that utilize natural language processing (NLP) to perform useful tasks: **Sentiment Analysis** and **English-to-Urdu Translation**. Both projects provide web applications that are easy to use, with interactive interfaces for analyzing sentiments or translating text.

## Project Overview

1. **Sentiment Analysis**: A web application that analyzes the sentiment of an input text, categorizing it as **Positive**, **Negative**, or **Neutral**. This project provides users with insights into the emotional tone of the provided content.
2. **English-to-Urdu Translator**: A web application that allows users to translate English text into Urdu, making it useful for communication and understanding across different language speakers.

Both projects are deployed using **Streamlit**, making them accessible via a web interface, and leverage the **Hugging Face API** for the underlying NLP tasks. Additionally, **LangChain** is used to manage and orchestrate the interactions between different components, enabling flexibility and scalability for these projects.

---

## Project 1: Sentiment Analysis

### Overview
The **Sentiment Analysis** project is a simple yet effective tool for determining the emotional tone of a given piece of text. Users can input any text, such as product reviews, social media comments, or general statements, and the application will classify the sentiment as **Positive**, **Negative**, or **Neutral**. This helps users understand how others may perceive a given message or statement.

### Technologies Used
- **Streamlit**: Utilized to develop an interactive and user-friendly web application. Streamlit enables users to input text directly into the interface and receive results instantaneously.
- **Hugging Face Transformers**: The core model for sentiment analysis is provided by the Hugging Face `pipeline`. Specifically, we use models such as `distilbert-base-uncased-finetuned-sst-2-english` for accurate sentiment predictions.
- **LangChain**: This project also integrates LangChain, which helps in orchestrating the models and makes future extensions possible by enabling complex workflows or multiple model integrations.

### Features
- **User Input**: Accepts any user-provided text through a web interface.
- **Sentiment Detection**: Analyzes the sentiment of the input text and classifies it as **Positive**, **Negative**, or **Neutral**.
- **Confidence Score**: Alongside the sentiment label, the model provides a confidence score, which indicates the certainty of the classification.
- **Interactive UI**: Built using Streamlit, making it accessible and straightforward for users.

### How It Works
The user enters text into the provided input field, and the model analyzes the sentiment using a pre-trained Hugging Face model. The results are displayed instantly, along with a confidence score to help gauge the reliability of the classification.

### Example Usage
- **Customer Reviews**: Determine whether customer feedback on a product or service is positive, negative, or neutral.
- **Social Media Monitoring**: Analyze comments or posts to understand public sentiment towards a topic or event.

---

## Project 2: English-to-Urdu Translator

### Overview
The **English-to-Urdu Translator** project provides a convenient tool for translating text from English to Urdu. This is particularly useful for breaking language barriers and enabling better communication among speakers of these two languages. The translation is performed in real-time, allowing users to quickly obtain results and use them as needed.

### Technologies Used
- **Streamlit**: The web application is built using Streamlit, providing an easy-to-use interface where users can input English text and receive Urdu translations.
- **Hugging Face Transformers**: The translation task is handled by leveraging models available through the Hugging Face API. This ensures accurate and context-aware translations for input text.
- **LangChain**: LangChain is employed to orchestrate the workflow between the NLP models, making it easy to manage the translation process and integrate additional functionality in the future.

### Features
- **User Input**: Users can provide any text in English that they wish to translate.
- **Real-Time Translation**: The model processes the input text and returns the translated text in Urdu in real time.
- **Simple Interface**: Streamlit’s interactive components make it easy for users to input their text and view the translated result without any hassle.

### How It Works
Users enter a piece of text in English into the input field. The translation model, provided by Hugging Face, processes this input and returns the translated text in Urdu, displayed on the same page. This helps users obtain translations quickly and effectively.

### Example Usage
- **Learning and Communication**: Useful for learners trying to understand Urdu from English texts or for anyone who needs a quick translation tool for communication.
- **Business Use**: Businesses that work with Urdu-speaking clients can use the translator to help bridge communication gaps.

---

## Getting Started

### Installation
To run these projects locally, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/sentiment-translator-mini-projects.git
   cd sentiment-translator-mini-projects
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the applications**:
   - **Sentiment Analysis**:
     ```bash
     streamlit run sentiment_analysis_app.py
     ```
   - **English-to-Urdu Translator**:
     ```bash
     streamlit run english_to_urdu_translator_app.py
     ```

### Prerequisites
- **Python 3.7+**
- **Streamlit** for creating the web interface
- **Hugging Face Transformers** for NLP models
- **LangChain** for managing the flow between models

---

## Future Improvements
- **Additional Languages**: Expand the translator to include more languages.
- **Sentiment Analysis Enhancements**: Include more granular sentiment analysis such as emotions (happy, sad, angry).
- **Deploy to Hugging Face Spaces**: Deploy these apps on Hugging Face Spaces to make them even more accessible to a wider audience.

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
