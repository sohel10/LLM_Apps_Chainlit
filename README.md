# LLM_Apps_Chainlit

This repository contains a **Chainlit** demo application that demonstrates how to build LLM (Large Language Model) apps quickly, similar to Streamlit. Chainlit allows you to easily create and deploy apps that use LLMs.

## Overview

The **LLM_Apps_Chainlit** application showcases how to integrate Chainlit with custom logic, such as querying a language model and responding to user input. The app is designed to handle conversational interactions where users input text, and the system provides relevant responses based on the input using the `ask_order` function.

## Features

- **LLM Integration**: Uses the `ask_order` function to query the language model.
- **Interactive User Interface**: The app allows users to input text and receive responses.
- **Chainlit Framework**: Uses Chainlit to develop and deploy the app easily.

## Prerequisites

- **Python 3.7+**
- **Pip**
- **Chainlit** package

## Installation

1. **Clone the repository**:

    ```bash
    git clone https://github.com/LLM_Apps_Chainlit.git
    cd LLM_Apps_Chainlit
    ```

2. **Create a virtual environment** (optional but recommended):

    ```bash
    python -m venv llm_chainlit_env
    source llm_chainlit_env/bin/activate  # For Windows: `llm_chainlit_env\Scripts\activate`
    ```

3. **Install the dependencies**:

    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. **Initialize Chainlit**:

    ```bash
    chainlit init
    ```

2. **Run the Chainlit app**:

    ```bash
    chainlit run app.py
    ```

3. **Open the app**:

   After running the above command, the app will be accessible at `http://localhost:8000` on your local machine.

### How It Works

- **Message Handling**: The app listens for incoming user messages and responds using the `ask_order` function from the `llm.py` module.
- **User Interaction**: Users can enter any query, and the system will respond by using the language model to generate contextually relevant answers.

## Project Structure

```bash
.
├── app.py                # Main application script
├── src/
│   └── llm.py            # LLM logic (ask_order function)
├── requirements.txt      # Python dependencies
└── README.md             # This readme file
