# Llama2 Chatbot Deep Learning
 Deep Learning expert chatbot built using Llama2, langchain and chainlit and Deep Learning books.

### Data
- Dive Into Deep Learning: https://d2l.ai/d2l-en.pdf
- Deep Learning: http://imlab.postech.ac.kr/dkim/class/csed514_2019s/DeepLearningBook.pdf

## System Requirements

Python 3.9 + requirements.txt

---

## Installation

1. Fork this repository and create a codespace in GitHub or clone it locally.

2. Use your HuggingfaceHub API key (from this [URL](https://huggingface.co/settings/tokens)) in the .env file
   ```
   HUGGINGFACEHUB_API_TOKEN=your_huggingface_api_token
   ```
   
3. Create a virtualenv and activate it
   ```
   conda create -n llama2chainlit python=3.9

   conda activate llama2chainlit
   ```

4. Run the following command in the terminal to install necessary python packages:
   ```
   pip install -r requirements.txt
   ```

5. Run the following command in your terminal to create the embeddings and store it locally:
   ```
   python run ingest.py
   ```

6. Run the following command in your terminal to run the app UI:
   ```
   chainlit run main.py -w
