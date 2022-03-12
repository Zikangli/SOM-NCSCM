1. The format of data: 
i) The Ordinal Number \t The List of the Segmented Chinese Original Query
	\t The List of the Corresponding Label Sequence 
 
2. Instructions:
i) Words in brackets are masked personal information and other sensitive information. If such information in queries contains more than one segmented Chinese word, we will still use one special token to mask that whole piece of word phrase. These tokens will not impede the use and comprehension of query sentences.
ii) Due to the use scenario of the data, user query sentences may be interrogative qeustions or imperative sentences, and their corresponding compressed sentences can be labeled to be declarative sentences.

3. shuffled_idx-3300.txt
i) Format: a list of length 3300.
ii) Description: the all 3300 data should be shuffled before applied to train models. This file provides the shuffled indexes of all data which was used in our paper.
iii) How to use: apply these shuffled indexes to the whole dataset and get the shuffled dataset, then split it into three parts, which produces 3,000, 150 and 150 samples for training set, development set and test set, respectively.
