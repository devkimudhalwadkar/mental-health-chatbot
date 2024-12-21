# Chatbot Using Deep Learning and Flask

This is a Python-based, web-based chatbot project that uses **deep learning** and **Flask** to interact with users. The chatbot is trained on a dataset containing categories (intents), patterns, and responses. It utilizes a special **artificial neural network (ANN)** to classify the user's message into a category and generate a random response from a list of predefined responses.

### Features

- **Dataset**: The chatbot is trained on a `data.json` file, which contains patterns to match against user input and corresponding responses.
- **Deep Learning Model**: Uses **Keras** to build and train a neural network model to classify user inputs into categories.
- **Web Interface**: A Flask-based web interface allows users to interact with the chatbot.
- **Natural Language Processing (NLP)**: **NLTK** is used for tokenizing and preprocessing text data.

### Project Structure

- **`data.json`**: This file contains predefined patterns and responses for various categories (intents).
- **`training.py`**: Script to build and train the deep learning model using the dataset.
- **`texts.pkl`**: Pickle file containing a list of vocabulary words extracted from the dataset using **NLTK**.
- **`labels.pkl`**: Pickle file containing the list of categories (labels) that the chatbot can recognize.
- **`model.h5`**: The trained Keras model, including weights and information about the neural network.
- **`app.py`**: The Flask web app script to serve the chatbot through a graphical user interface.

### Steps to Create the Chatbot

1. **Import and Load the Data**: Load the `data.json` file containing patterns and responses.
2. **Preprocess the Data**: Tokenize and preprocess the text using **NLTK** to prepare it for training.
3. **Split Data**: Split the data into training and test sets.
4. **Build the ANN Model**: Use **Keras** to build a neural network model for classification.
5. **Predict Outcomes**: Load the trained model and use it to predict the class of user input.
6. **Deploy in Flask App**: Integrate the trained model into a Flask app and deploy it with a web-based interface.

### How to Run the Chatbot

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/chatbot-flask.git
    cd chatbot-flask
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Train the model (if not already trained):
    ```bash
    python training.py
    ```

4. Start the Flask application:
    ```bash
    python app.py
    ```

5. Open your browser and navigate to `http://127.0.0.1:5000/` to start chatting with the bot!

### Technologies Used

- **Flask**: Web framework for serving the chatbot.
- **Keras**: Deep learning framework used to build and train the neural network.
- **NLTK**: Natural Language Toolkit for processing text data.
- **Python**: Programming language used for building the chatbot and backend functionality.

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

### Acknowledgments

- Thanks to the open-source community for providing the tools and libraries used in this project.
- **Keras**, **Flask**, and **NLTK** are essential tools that enabled the creation of this chatbot.

---

Feel free to modify the code, improve the bot's responses, and enhance its capabilities. Happy coding!

