
# Calorie Advisor App

This Streamlit app uses Google Gemini to estimate the calorie content of food from an uploaded image.

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/your-repository.git
   ```
2. **Install dependencies:**
   ```bash
   pip install streamlit google-generativeai python-dotenv Pillow
   ```
3. **Set up a Google Gemini API Key:**
   - Obtain an API key from [Google AI](https://developers.google.com/workspace/generative-ai).
   - Create a `.env` file in the project directory and add the following line:
     ```
     GOOGLE_API_KEY=YOUR_API_KEY
     ```

## Usage

1. **Run the app:**
   ```bash
   streamlit run app.py
   ```
2. **Upload an image:** Use the file uploader to select an image of food.
3. **(Optional) Add context:** Provide additional details in the input prompt.
4. **Click "Tell me about the total calories":** The app will send the image and prompt to Google Gemini and display the estimated calorie information.

## How it Works

The app uses the `google-generativeai` library to interact with the Gemini API.  It sends the uploaded image and user prompt to the model, which then returns a text response containing the calorie estimations.  The `PIL` library is used for handling image uploads.

## Limitations

* Calorie estimations are based on visual analysis and may not be perfectly accurate.
* The app relies on the availability and performance of the Google Gemini API.

## Contributing

Contributions are welcome! Feel free to open issues and pull requests.

## License

[MIT](LICENSE) (or specify your actual license)
```
