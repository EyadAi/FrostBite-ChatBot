# FrostBite Chatbot

FrostBite is a simple and lightweight chatbot designed for casual conversations. It uses natural language processing (NLP) and a neural network model to understand and respond to user inputs. Whether you're looking for a quick chat, a joke, or just someone to talk to, FrostBite is here to help!

---

## Overview

FrostBite is built using Python and leverages libraries like **TensorFlow**, **Keras**, and **NLTK** for natural language understanding. The chatbot is trained on a set of predefined intents (stored in `intents.json`), which include common conversational topics like greetings, jokes, hobbies, and more. FrostBite is perfect for casual interactions and can be easily integrated into your projects.

---

## Features

- **Natural Language Processing**: FrostBite uses NLTK for tokenization and lemmatization to understand user inputs.
- **Neural Network Model**: A simple deep learning model powers FrostBite's ability to classify user inputs and generate appropriate responses.
- **Customizable Intents**: The chatbot's behavior can be easily customized by modifying the `intents.json` file.
- **Gradio Interface**: FrostBite comes with a user-friendly web interface powered by Gradio, making it easy to interact with the chatbot.

---

## Getting Started

### Prerequisites

To run FrostBite, you'll need the following Python libraries installed:

- TensorFlow
- Keras
- NLTK
- NumPy
- Gradio

You can install the dependencies using `pip`:

## Installation
### Clone the repository:

```Bash
git clone https://github.com/EyadAi/FrostBite.git

```
### Navigate to the project directory:

```Bash
cd FrostBite

```

### Run the chatbot:

```Bash
python ChatBotModel.ipynb

```
## Usage
Once FrostBite is running, you can interact with it through the Gradio interface. Simply type your message, and FrostBite will respond!

## Example Interactions

```Bash
You: "Hi"
FrostBite: "Hello! I'm FrostBite, nice to meet you!"

You: "Tell me a joke"
FrostBite: "Why don't scientists trust atoms? Because they make up everything!"

You: "What's your favorite food?"
FrostBite: "FrostBite doesn’t eat, but I love hearing about your favorite foods!"

```

## Customizing FrostBite
You can customize FrostBite's behavior by editing the intents.json file. Add new patterns, responses, or tags to make the chatbot more tailored to your needs.

## Example: 
### Adding a New Intent
```json
{
  "tag": "new_intent",
  "patterns": ["What's your favorite color?", "Do you like colors?", "Tell me about colors"],
  "responses": ["FrostBite loves all colors, but blue is my favorite!", "Colors are amazing! FrostBite likes them all!"],
  "context_set": ""
}

```
### Running the Gradio Interface
FrostBite comes with a Gradio interface for easy interaction. To launch it, run the following code in your Python environment:

```python
import gradio as gr

iface = gr.Interface(
    inputs=gr.Textbox(lines=2, placeholder="Enter your message here..."),
    fn=predict_tag,
    outputs="text",
    title="FrostBite Chatbot",
    description="Interact with the chatbot and ask your questions.",
)

iface.launch()
```
## License
This project is licensed under the Apache 2.0 License. See the [LICENSE](https://github.com/EyadAi/FrostBiteChatBot/blob/main/LICENSE) file for details.

Enjoy chatting with FrostBite! 🎉
