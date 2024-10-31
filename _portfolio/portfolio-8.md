---
title: "CS 5302: Generative AI for Natural Language and Speech Processing"
excerpt: "This project, part of CS 5302: Generative AI for Natural Language and Speech Processing, an application that can interpret, translate, and vocalize spoken language in real-time, and is specifically catered for patient-doctor conversations"
time_period: "Spring 2023"
collection: portfolio
---

As part of a research project for CS 5302: Generative AI for Natural Language and Speech Processing, we aimed to develop an application that can interpret, translate, and vocalize spoken language in real-time, and is specifically catered for patient-doctor conversations. The application is dubbed as a Speech to Machine Translation + Speech (SMTS) system. This system can potentially help overcome language barriers in healthcare, facilitating clear communication and thereby improving the quality of patient care and outcomes. Our system is built upon four key components:

1. **Speech Recognition**: This is the first step where the system listens to the spoken words (e.g., a patient's symptoms) and *transcribes* them into English for easier processing.
2. **Large Language Model (LLM) + Retrieval Augmented Generation (RAG)**: The English text is then fed into a pre-trained LLM to fetch accurate and contextually appropriate responses (e.g., the diagnosis of the patient) from a set of curated medical documents.
3. **Machine Translation**: Once the diagnosis has been done, the system then translates the text into the desired language (which can be different from the patient's language).
4. **Text-to-Speech Synthesis**: The translated text is finally converted back into speech in the translated language.

The details of our idea, methodology, results etc can be found [here](https://drive.google.com/drive/folders/13qdQP7t7Sx0urabw9OtLoRGnuB75b3C1?usp=sharing) while our github can found [here](https://github.com/CS-5302/CS-5302-Project-Group-15)
