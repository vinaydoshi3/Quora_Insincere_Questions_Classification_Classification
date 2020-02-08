# Quora_Insincere_Questions_Classification_Classification
Detect toxic content to improve online conversations

# Challenge Description
Quora is a platform that empowers people to learn from each other. On Quora, people can ask questions and connect with others who contribute unique insights and quality answers. A key challenge is to weed out insincere questions -- those founded upon false premises, or that intend to make a statement rather than look for helpful answers.

In this competition, you will develop models that identify and flag insincere questions. To date, Quora has employed both machine learning and manual review to address this problem. With your help, they can develop more scalable methods to detect toxic and misleading content.

# Data Description
An insincere question is defined as a question intended to make a statement rather than look for helpful answers. Some characteristics that can signify that a question is insincere:

Has a non-neutral tone
Has an exaggerated tone to underscore a point about a group of people
Is rhetorical and meant to imply a statement about a group of people
Is disparaging or inflammatory
Suggests a discriminatory idea against a protected class of people, or seeks confirmation of a stereotype
Makes disparaging attacks/insults against a specific person or group of people
Based on an outlandish premise about a group of people
Disparages against a characteristic that is not fixable and not measurable
Isn't grounded in reality
Based on false information, or contains absurd assumptions
Uses sexual content (incest, bestiality, pedophilia) for shock value, and not to seek genuine answers
The training data includes the question that was asked, and whether it was identified as insincere (target = 1). The ground-truth labels contain some amount of noise: they are not guaranteed to be perfect.

# File Description
train.csv - the training set

test.csv - the test set

sample_submission.csv - A sample submission in the correct format

External data sources are not allowed for this competition. We are, though, providing a number of word embeddings along with the dataset that can be used in the models. These are as follows:

GoogleNews-vectors-negative300 - https://code.google.com/archive/p/word2vec/

glove.840B.300d - https://nlp.stanford.edu/projects/glove/

paragram_300_sl999 - https://cogcomp.org/page/resource_view/106

wiki-news-300d-1M - https://fasttext.cc/docs/en/english-vectors.html

# Data Fields Description
qid - unique question identifier

question_text - Quora question text

target - a question labeled "insincere" has a value of 1, otherwise 0

# Evaluation Metric
Submissions are evaluated on F1-Macro Score between the predicted class and the observed target.

# LB Score = 0.684
 
