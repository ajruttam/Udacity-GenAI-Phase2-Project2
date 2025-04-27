# Udacity-GenAI-Phase2-Project2

**Build Your Own Custom Chatbot**

The main objective of this project is to build a customized chatbot capable of answering questions using a customized database. That is, a data set that was not used during model training.

## Rubrics

### 1. Choose a Dataset and Explain the Scenario

In this project, I choose `2023_fashion_trends.csv` as my dataset provided in the data folder of this module. I am using it because the model I will be using is `gpt-3.5-turbo-instruct` which was trained till 2021 and it might not know about the 2023 fashion trends.

To improve the question answering capability of our tool, we employ the Retrieval Augmented Generation technique. This technique complements the prompt with contextual information from the dataset, allowing the model to provide more accurate and relevant answers to the questions posed to it.

### 2. Prepare the Dataset for the Custom Query Process

The chosen dataset was loaded into a `pandas` dataframe with a column called "text". This column should contain all of your text data, separated into at least 20 lines and then transformed into a DataFrame so that embeddings could be created in the next step. The objective of this was to demonstrate the correct functioning of the project, since OpenAI's GPT-3.5-instruct has information until 2021.

### 3. Perform the Custom Query Process

To perform the customized query, embeddings were created using the OpenAI API and saved in the `csv` file. With this, a customized search was carried out with an OpenAI `Completion` Model.

### 4. Write Questions to Demonstrate Custom Performance

To evaluate the results of the developed project, a series of questions were asked, and each was answered both without context and with context.
