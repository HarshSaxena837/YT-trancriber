# YouTube Transcript to Detailed Notes Converter

This project is a Streamlit web application that extracts the transcript from a YouTube video and summarizes it into detailed notes using Google's Generative AI model. The application is designed to provide a concise and important summary of the video transcript in points, within 250 words.

## Features

- Extracts transcript data from YouTube videos.
- Summarizes the transcript into detailed notes.
- Utilizes Google Gemini Pro for generating the summary.
- Provides a user-friendly interface for inputting YouTube video links and displaying summaries.

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/HarshSaxena837/YT-trancriber.git
   cd YT-trancriber
   ```

2. **Create and activate a virtual environment:**

   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows, use `venv\Scripts\activate`
   ```

3. **Install the required packages:**

   ```bash
   pip install -r requirements.txt
   ```

4. **Set up environment variables:**

   Create a `.env` file in the root directory of your project and add your Google API key:

   ```env
   GOOGLE_API_KEY=your_google_api_key
   ```

## Usage

1. **Run the Streamlit application:**

   ```bash
   streamlit run app.py
   ```

2. **Open your browser and navigate to:**

   ```
   http://localhost:8501
   ```

3. **Use the application:**

   - Enter the YouTube video link in the provided input box.
   - Click the "Get Detailed Notes" button to extract and summarize the transcript.
   - View the detailed notes displayed on the page.

## Code Overview

- **app.py:** The main application file that contains the Streamlit code and functions for extracting transcripts and generating summaries.

### Key Functions

- `extract_transcript_details(youtube_video_url)`: Extracts transcript data from a YouTube video given its URL.
- `generate_gemini_content(transcript_text, prompt)`: Generates a summary of the transcript using Google's Generative AI model.

## Contributing

1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -m 'Add YourFeature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a pull request.



## Acknowledgments

- [Streamlit](https://www.streamlit.io/) for the awesome web app framework.
- [YouTube Transcript API](https://pypi.org/project/youtube-transcript-api/) for providing easy access to YouTube video transcripts.
- [Google Generative AI](https://developers.google.com/generative-ai) for the powerful AI model used for summarization.

---
