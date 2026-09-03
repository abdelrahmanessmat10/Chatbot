# Chatbot Project

A simple and interactive React-based Chatbot user interface. This project demonstrates how to build a basic chat application using React and Babel standalone to compile JSX directly in the browser.

## 📁 Project Structure

The project code is modularized into styles and components for better maintainability:

- `index.html`: The main entry point of the application.
- **`styles/`**: Contains modular CSS files:
  - `general.css`: Base layout and body styles.
  - `chat-input.css`: Styling for the message input area and send button.
  - `chat-message.css`: Styling for chat bubbles and user/robot message alignment.
- **`scripts/`**: Contains React components:
  - `App.js`: The main application container holding the state.
  - `ChatMessages.js`: Component that renders the list of messages and auto-scrolls to the newest message.
  - `ChatMessage.js`: Component for an individual chat bubble.
  - `ChatInput.js`: Component for the text input and sending logic.
  - `index.js`: The React entry script that renders the App to the DOM.

## 🚀 How to Run Locally

Because the JavaScript files are separated and loaded dynamically by Babel via HTTP, opening `index.html` directly from your file system (as `file:///...`) will result in a **CORS error**. 

To run the project, you need to serve it via a local HTTP server:

1. **Option 1: Using VS Code**
   - Install the **Live Server** extension.
   - Right-click on `index.html` and select **"Open with Live Server"**.

2. **Option 2: Using Node.js (npx)**
   - Open your terminal in the project directory.
   - Run the following command:
     ```bash
     npx serve .
     ```
   - Open your browser and navigate to the local link provided (usually `http://localhost:3000`).

3. **Option 3: Using Python**
   - Open your terminal in the project directory.
   - Run the following command:
     ```bash
     python -m http.server
     ```
   - Open your browser and navigate to `http://localhost:8000`.

## 🛠️ Technologies Used
- HTML5 & CSS3
- React (via CDN)
- Babel Standalone (for in-browser JSX compilation)
