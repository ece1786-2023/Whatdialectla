# Whatdialectla

Introduction of Project 

What Dialect La has two main objectives, using GPT-4, we are looking to classify dialects based on written text and to regenerate sentences in one dialect into another dialect. For a foreign individual moving to a new place, the best way to adapt is by understanding the region’s culture and getting accustomed to its way of life. Language is one significant way to adapt, tailoring responses that are most respectful to people of that culture and ensuring we do not tap into anything that may be taboo within that culture shows significant effort. 


Data Processing 

We obtained the datasets from online street interviews and picked out specific sentences that we thought were telling of the dialect. Some of the sentences were very obviously of a certain dialect while other sentences are vaguer and can share vocabulary and sentence structures with other dialects. We collected 30 sentences from 6 different dialects and 30 sentences that we felt were more neutral.
 

Architecture  

GPT-4 was used to produce the results for both the classifier and the translator

The context prompt tells GPT-4 to be a classifier and the kinds of labels that are available. The sentence that we want GPT-4 to classify is the input prompt and GPT-4 will provide the classification label.

The context prompt tells GPT-4 to translate a specific dialect to another specific dialect. The sentence that we want GPT-4 to translate is the input prompt and GPT-4 will provide the translated sentence
