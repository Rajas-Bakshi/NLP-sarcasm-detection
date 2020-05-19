# sarcasm-detection
**Natural Language Processing to detect whether news are sarcastic or not**

We have used Artificial Neural Network to predict the outcome. 

Before we train any model on the data we need to pre-process the data. 

**Pre-processing of the data includes following steps.**
1. Removing the punctuations. 
2. Converting all upper case letters to lower case.
3. Stemming of words. 
4. Removing unwanted words(The, of, is, and etc ). 
5. Word Tokenization

Each of the above process is elaborated in the section below. 

**Removing the punctuations.**

We often see punctuations used in new, But this punctuations are do not hold importance as compared to the actual words in the sentence so we remove this punchuations in order to avoid unnecessary computation. 

**Converting all upper case letters to lower case.**

In this process we convert the upper case letters to lower cases. This operation is performed so that our model does not consider "London" and "london" differently or may be for instance "BEAUTIFUL" and "beautiful" as two different words. 

**Stemming of words.**

It is used to find the root of a particular word. Say for instance "Strong" this word can be used in sentence in various forms like "Stronger" or "Strongest". Again in order to reduce the unnecessary operations we can covert all this words into their base form which is "Strong" 

**Removing unwanted words(The, of, is, and etc ).**

The meaning of the sentence can be fairly understood by the main words of the sentence which are essentially the crux if the sentence. this can be illustrated by the example below. 
Before:  Taj mahal is beautiful place
After:   Taj mahal beauty place
The words like "Is", "and", "The" are unnecessary during understanding the essence of a sentence thus can be ignored. 

**Word Tokenization.**

In this step we give every word in dataset a token. Thus whenever a sentence has particular word the respective cell is set.


Finally we use Artificial Neural Networks to predict the output as shown above.

The ANN used is three layers deep.
1. First layer is of 28 neurons with Rectifier activation function. 
2. First layer is of 4 neurons with Rectifier activation function.
3. The final layer is of 1 neuron with sigmoid activation function.   

The training accuracy of the model is 86% and the testing accuracy is 80%
