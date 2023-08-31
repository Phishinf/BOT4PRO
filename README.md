# TECHNICAL DISCUSSION - BOT4PRO
This is a technical communication for all issues of the different stages of development cycle amongst team members  
Before going to the project, we can use gist to share either in Gist or Colab and comment on the code

## Gist
This is a template that you can use to share [the code](https://gist.github.com/AIBIZAPP/90126e343741c4ab4dfbc78f0494e7fc)  

## Colab Test Ground
All codes can run on the Colab environment [template notebook](https://github.com/AIBIZAPP/BOT4PRO/blob/main/Templatenotebook.ipynb)

## Image
![Dale-E](https://user-images.githubusercontent.com/134267717/261605015-1cba70f5-54cc-4845-abd6-e030711ecfa9.png)

## Proof of Concept on GENERATIVE AI
* To get the machine to understand the customer-specific needs (question attributes x11, x12, ..., xN1, xN2, ..., XNn) from their question prompts (X1, X2, ... XN)
* To able let the machine relate the customer-specific needs with (the document attributes y11, y12, ..., yM1, yM2, ..., yMm) document (Y1, Y2, ...,YM)
* To calculate the "score correlation" of (xi1, xi2, ... , ) and (yj1, yj2, ...) i =1,2,...500, j = 1,2,...Number of documents
* To answer the specific need of the machine in human language to the customer 

### Step 1: Understand the NEED
* To digest the different groups of words or numerics that represent the specific needs from the prompt questions
* To base on the limited number of prompt questions to generate an additional number of questions (at least 1000 valid questions, at least 200 invalid questions) without losing the meaning

[Question_generation_via_GPT](https://github.com/AIBIZAPP/BOT4PRO/blob/main/question_generation_via_GPT.ipynb)

* The generated questions are evaluated by the human feedback

* From all questions, we find the "attributes" xi1, xi2, xi3, ... of question i (i=1,2,...,500)

[Generate_key_info_GPT3.5(txt&doc) for reference](https://github.com/AIBIZAPP/BOT4PRO/blob/main/Generate_key_info_GPT3.5(txt%26doc).ipynb)

### Step 2: Understand the documents
* First form a sample of attributes yi1, yi2, ... for document i from a selected document summaries Y1, Y2, ... (level 2, abridged one)
* From the sample attributes yi1, yi2, ... of selected document summaries Y1, Y2, ..., Train the machine using LLM model by fine-tuning to complete sort out attributes of each document summary.
![HuggingFaceEndtoEnd](https://user-images.githubusercontent.com/134267717/262072944-b244daed-23c5-4653-9dd4-9d2dd3f64004.png)

One can reference the [fine-tuning model](https://github.com/AIBIZAPP/BOT4PRO/blob/main/Fine_tune_generative_ai_model.ipynb)  

### Step 3: Calculate the SCORE of the question prompt and documents (HEAT Diagram)

## Answer the question in human language
* Remark: Use the initial set of a limited number of questions to create a diverse set of related questions. Here's a high-level approach you could consider:

####  Point to Focus
Analyze the 60 Questions: Understand the patterns, structures, and common themes in the original 60 questions. 

This will help you identify the key elements that need to be preserved in the new questions.

Paraphrasing: Use paraphrasing techniques to rephrase the original questions while maintaining their underlying meaning. This involves changing the wording, sentence structure, or using synonyms to convey the same ideas.

Data Augmentation: Apply data augmentation strategies, such as replacing nouns, verbs, or other parts of speech with their synonyms, altering the order of clauses, or modifying tense

Restructuring and Combination: Combining elements from multiple original questions to create new questions is not recommended. For example, if you have questions about "cats" and questions about "dogs," you could combine aspects of both to generate questions about "pets."

Semantic Transformations: Apply semantic transformations like negation, inversion, or conditional phrasing to create variations.

Manual Review and Refinement: After generating the new questions, review them manually to ensure they make sense and maintain the intended meaning. Some questions generated might not be valid or might have unintended changes in meaning.

Accuracy: It's important to note that while these approaches can help you generate a larger set of related questions, achieving exactly 500 questions with the exact same meaning as the original small number of questions is unlikely due to the complexity of language and the potential for nuanced differences in phrasing.

Lastly, remember that generating questions with exact meanings is not always the ultimate goal. A diverse set of related questions that capture different aspects of a topic can be more valuable for learning and exploration.
