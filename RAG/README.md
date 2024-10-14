# BKMS2 Hands-on #4: Developing a Q&A system based on RAG
- **Instructor**: Prof. Sang-Won Lee (swlee69@snu.ac.kr)
- **TA**:         snu.vldb.ta@gmail.com

## Overview
RAG 기본 구조 구현 및 langchain 활용.
데이터사이언스 공지와 웹 url 데이터를 이용한 GSDS용 챗봇 간단 구현

<p align="center">
  <img width="70%" src="https://github.com/user-attachments/assets/a590a8c9-9a95-4bc2-89e4-26c049028e75">
</p>

To ensure consistency in the Python module dependencies for this hands-on exercise, we will be using **Google Colab**.

1. **Download the notebook**: Download the `BKMS2_hands_on_4.ipynb` file from this repository.
2. **Open in Colab**: Upload and open the notebook in Google Colab.

## Requirements
Setup이 잘되는지 실제로 테스트 한 번 해보고 오고 잘 안된다면 조교에게 문의.

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

## References
langchain 관련 문서들..
