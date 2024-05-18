9# chatbot
A Django-based web application integrating a chatbot for interactive and automated user responses.


# Chatbot Integration using Python, Django, and Dialogflow

## Overview
This project integrates a Dialogflow chatbot into a Django web application. The chatbot provides interactive and automated responses to user queries, enhancing the user experience on the website.

## Features
- Natural language processing powered by Dialogflow
- Seamless integration with Django framework
- Interactive and automated responses
- Easy to extend and customize

## Requirements
- Python 3.9
- Django 4.x
- Dialogflow API client library for Python
- Google Cloud account with Dialogflow enabled

## Installation
1. **Clone the repository:**
    ```sh
    git clone https://github.com/yourusername/your-repo-name.git
    cd your-repo-name
    ```

2. **Create a virtual environment and activate it:**
    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install the required packages:**
    ```sh
    pip install -r requirements.txt
    ```

4. **Set up Dialogflow:**
    - Create a Dialogflow agent on the Dialogflow console.
    - Download the service account key JSON file from Google Cloud.
    - Set the environment variable for the service account key:
      ```sh
      export GOOGLE_APPLICATION_CREDENTIALS="/path/to/your/service-account-file.json"
      ```

5. **Configure Django settings:**
    - Add your Dialogflow project ID and other settings in `settings.py`:
      ```python
      DIALOGFLOW_PROJECT_ID = 'your-dialogflow-project-id'
      ```

## Usage
1. **Run the Django development server:**
    ```sh
    python manage.py runserver
    ```

2. **Access the chatbot:**
    - Open your web browser and go to `http://127.0.0.1:8000/chatbot/`.
    - Interact with the chatbot by typing messages into the chat interface.

## Project Structure
- `chatbot/`: Contains the Django app for the chatbot.
- `templates/`: HTML templates for rendering the chat interface.
- `static/`: Static files (CSS, JavaScript) for the chatbot UI.
- `requirements.txt`: Lists the Python dependencies for the project.
- `manage.py`: Django's command-line utility for administrative tasks.

## Customization
- **Dialogflow Intents and Entities:**
  - Customize the intents and entities in your Dialogflow agent to handle different types of user queries.
  
- **Django Views and URLs:**
  - Modify the views and URLs in the `chatbot` app to change the behavior and routing of the chatbot.

- **Frontend UI:**
  - Edit the HTML, CSS, and JavaScript files in the `templates` and `static` directories to customize the chat interface.

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any changes or improvements.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgements
- [Dialogflow](https://dialogflow.cloud.google.com/) for the powerful NLP capabilities.
- [Django](https://www.djangoproject.com/) for the robust web framework.

