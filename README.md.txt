Hate Speech Detection

Links

- [Task Description](https://hasocfire.github.io/hasoc/2020/index.html)
- [Slides](https://drive.google.com/file/d/1O35ml7swxw21AjZm4fHkkVlG9-Khy-nt/view?usp=sharing)

Links
https://hasocfire.github.io/hasoc/2020/index.html
https://drive.google.com/file/d/1O35ml7swxw21AjZm4fHkkVlG9-Khy-nt/view

Using the Processed Data

- Refer to the `./data/2020_processed` directories for train and test splits
- One pickle file for each language
- Each having a dictionary structure
- Keys map you to lists containing the following:
  1. `tweet_id`: The provided tweet ID
  2. `task_1`: Label for Task 1
  3. `task_2`: Label for Task 2
  4. `hasoc_id`: Provided ID for the HASOC task
  5. `full_tweet`: The complete tweet as is
  6. `tweet_raw_text`: Pure tweet text without hashtags, smileys, ...
  7. `hashtags`: Hashtags
  8. `smiley`: Smileys
  9. `emoji`: Emojis
  10. `url`: URLs
  11. `mentions`: Mentions
  12. `numerals`: Numbers
  13. `reserved_word`: Reserved Words
  14. `emotext`: A textual description of all emojis
  15. `segmented_hash`: The hashtag text segmented into words
  
Description

<p align="justify"> Detecting and classifying instances of hate in social media text has been a problem of interest in Natural Language Processing in the recent years. Our work leverages state of the art Transformer language models to identify hate speech in a multilingual setting. Capturing the intent of a post or a comment on social media involves careful evaluation of the language style, semantic content and additional pointers such as hashtags and emojis. We look at the problem of identifying whether a Twitter post is hateful and offensive or not. We further discriminate the detected toxic content into one of the following three classes: (a) Hate Speech (HATE), (b) Offensive and (c) Nither. With a pre-trained multilingual Transformer-based masked LM at the base, we are able to successfully identify and classify hate speech from multiple languages. In our experiments, we show the efficacy of Perspective API features for hate speech classification, and the effects of exploiting a multilingual training scheme. 

This is Hate speech detection model created using XGBoost Classifier and decision take with the Lime Algorithm with an Accuracy upto 0.9471, train-test split of 70:30, means that 70% of the knowledge will go to the training set and 30% of the dataset which can be used to predict whether tweets are hate, offensive and nither.