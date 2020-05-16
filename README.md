# sarcasm-detection
**Natural Language Processing to detect whether news are sarcastic or not**

The same has been achieved using two engines.
1. Linear SVR 
2. ANN

Before we train any model on the data we need to pre-process the data. 

**Pre-processing of the data includes following steps.**
1. Removing the punchuations. 
2. Converting all upper case letters to lower case.
3. Stemming of words. 
4. Removing unwanted words(The, of, is, and etc ). 
5. Word Tokenization

Each of the above process is eloborated in the section below. 

**Removing the punchuations.**

We often see punchuations used in new, But this punctuations are do not hold importance as compared to the actual words in the sentence so we remove this punchuations in order to avoid unnecessary computation. 

**Converting all upper case letters to lower case.**

In this process we cnvert the upper case letters to lower cases. This opertation is performed so that our model does not consider "London" and "london" differently or may be for instance "BEAUTIFUL" and "beautiful" as two different words. 

**Stemming of words.**

It is used to find the root of a particular word. Say for instance "Strong" this word can be used in sentence in various forms like "Stronger" or "Strongest". Again in order to reduce the unecerry operations we can covert all this words into their base form which is "Strong" 

**Removing unwanted words(The, of, is, and etc ). **

The meaning of the sentence can be fairly unstood by the main words of the sentence which are essentially the crux if the sentence. this can be illustrated by the example below. 
Before:  Taj mahal is beautiful place
After:   Taj mahal beauty place
The words like "Is", "and", "The" are unecessay during understanding the essence of a sentence thus can be ignored. 

**Word Tokenization**

In this step we give every word in dataset a token. Thus whenever a sentence has perticuler word the respective cell is set. 

