# Number Name Grammar 

## What is this project?
Converting numbers to its proper names in one language (e.g. 23 - twenty three) is an important task in speech technology. Currently there are three major approaches: the rule-based system, the neural models and the Finite State Transducers (FSTs). This project is to exploring a hybrid method of rule-based system and neural models that is inspired by how humans learn to count numbers. 

An adult learner can derive the number grammar of a new language based on a very few words, such as the name for 1 to 20, the names for the tens and the names for big numbers. The human learning mechanism is simplified as decompose the number into a mathematical equation (e.g. 4876 = 4* 1000 + 8* 100 + 70 + 6) and map the names for each number onto the equation. The neural network is first trained to learn how to decompose number in a language. The number name in each language will then be mapped onto the equation. 

## Summary

## Data
random numbers between 1 - 10,000,000 in Chinese, English, German, French and Russian

## Step 1 
### Input
54876
### Output
For English: (50+4)* 1000 + 8 * 100 + 70 + 6
For Chinese: 5 * 10,000 + 4 * 1000 + 8 * 100 + 7 * 10 + 6
### Model 
Transformer

## Step 2
### Input 
(50 + 4)* 1000 + 8 * 100 + 70 + 6
5 * 10,000 + 4 * 1000 + 8 * 100 + 7 * 10 + 6
### Output
fifty four thousand eight hundred seventy six
wu wan si qian ba bai qi shi liu 
### Model
Rule based mapping

## Publication
In preparation

