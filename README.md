# Whatdialectla

Introduction of Project 

What Dialect La has two main objectives, using GPT-4, we are looking to classify dialects based on written text and to regenerate sentences in one dialect into another dialect. While english is a universal language, there are regional dialects that are tied to the specific cultures for each region. By understanding who might be typing something, we are able to tailor responses that are most reseptive to people of that culture and to ensure we do not tap on anything that may be taboo within that culture. By regenerating sentences from one dialect to another, people will have a tool to understand the nuances in other cultures to assist them with getting assimilated into their new culture. 


Data Processing 

We got the datasets from online street interviews and picking out specific sentences that we thought were unique and might be telling of the dialect. Some of the sentences were very obviously of a certain dialect while other sentences are more vague and can share vocabulary and sentence structures with other dialects. 

We collected 30 sentences from 6 different dialects and 30 sentences that we felt were more neutral in nature.

The first 10 sentences are normally sentences with unique vocabulary and are sentences that should be easiest to classify. The next 10 sentences are formed with mostly only sentence structure differences, using common english vocabuary. The last 10 sentences are mixed and reserved for testing the classifier if we do not want to expose it to anything else. 
 

Architecture  

For the classifier, the context prompt tells GPT-4 to be a classifier and the kinds of labels that are available. The sentence that we want GPT-4 to classify is the input prompt and GPT-4 will provide the classification label. 

The context prompting will have 3 variants and we will test the effectiveness of each of these prompting styles: Zero-Shot, Single-Shot and Single-Shot with Chain of Thought Prompting. 

For the generator, the context prompt tells GPT-4 to translate a specific dialect to another specific dialect. The sentence that we want GPT-4 to translate is the input prompt and GPT-4 will provide the translated sentance. 

We will likely test the initial generations on how well it can generate in any given dialects. Unfortunately, Jashwant and Yi Da are only fluent in some dialects and we will be serverely limiting the dialects we choose to test. 
 

Model effectiveness gauge 

To test the effectiveness of the classifier, we will let GPT-4 process the datasets and provide the labels. We will test the accuracy of the output with our own labels and determine the accuracy. For the comparison, we will compare the system to the zero-shot prompt as the baseline to determine how much we have succeeded. 

To test the generator, GPT-4 will take in the prompt and provide the translated sentence. Jashwant and Yi Da will assess how well the sentence has been translated using mean opinion score (1 to 5, base score is 1).  

The generator would have succeeded if we got a rating of at least 4.3, or if it has improved it from the zero-shot variant. 
