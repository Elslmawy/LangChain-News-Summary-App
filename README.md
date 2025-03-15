## George Nashat  21100825
## Mohamed Elslmawy  21100809
# LangChain News Summary App  

This application fetches news articles based on user input, processes them, and generates a summary using LangChain and Groq's Llama3 model.

## Features

Fetches news articles from NewsAPI.

Uses a sentence transformer model for text processing.

Summarizes fetched articles using a Groq-powered language model.

Saves user preferences for future queries.  

 
---

## Project Structure  

```
📦 langchain-news-app
├── 📂 data                 # Stores user preferences and cached data
├── 📂 models               # Contains pre-trained language models (if needed)
├── 📂 src                  # Source code of the application
│   ├── langchain_news_app.py  # Main application script
│   ├── utils.py            # Helper functions (optional)
├── requirements.txt        # List of dependencies
├── README.md               # Documentation
```

---

## Installation  

1. **Clone the Repository**  
   ```bash
   git clone https://github.com/your-repo/langchain-news-app.git
   cd langchain-news-app
   ```

2. **Install dependencies:**  
   ```bash
    pip install -r requirements.txt
   ```

3. **Set API keys as environment variables or enter them when prompted:**  
   ```bash
   export NEWS_API_KEY=your_newsapi_key
   export GROQ_API_KEY=your_groq_api_key
   ```

---

## Usage  

Run the application using:  

```bash
python src/langchain_news_app.py
```

## Example Output
```bash
Enter a topic to fetch news: AI Technology

Fetched Articles:
1. OpenAI Releases New Model - AI innovation is accelerating...
2. Google's AI Research Breakthrough - New transformer model...
...

Generated Summary:
Recent AI advancements include OpenAI's latest model...
```


## How It Works  

The user enters a topic of interest.

The application fetches relevant news articles from NewsAPI.

The retrieved articles are processed, extracting titles and descriptions.

The extracted text is passed to Groq's Llama3 model for summarization.

The generated summary is displayed to the user.

User preferences, including the last searched query, are saved for future use.
