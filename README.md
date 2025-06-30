# Language Translation Tool

This project is a simple, client-side web application that provides a basic language translation tool. It allows users to input text, select source and target languages, and receive an instant translation powered by the Google Translate API.

## Features

*   **Text Input:** Easily enter text into a dedicated input area.
*   **Language Selection:** Intuitive dropdowns for choosing both the source and target languages from a predefined list.
*   **Real-time Translation:** Get translations quickly by interacting with the Google Translate API.
*   **Copy to Clipboard:** A convenient button to copy the translated text.
*   **Text-to-Speech:** A "Play" button that reads out the translated text aloud using the Web Speech API.
*   **Auto-detect Source Language:** Automatically identifies the language of the source text.
*   **Clean User Interface:** A simple and responsive design for easy usability.

## Technologies Used

*   **HTML5:** For the structure and content of the web page.
*   **CSS3:** For styling the user interface, making it visually appealing and responsive.
*   **JavaScript (ES6+):** For handling all the dynamic functionality, including:
    *   DOM manipulation to update the UI.
    *   Fetching data from the Google Translate API.
    *   Implementing copy-to-clipboard functionality (`navigator.clipboard.writeText`).
    *   Utilizing the Web Speech API for text-to-speech (`SpeechSynthesisUtterance`, `speechSynthesis.speak`).

## How to Use

1.  **Clone the Repository (or Save the Files):**
    If this code is part of a repository, clone it:
    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```
    Otherwise, simply save the provided `index.html` file to your local machine.

2.  **Open in Browser:**
    Open the `index.html` file directly in your web browser (e.g., Chrome, Firefox, Edge). You can do this by double-clicking the file or by dragging it into your browser window.

3.  **Enter Text:**
    Type or paste the text you wish to translate into the "Source Text" area.

4.  **Select Languages:**
    *   Choose the "From" language (default is "Auto-detect").
    *   Choose the "To" language (default is "English").

5.  **Translate:**
    Click the "Translate" button. The translated text will appear in the "Translated Text" area.

6.  **Copy/Play:**
    *   Click the "Copy" button to copy the translated text to your clipboard.
    *   Click the "Play" button to hear the translated text spoken aloud.

## Project Structure


The entire application is contained within a single `index.html` file, which includes both the HTML structure and the JavaScript logic.

## Limitations

*   **API Usage:** This tool uses a publicly accessible Google Translate API endpoint. While generally reliable for personal use, it's not an official or guaranteed stable API for large-scale production applications. For commercial or high-volume usage, an official API key from Google Cloud Translation API (or similar services like Microsoft Translator) would be required.
*   **Error Handling:** Basic error handling is in place for network issues, but more robust error messaging for various API responses could be added.
*   **Styling:** The CSS is embedded directly in the HTML, which is fine for a small project but for larger applications, it's best practice to use external CSS files.
*   **Language List:** The list of supported languages is hardcoded. For a more dynamic application, this could be fetched from an external source or configured more flexibly.
