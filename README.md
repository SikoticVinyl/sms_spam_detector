# SMS Spam Detection Project

## Overview
A straightforward project using machine learning to detect spam SMS messages. Initially started with a basic implementation, but it got interesting when we noticed it wasn't catching obvious spam messages (like those "$5000 winner!!" texts we all love to get 😄).

## What It Does
- Takes SMS messages as input
- Tells you if it's spam or not
- Has a nice web interface using Gradio
- Comes with some classic spam examples to test with

## The Journey
Started simple but ran into some fun challenges:
1. First version was like "nah, winning $5000 is totally legit!" 🤦‍♂️
2. Had to beef up the model with better text processing
3. Added special spam markers for those sneaky prize/money combinations
4. Finally got it to recognize that no, you didn't actually win $5000

## Technical Improvements Made
- Enhanced the TF-IDF vectorizer settings
- Added preprocessing to catch spam patterns
- Adjusted class weights to be more spam-sensitive
- Fixed some Gradio interface quirks
- Made sure preprocessing was consistent across training and testing

## Quick Start
1. Make sure you have the requirements:
```bash
pip install pandas scikit-learn gradio
```

2. Load up your SMS dataset
3. Run the classifier
4. Test it out with the Gradio interface

## Fun Fact
The project was pretty straightforward to get running at 50% accuracy, but making it actually useful was the fun part. Sometimes "good enough" isn't good enough when your model thinks winning thousands of dollars from random texts is legitimate! 😅

## Files
- `gradio_sms_text_classification.ipynb`: Main notebook with all the code for the app.
- `SMSSpamCollection.csv`: Dataset for training.
- `sms_text_classification_solution`: Initial notebook with model work.
