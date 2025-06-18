# ChatBot Project

Welcome to the ChatBot project! This is a Flask-based chatbot application designed to assist users with a wide range of queries related to a college, including admissions, courses, fees, campus life, internships, and more. The chatbot leverages Natural Language Processing (NLP) techniques to interpret user inputs and provide relevant responses, making it an interactive and helpful tool for prospective students and current attendees.

## Project Overview

This project is a web-based chatbot built using Python and Flask, with a focus on providing information about Dr. D.Y. Patil Technical University (DYP-ATU). It uses NLP libraries like NLTK for text preprocessing and Scikit-learn for intent recognition based on cosine similarity. The chatbot supports both a web interface and a console-based interaction mode, offering flexibility in how users can engage with it.

## Project Structure

```
CHATBOT/
│
├── static/
│   └── ima2.jpeg              # Static image file for the web interface
│
├── templates/
│   └── index.html             # HTML template for the chatbot web interface
│
├── venv/                      # Virtual environment for Python dependencies
│
├── .gitignore                 # Git ignore file to exclude temporary files
├── name                       # Project name file (optional)
├── app.py                     # Flask application entry point
├── chatBot.iml                # IntelliJ IDEA project configuration
├── chatbot.py                 # Console-based chatbot script
├── intents.py                 # Dictionary of intents and responses
├── misc.xml                   # Miscellaneous configuration file
├── modules.xml                # Module configuration file
├── preprocess.py              # Text preprocessing script using NLTK
├── profiles_settings.xml      # Profile settings configuration
├── requirements.txt           # List of Python dependencies
├── similarity.py              # Intent recognition using TF-IDF and cosine similarity
├── Technologies Used.pdf      # Documentation of technologies and NLP techniques
└── workspace.xml              # Workspace configuration file
```

### Directory Description
- `static/`: Stores static assets like images used in the web interface.
- `templates/`: Contains HTML templates rendered by Flask for the web UI.
- `venv/`: Holds the virtual environment for isolating project dependencies.
- Root files: Include the main application logic, configuration files, and supporting documentation.

## Technologies Used

### Backend
- **Flask**: A lightweight Python web framework that powers the backend, handling HTTP requests and responses.
- **Python**: The primary programming language for the project.

### Frontend
- **HTML**: Structures the chatbot's web interface, including the chat window and input fields.
- **CSS/Bootstrap**: Styles the UI with a responsive design, utilizing Bootstrap for pre-built components like cards.
- **JavaScript/jQuery**: Manages client-side interactivity, including sending user inputs to the backend and updating the chat display.

### NLP and Machine Learning
- **NLTK (Natural Language Toolkit)**: Used for tokenization and lemmatization to preprocess user input, enhancing intent recognition.
- **Scikit-learn**: Implements TF-IDF vectorization and cosine similarity to match user queries to predefined intents.
- **JSON**: Facilitates data exchange between the frontend and backend in a structured format.

### Additional Tools
- **Git**: Version control for managing the project codebase.
- **Virtualenv**: Ensures dependency isolation for a clean development environment.

## Features

- **Intent Recognition**: Identifies user intents (e.g., "What courses are offered?") using cosine similarity on TF-IDF vectors.
- **Response Generation**: Provides tailored responses based on recognized intents from the `intents.py` file.
- **Web Interface**: Allows users to interact with the chatbot via a browser at `http://localhost:5000`.
- **Console Mode**: Offers a command-line interface for testing and development.
- **Multi-Topic Support**: Covers admissions, courses (Engineering, BCA, MCA, Agriculture), fees, campus life, and more.

## Screenshots

Add images to showcase the chatbot interface and features.

- **Chatbot Web Interface (Initial View)**:
  ![Chatbot Initial Interface](https://raw.githubusercontent.com/hriturajnarvekar27/Chatbot/main/Screenshot%202025-06-18%20145329.png)
  *Description*: The initial view of the chatbot web interface showing the greeting message.

- **Chatbot Web Interface (Response View)**:
  ![Chatbot Response Interface](https://raw.githubusercontent.com/hriturajnarvekar27/Chatbot/main/Screenshot%202025-06-18%20145353.png)
  *Description*: The chatbot interface displaying a response to a user query.

## Installation

### Prerequisites
- Python 3.x
- pip (Python package manager)
- Git (for cloning the repository)

### Steps
1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   cd CHATBOT
   ```

2. **Set Up Virtual Environment**:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
   Ensure `requirements.txt` includes: `flask`, `nltk`, `scikit-learn`, and other necessary packages.

4. **Run the Application**:
   ```bash
   python app.py
   ```

5. **Access the Chatbot**:
   Open a web browser and navigate to `http://localhost:5000` to use the web interface, or run `python chatbot.py` for console mode.

## Usage

- **Web Interface**: Type your query in the input field and press "Send" to receive a response. The chat history updates dynamically.
- **Console Mode**: Start the script with `python chatbot.py`, type your query, and type 'exit' to end the session.
- **Supported Queries**: Ask about college courses, admission processes, fees, hostel details, campus facilities, etc. Examples include:
  - "What is the application deadline?"
  - "What engineering departments are available?"
  - "Is there a gym on campus?"

## Development and Contributing

### How to Contribute
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit them (`git commit -m "Add new feature"`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a pull request with a clear description of your changes.

### Issues and Bugs
Report any issues or suggest enhancements by opening an issue on the repository.

## Acknowledgments

- Thanks to the open-source communities behind Flask, NLTK, Scikit-learn, and Bootstrap.
- Special thanks to Dr. D.Y. Patil Technical University for the context and inspiration.

## Contact

For questions or support, please reach out via the repository's issue tracker or [your email/contact info].

*Last updated: June 18, 2025*
