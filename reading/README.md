# Report: A Survey of Computational Framing Analysis Approaches

AIM: The goal of the paper is to survey existing computational framing analysis approaches and to gain a deeper understanding of how frames are being explored computationally.

## Framing

Frame is largely determined by its outcomes -

1. defining problems
2. diagnosing causes
3. making judgments
4. suggesting remedies

Framing may also include highlighting certain features and omitting others.

## Methods

Corpus for frames analysis can be generated manually by creating frame categories and labelling datasets.

### Topic Modelling

Models such as the LDA model and the STM model can be trained on these datasets. The STM model can also offer additional insights, but both models lack semantic contextualization for exploring frames.

Hierarchical topic modelling considers two levels of agenda and frames.

### Cluster Analysis

k-means clusters were used to cluster different documents using word vectors. These gave a single membership model with each document referring to a topic. However this does not reveal semantic and logical relationships.

### Neural Networks

State of the art pretrained neural network models are used for computational framing analysis. These include LSTM, RNNs, BERT, etc. The quality of the annotated datasets seem to be a bottleneck for this approach.

### Parsing Semantic Relations

This method tries to analyse semantics of the text, unlike the bag-of-words approach. This holds potential for advancing the effort for computational framing analysis.

### Frequency Based

Frames are defined in terms of word occurence in a document. This definition is not an appropriate conceptualization of a frame.

### FrameAxis

Microframes were used as the object of analysis. However the core aspect of 'antonyms' proves to be a limit.

### Topic Model Networks

Topics were clustered into communities which were treated as frames. It tries to combine semantic analysis and topic modelling. However the claim of using communities as frames is not well supported.

## Improving Methods

Most of the aforementioned methods either lacked good conceptualization of what frames are or were limited by their definitions (for example the FrameAxis method).

Improving the conceptualizaiton will be hugely beneficial in framing analysis. One such way to achieve this would be to look at both text and non-text content such as images used in the article or sources cited.

Another avenue of improvement could be to improve the quality of annotated dataset, or to automate the annotation process to get more data more efficiently.

## Applying methods for Elections 2024

The topic model networks method can prove to be very useful - it can be used to create communities of election related articles. These communities can be related to different political agendas such as welfare, healthcare, caste-based, etc. and can give insights about the major issues and talking points for the political landscape.

Another method could be the use of aforementioned neural networks to perform analysis on documents from different news sources. This can be done to identify biases in the text using these models. Identifying bias in news can be an important tool to judge whether a news source is aligned towards a party.

## Project Ideas

The following come to mind:

1. Bias analysis of different news sources. This can be done as mentioned above using models trained to detect biased framing in articles. Getting labelled datasets for this task might prove to be a challenge, since several known biased articles are needed. However this can prove to be very helpful for election analysis.
2. Using topic modelling or cluster analysis to gather articles about elections. These methods can identify whether the article is about the election cycle using the bag-of-words and clustering approaches.
