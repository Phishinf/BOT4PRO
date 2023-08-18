# TECHNICAL DISCUSSION - BOT4PRO
This is a technical communication for all issues of the different stages on development cycle amongst team members  
Before going to the project, we can use gist to share either in Gist or Colab and comment on code

## Gist
This is a template that you can use it to share [the code](https://gist.github.com/AIBIZAPP/90126e343741c4ab4dfbc78f0494e7fc)  

## Colab Template
This is the [notebook](https://github.com/AIBIZAPP/BOT4PRO/blob/main/Templatenotebook.ipynb) which one can run on colab

## Proof of Concept on GENERATIVE AI
* To get the machine to understand the customer specific needs (question attributes x11, x12, ... , xN1, xN2, ..., XNn) from their question prompts (X1, X2, ... XN)
* To able let the machine to relate the customer specific needs with (the document attributes y11, y12, ..., yM1, yM2, ..., yMm) document (Y1, Y2, ... ,YM)
* To answer the specific need by the machine in human langauage to customer 

### Understand the NEED
* To digest the different groupd of words or numerics represent the specific needs
* To base on the limited number of prompt questions to generata addiitonal number of questions (at least 500 questions)
* To calculate the "correlation" of (xi1, xi2, ... , ) and (yj1, yj2, ...) i =1,2,...500, j = 1,2,...Number of documents
* Remark: use the initial set of limited number questions to create a diverse set of related questions. Here's a high-level approach you could consider:

####  Point to Focus
Analyze the 60 Questions: Understand the patterns, structures, and common themes in the original 60 questions. 

This will help you identify the key elements that need to be preserved in the new questions.

Paraphrasing: Use paraphrasing techniques to rephrase the original questions while maintaining their underlying meaning. This involves changing the wording, sentence structure, or using synonyms to convey the same ideas.

Data Augmentation: Apply data augmentation strategies, such as replacing nouns, verbs, or other parts of speech with their synonyms, altering the order of clauses, or modifying tense

Restructuring and Combination: Combine elements from multiple original questions to create new questions is not recommended. For example, if you have questions about "cats" and questions about "dogs," you could combine aspects of both to generate questions about "pets."

Semantic Transformations: Apply semantic transformations like negation, inversion, or conditional phrasing to create variations.

Manual Review and Refinement: After generating the new questions, review them manually to ensure they make sense and maintain the intended meaning. Some questions generated might not be valid or might have unintended changes in meaning.

Accuracy: It's important to note that while these approaches can help you generate a larger set of related questions, achieving exactly 500 questions with the exact same meaning as the original small number of questions is unlikely due to the complexity of language and the potential for nuanced differences in phrasing.

Lastly, remember that generating questions with exact meaning is not always the ultimate goal. A diverse set of related questions that capture different aspects of a topic can be more valuable for learning and exploration.
