# Natural Language Processing in Microsoft Azure

[![License](https://img.shields.io/npm/l/react)](https://github.com/JadesonBruno/natural-language-processing-in-azure/blob/main/LICENSE)

This repository has the purpose of storing the project developed within the scope of the "Natural Language Processing" module of the "Microsoft Azure AI Fundamentals" Bootcamp by [DIO](https://www.dio.me/), under the instruction of the teacher [Valéria Baptista](https://www.linkedin.com/in/valeriabaptista/).

The project is an essential requirement for passing the "Natural Language Processin" module, consolidating participants practical learning and preparing them for subsequent challenges.

The development of this project aims to identify Azure AI services that include natural language processing, specifically speech-to-text and sentiment analysis services. For a better understanding, i divided the entire process into steps,from creating resources to the final result of conversion and sentiment analysis.

## Speech-to-Text

### Step 1: Creating  a Resource to Speech-to-Text

Let's start by accessing the following Microsoft portal: https://speech.microsoft.com/portal.

In the [Speech Studio](https://speech.microsoft.com/portal) portal, we will create a new resource.

<p align="center">
  <img src="./assets/01_creating_a_resource.gif" alt="Creating a Resourse">
</p>

You will need to fill in some information to create a speech resource.

<p align="center">
  <img src="./assets/02_configuring_a_resource.png" alt="Configuring a Resourse">
</p>

We will use the created resource to start our work.

<p align="center">
  <img src="./assets/03_use_resource.png" alt="Use Resourse">
</p>

### Step 2: Selecting Real-time speech to text

In the Speech to text category we will select Real-time speech to text.

<p align="center">
  <img src="./assets/04_real_time_speech_to_text.gif" alt="Real-time speech to text">
</p>

### Step 3: Speech to text conversion

It is important to configure the language of the audio that will be loaded. After that, we will select our file in the directory corresponding to our desktop and have our speech converted into text.

For the laboratory i chose a biblical excerpt in English. 

Used audio: [01_mattew_11_28_30.mp3](./inputs/01_mattew_11_28_30.mp3).

<p align="center">
  <img src="./assets/05_result_of_converting_speech_to_text.png" alt="Result of converting speech to text">
</p>

Result in text: Matthew Chapter 11 verses 28 to 30 Come to me all you who labor and are heavy laden and I will give you rest. Take my yoke upon you and learn from me, for I am gentle and lowly in heart. And you will find rest for your souls. For my yoke is easy and my burden is light. 

The result in json format can be seen here: [01_result_of_converting_speech_to_text.json](./outputs/01_result_of_converting_speech_to_text.json).

### Step 4: Next Steps

We can use the Real-time speech to text service to integrate it with different programming languages to create personalized applications that use this feature.

## Sentiment Analysis

### Step 1: Creating a resource to sentiment analysis

First, let's access the [Microsoft Azure](https://portal.azure.com/#home) portal.

Let's create a resource and configure it.

<p align="center">
  <img src="./assets/06_creating_a_resource_to_sentiment_analysis.gif" alt="Creating a resource for sentiment analysis">
</p>

Now, let's configure the resource.

<p align="center">
  <img src="./assets/07_configuring_resource_to_sentiment_analysis.png" alt="Configuring resource for sentiment analysis">
</p>

<p align="center">
  <img src="./assets/08_create.png" alt="Create">
</p>

By going to the resource group, we can confirm the deployment.

<p align="center">
  <img src="./assets/09_go_to_resource_group.png" alt="Create">
</p>

<p align="center">
  <img src="./assets/10_resource_created.png" alt="Resource created">
</p>

## Step 2: Select an Azure resource

After completing this creation stage, we go to the [Language Cognitive](https://language.cognitive.azure.com/) portal.

To access Language Studio we need to link it with an Azure resource.

<p align="center">
  <img src="./assets/11_select_an_azure_resource.png" alt="Select an Azure resource">
</p>

### Step 3: Selecting analyze sentiment and mine opinions

To perform sentiment analysis in Azure we can select "Selecting analyze sentiment and mine opinions".

<p align="center">
  <img src="./assets/12_selecting_analyze_sentiment_and_mine_opinions.gif" alt="Select analyze sentiment and mine opnions">
</p>

By selecting the text from our directory to perform sentiment analysis, we will be able to obtain the results.

Text file used: [02_review_of_the_royal_hotel.txt](./inputs/02_review_of_the_royal_hotel.txt).

<p align="center">
  <img src="./assets/13_run_sentiment_analysis.png" alt="Run sentiment analysis">
</p>

### Step 4: Examining the results

**Sentence 1:**

<p align="center">
  <img src="./assets/14_sentence_01.png" alt="Sentence 01">
</p>

**Sentence 2:**

<p align="center">
  <img src="./assets/15_sentence_02.png" alt="Sentence 01">
</p>

**Sentence 3:**

<p align="center">
  <img src="./assets/16_sentence_03.png" alt="Sentence 01">
</p>

**Original Text:**

<p align="center">
  <img src="./assets/17_original_text.png" alt="Sentence 01">
</p>

Analyzing the results we realized that sentiment analysis is classified into three variables: positive, neutral and negative. **Positive** denotes positive feelings such as "happy", "great", "lovely", among others. **Neutral** refers to neutral and objective statements that do not express a strong emotional opinion. **Negative** denotes the presence of words with negative feelings, such as "sad", "bad", "frustrating", among others.

In our text, we noticed the customer's frustration with the hotel, and this will lead our sentiment analysis to a higher percentage in Negative.

The result in json format can be seen here: [02_sentiment_analysis.json](./outputs/02_sentiment_analysis.json).

### Step 5: Next Steps

We can use the "Analyze sentiment and mine opinions" service to integrate it with different programming languages to create personalized applications that use this feature.

## Useful Links:

[Explore Speech Studio](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/09-speech.html)

[Analyze text with Language Studio](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/06-text-analysis.html)


## Tecnologias Utilizadas

- Microsoft Azure AI Speech Studio
- Microsoft Azure AI Language Studio

## Contributions

Contributions are welcome. Feel free to suggest improvements and possible fixes to the code through an issue or pull requests.

## Author

Jadeson Bruno Albuquerque da Silva

[![Linkedin](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jadeson-silva/)