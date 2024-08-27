The YouTube Video Transcribe Summarizer App is is designed to take the transcript from a YouTube video and generate a summarized version of the content using Google Gemini Pro.

Working:-

Environment Setup: The app loads environment variables using the dotenv package, particularly to access the Google API key needed for Gemini Pro.

Transcript Extraction: The app retrieves the transcript of a YouTube video using the YouTubeTranscriptApi package.
It extracts the video ID from the provided YouTube link and uses it to fetch the transcript, compiling all the transcript parts into a single string.

Content Generation: A pre-defined prompt instructs the LLM (Google Gemini Pro) to summarize the transcript into important points within 250 words.
The summary generation function sends the transcript text combined with the prompt to the Gemini Pro API to obtain the summarized content.

User Interface: The app provides a text input field for the user to enter a YouTube video link.
Upon entering the link, the app displays a thumbnail of the video.
When the user clicks "Get Detailed Notes," the app extracts the transcript, generates a summary, and displays it on the screen.

