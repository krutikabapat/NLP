# NLP  

## Basic Tasks in NLP:  
1. Sentimental Analysis  
2. Question Answering  
3. Text Summarization  
4. Machine Translation  
5. Image to text generation  
6. Natural Language Translators.  

![Screenshot](NLP.png)
## Question Answering Techniques and Paradigms  

Approaches of Question Classification:  

<b>Manual classification:</b>​ Manual classification applies hand-made rules to identify expected answer types. These rules may be accurate but they are time-consuming, tedious, and non-extensible in nature.  

<b>Automatic classification:</b>​ This type of definition helps on a better answer detection. Automatic classifications, in contrast, are extensible to new questions types with acceptable accuracy.  

## Type of Questions:  

<b>Factoid:</b> ​ Factoid questions are the ones that ask about a simple fact and can be answered in a few words.  

<b>Complex questions:</b>​ Complex Question is about information in a context. Usually, the answer is a merge of retrieved passages.
Examples to implement the above: Normalized Raw-Scoring, Logistic Regression, Round-Robin, Raw Scoring and 2-step RSV.  

<b>List Questions:</b> ​ Demands as an answer a set of entities that satisfies a given criteria.  
Example: When did Brazil win Soccer World Cups? illustrates this point clearly.  
 
<b>Definition questions:</b>​ They expect a summary or a short passage in return
How does the mitosis of a cell work?  

## Types of QA systems can be defined by the paradigm each one implements:

<b>Information Retrieval QA:</b>​ Usage of search engines to retrieve answers and then apply filters and ranking on the recovered passage.  

<b>Natural Language Processing QA:</b>​ Usage of linguistic intuitions and machine learning methods to extract answers from retrieved snippet.  

<b>Knowledge Base QA:</b>​ Find answers from structured data source (a knowledge base) instead of unstructured text. Standard database queries are used in replacement of word-based searches. This paradigm, make use of structured data, such as ontology. An ontology describes a conceptual representation of concepts and their relationships within a specific domain. Ontology can be considered as a knowledge base which has a more sophisticated form than a relational database (Abdi et al., 2016). To execute queries in order to retrieve knowledge from the ontology, structured languages are proposed and one of then is SPARQL.  

<b>Hybrid QA:</b>​ High performance QA systems make use of as many types of resources as possible, especially with the prevailing popularity of modern search engines and enriching community contributed knowledge on the web. A hybrid approach is the combination of IR QA, NLP QA and KB QA. The main example of this paradigm is IBM Watson.  


## Reference material to read:  

1. https://www.semanticscholar.org/paper/A-literature-review-on-question-answering-paradigms-Soares-Parreiras/bf4f4ebd43ac87431fdf978988c2a90b1034e994  
2. https://www.aclweb.org/anthology/S13-1041.pdf  
3. https://arxiv.org/pdf/1905.07098v2.pdf  
4. https://towardsdatascience.com/automatic-question-answering-ac7593432842  
5. https://www.kdnuggets.com/2017/12/general-approach-preprocessing-text-data.html (NLP Processing)  
6. https://medium.com/@ageitgey/natural-language-processing-is-fun-9a0bff37854e  
7. https://github.com/Kyubyong/nlp_tasks (useful github repo)  
8. https://github.com/keon/awesome-nlp#reading-content (useful github repo)   
9. https://arxiv.org/pdf/1801.06287.pdf (Text CNN)  
10. https://arxiv.org/pdf/1808.04926.pdf (How Much Reading Does Reading Comprehension Required?)  
11. https://arxiv.org/abs/1804.09541 (QA Net)  
12. https://towardsdatascience.com/nlp-building-a-question-answering-model-ed0529a68c54  
13. http://jalammar.github.io/illustrated-transformer/  
14. https://lambdaviking.com/post/capsule-networks-for-nlp/writeup.pdf  
15. https://github.com/facebookresearch/  (DRQA Implementation)
16. https://hackernoon.com/finding-the-most-important-sentences-using-nlp-tf-idf-3065028897a3  (TF-IDF Matching)  
17. https://arxiv.org/abs/1611.01603 (BiDAF)  
18. https://towardsdatascience.com/bert-explained-state-of-the-art-language-model-for-nlp-f8b21a9b6270  (Bert Implementation)    
19. https://github.com/facebookresearch/DrQA/issues/4 (Issues in DRQA Implementation)  
20. https://towardsdatascience.com/tf-idf-for-document-ranking-from-scratch-in-python-on-real-world-dataset-796d339a4089
(TF-IDF Matching)  
21. https://machinelearningmastery.com/how-does-attention-work-in-encoder-decoder-recurrent-neural-networks/ (Attention Models)  
22. https://medium.com/analytics-vidhya/fundamentals-of-bag-of-words-and-tf-idf-9846d301ff22 (Bag Of Words).   
23. https://spacy.io/usage/spacy-101  
24. https://towardsdatascience.com/building-a-question-answering-system-part-1-9388aadff507  
25. https://github.com/davidgolub/QuestionGeneration (Generating Questions for a target domain daatset).  
26. https://www.analyticsvidhya.com/blog/2018/11/introduction-text-summarization-textrank-python/ (Text Summarization in NLP)    
27. https://medium.com/inside-machine-learning/what-is-a-transformer-d07dd1fbec04 (Transformers in NLP)    



## Latest Libraries to have knowledge about related to NLP:  

1. gluonnlp  
2. tqdm  
3. ParlAI  
4. allennlp  
5. Spacy  
6. Corenlp  

## Dataset:  

1. SQuAD v1 and v2 (https://rajpurkar.github.io/SQuAD-explorer/)    
2. MCTest (Machine comprehension): It contains 660 stories with 4 questions per story and 4 answer choices per question.  
3. WikiQA: WikiQA is an open domain dataset of question and sentence pairs, collected and annotated for research on open-domain question answering.  
4. CLOZE dataset: To predict a missing word in the passage.  
5. WIKIMOVIES Dataset (220K questions and 18K wikipedia articles)  
6. Quora dataset  
7. Twitter datset  

## Present Methods of Question-Answer Retrieval:

a) Dynamic Coattention Nets  
b) Multi Perspective Matching  
c) BiDAF  
d) R-Net  
e) DRQA  
f) QNet  

## Create embeddings:  

a) Character Embeddings (Char-CNN)  
b) Word Embeddings (GLove)  
c) Seq2Seq Model (https://www.analyticsvidhya.com/blog/2018/03/essentials-of-deep-learning-sequence-to-sequence-modelling-with-attention-part-i/#:~:text=A%20typical%20sequence%20to%20sequence,smaller%20dimensional%20representation%20of%20it.)  
## Evaluation Matrices:  

Most of the networks use ESM and F1 score as a matrix for evaluation.  
<b>a) Exact String Match (ESM): </b>​ The target and the generated string must match completely.  
<b>b) F1 score:</b>​ The percentage of generated string words that match with the target words.   
<b>c) BLEU Score:</b>   
<b>d) METEOR Score:</b>  






