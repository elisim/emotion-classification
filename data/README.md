# EmotionLines Description

EmotionLines contains a total of 29245 labeled utterances from 
2000 dialogues. Each utterance in dialogues is labeled with one of 
seven emotions, six Ekman’s basic emotions plus the neutral emotion. Each labeling was 
accomplished by 5 workers, and for each utterance in a label, the emotion category with 
the highest votes was set as the label of the utterance. 
Those utterances voted as more than two different emotions were put into the non-neutral category. 
Therefore the dataset has a total of 8 types of emotion labels:

* anger
* disgust
* fear
* happiness
* sadness
* surprise 
* neutral
* non-neutral

Reference: [paperswithcode - emotionlines](https://paperswithcode.com/dataset/emotionlines)

## Technical Details
**Download link:** http://doraemon.iis.sinica.edu.tw/emotionlines/download.html

It contains two datasets, Friends and EmotionPush. The Friends dataset is open to download,
while the EmotionPush dataset is not (need to ask for access). 

### Problem Definition
Given the transcript of a conversation along with speaker
information of each  utterance, the ERC task aims
to identify the emotion of each utterance from a set of predefined emotions. 
Fig. 2 illustrates one such conversation between two people, where each utterance is labeled by
the underlying emotion. Formally, given the input sequence
of `N` number of utterances `[(u1, p1), (u2, p2), . . . ,(uN , pN )]`,
where each utterance `ui = [ui,1, ui,2, . . . , ui,T ]` consists of `T`
words `ui,j` and spoken by party `pi`, the task is to predict the
emotion label `ei` of each utterance `ui`

Reference: [Emotion Recognition in Conversation](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8764449).
This paper contains "datasets" section, which contains another datasets for emotion recognition 
in dialogues.


# My Plan
* Reproduce the methods from emotionlines paper
* Think about transformers

Questions: what to check now in the EDA? 
In this type of problem, how can we use transformers to find the order?