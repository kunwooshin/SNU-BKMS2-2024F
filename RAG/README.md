# BKMS2 Hands-on #4: Developing a Q&A system based on RAG
- **Instructor**: Prof. Sang-Won Lee (swlee69@snu.ac.kr)
- **TA**:         snu.vldb.ta@gmail.com

## Overview


<p align="center">
  <img width="70%" src="https://github.com/user-attachments/assets/a590a8c9-9a95-4bc2-89e4-26c049028e75">
</p>

To ensure consistency in the Python module dependencies for this hands-on exercise, we will be using **Google Colab**.

1. **Download the notebook**: Download the `BKMS2_hands_on_4.ipynb` file from this repository.
2. **Open in Colab**: Upload and open the notebook in Google Colab.


## Setup

1. **Download `data.zip`**: Please download the `data.zip` file and upload it to your Google Colab environment.
2. **Unzip the file**: Unzip the data by running the following command in Colab:

    ```bash
    !unzip /content/data.zip -d /content
    ```

3. **Install dependencies**: Install the required Python packages listed in the `requirements.txt` file:

    ```bash
    !pip install -r /content/data/requirements.txt
    ```

4. **Set up OpenAI API key**: To run the generation part, you'll need to set your OpenAI API key. Use the following code to securely enter your key:

    ```python
    from getpass import getpass

    # Enter your OpenAI API key
    OPENAI_API_KEY = getpass("Please enter your OpenAI API key: ")
    ```

## Table of Contents for BKMS2 Hands-on #4

### Colab Setup
Before starting, make sure to set up the environment by downloading the necessary data and installing dependencies. All the steps can be executed within Google Colab.

### Basic Implementation
1-1. **Load and Split the Document**: Load the source document and split it into manageable chunks for processing.  
1-2. **Store in a Vector Database**: Store the document chunks in a vector database (e.g., ChromaDB) for efficient retrieval.  
1-3. **Retrieval, Augmentation and Generation (RAG)**: Perform document retrieval and generate a response using OpenAI's API, combining retrieved data with a generative model.  
1-4. **Various Distance Metrics for Semantic Search**: Explore different distance metrics (e.g., cosine, Euclidean) to improve the semantic search performance.

### Implementing RAG with Langchain
2-1. **Load and Store Data from URL**: Fetch and store data from a URL for RAG processing.  
2-2. **Load and Store Data from TXT**: Load data from a local text file and store it in the vector database.  
2-3. **Retrieval, Augmentation and Generation (RAG)**: Repeat the RAG process using Langchain to retrieve and generate context-aware answers.  
2-4. **Prototype for Chatbot**: Develop a basic chatbot prototype that integrates retrieval and generation to answer user queries based on the stored data.

## References
