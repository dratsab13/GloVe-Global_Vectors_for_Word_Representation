# Project 2 - Team Gemera, team_ind 13
## CSS503 - Advanced Programming Technologies course
## “GlоVе: Glоbаl Vеctоrs fоr Wоrd Rеprеsеntаtiоn”.

![Wоrd Rеprеsеntаtiоn](https://media.giphy.com/media/87jGply3Ophq36yhaP/giphy.gif)

### Dear Reader, we are Team Gemera and we are happy to see you here again!

Among the dozens of articles offered to us, for our Project we chose the one that seemed the most interesting to us -  “GlоVе: Glоbаl Vеctоrs fоr Wоrd Rеprеsеntаtiоn”.


### Shortly about GloVe

The GloVe model stands for Global Vectors (and has nothing to do with gloves, unfortunately) which is an unsupervised learning model which can be used to obtain dense word vectors similar to Word2Vec. However the technique is different and training is performed on an aggregated global word-word co-occurrence matrix, giving us a vector space with meaningful sub-structures. This method was invented in Stanford by Pennington et al. and you can easily find the original article right [here](https://nlp.stanford.edu/pubs/glove.pdf).

![GloVe](https://media.giphy.com/media/MY01tMGTj6nEIvHzxA/giphy.gif)

We won’t cover the implementation of the model from scratch in too much detail right here but if you are interested in the actual code, you can check out the official [GloVe page](https://nlp.stanford.edu/projects/glove/). We will keep things simple here and try to understand the basic concepts behind the GloVe model. We have talked about count based matrix factorization methods like LSA and predictive methods like Word2Vec. The paper claims that currently, both families suffer significant drawbacks. Methods like LSA efficiently leverage statistical information but they do relatively poorly on the word analogy task like how we found out semantically similar words. Methods like skip-gram may do better on the analogy task, but they poorly utilize the statistics of the corpus on a global level.

In the original article authors present a simple example based on the words ice and steam that sheds some light on this question. The relationship of these words can be examined by studying the ratio of their co-occurrence probabilities with various probe words, k.

![Image alt](https://blog.acolyer.org/wp-content/uploads/2016/04/glove-table-1.png)

The basic methodology of the GloVe model is to first create a huge word-context co-occurence matrix consisting of (word, context) pairs such that each element in this matrix represents how often a word occurs with the context (which can be a sequence of words). The idea then is to apply matrix factorization to approximate this matrix as depicted in the following figure.

![Image alt](https://cdn-images-1.medium.com/max/800/1*UNtsSilztKXjLG99VXxSQw.png)

### Dear friend, please, feel free to leave your comments below and come visit us again any time!

![Friends](https://media.giphy.com/media/ZCZVa6W2f1W4mATLEc/giphy.gif)

Best regards,
Aidana, Yerkebulan, Bekzot and Olzhas.
