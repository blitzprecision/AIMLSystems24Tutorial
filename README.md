# Deep Learning Methods for Query Auto Completion

## Abstract

Query Auto Completion (QAC) aims to help users reach their search intent faster and is a gateway to search for users. Everyday, billions of keystrokes across hundreds of languages are served by Bing Autosuggest in less than 100 ms. The expected suggestions could differ depending on user demography, previous search queries and current trends. In general, the suggestions in the AutoSuggest block are expected to be relevant, personalized, fresh, diverse and need to be guarded against being defective, hateful, adult or offensive in any way. In this tutorial, we will first discuss about various critical components in QAC systems. Further, we will discuss details about traditional machine learning and deep learning architectures proposed for four main components: ranking in QAC, personalization, spell corrections and natural language generation for QAC.

## Motivation for the tutorial

Query Auto Completion (QAC) is the first service that search users interact with. Thus, it is critical to ensure that QAC is highly accurate and efficient. While web search suffers from intent gap (gap between user's information need and the actual query typed by user), the intent gap for QAC is larger since the system needs to guess the intent with just a partially typed query. QAC is challenging -- showing fresh relevant suggestions across languages and regions in a time sensitive and personalized manner involves a very complex orchestration of multiple sub-systems. Advances in deep learning have improved several areas in Natural Language Processing (NLP) and information retrieval including QAC. Given so much work on deep learning for QAC, we think this is a good time to summarize the work in this area in an organized manner. The tutorial should be relevant to researchers and data scientists working in web search companies, domain specific search portals (like Monster, apartments.com, etc.), enterprise search companies, etc.

Learning objectives are: (1) establish an understanding of important components in QAC systems, (2) understand basic machine learning approaches for ranking and personalization for QAC, and (3) understand state-of-the-art deep learning approaches for ranking, personalization, defect removal and natural language generation for QAC systems.

## Presenters' names and bibliography: 

Manish Gupta (http://research.microsoft.com/en-us/people/gmanish/) is a Principal Applied Researcher at Microsoft AI and Research at Hyderabad, India. He is also an Adjunct Faculty at a premier engineering school in India - International Institute of Information Technology, Hyderabad (IIIT-H) and a visiting faculty at the Indian School of Business (ISB). He received his Masters in Computer Science from IIT Bombay in 2007 and his Ph.D. from the University of Illinois at Urbana-Champaign in 2013. With research interests in the areas of deep learning, web mining and information retrieval, he has published more than 100 research papers in referred journals and conferences, including WWW, SIGIR, ECIR, ICDE, KDD, WSDM conferences. He has also co-authored two books: one on Outlier Detection for Temporal Data and another one on Information Retrieval with Verbose Queries. Currently, along with Puneet, he works in the Bing Autosuggest team which is responsible for powering query auto completion across Bing and other Microsoft endpoints.

Manish has a strong track record of teaching. He taught a full credit course on Web Mining at IIIT-H, India in 2013 and in 2014. He currently teaches a course on Information Retrieval and Extraction (with Prof. Vasudeva Varma) at IIIT-H and courses on Text Analytics and Deep Learning at ISB, Hyderabad. He has an extensive experience in offering tutorials at top conferences. Further, he runs a very active youtube channel on large language models (https://www.youtube.com/@dlByManish). 

## Tutorial outline

- Components in Query Auto Completion systems: Ranking suggestions using Most popular completion, Time sensitive suggestions, Location sensitive suggestions, Personalization; Ghosting; Session co-occurrences; Online spell correction; Defect handling; Non-prefix matches; Generating suggestions; Mobile QAC; Enterprise QAC.
- Suggestion Ranking: Traditional Machine Learning methods for ranking suggestions; Convolutional Latent Semantic Model; LSTM encoder; BERT and BART.
- Personalization: Traditional Machine Learning methods; Hierarchical RNN Encoder-decoder with pointer generator; GRUs with user and time representations; Transformer-based hierarchical encoder; Trie-NLG. 
- Handling defective and toxic suggestions and prefixes: LSTMs for inappropriate query suggestion detection; Online Spell Correction: A* search with spell correction pairs; Offline Spell Correction; detoxification.
- Natural Language Generation: RNNs with character and word embeddings; LSTMs with subword embeddings; Hierarchical RNN Encoder-decoder; Next Phrase Prediction with T5; Problems with NLG.
- Summary and Future Trends 

## What will the participants learn from the tutorial.

Practitioners and people from the search industry will clearly benefit from the discussions both from the methods perspective, as well from the real  challenges and experiences that the team had during deployment of such solutions. This tutorial will give them a systematic overview of recent work on QAC using deep learning. A lot of recent research happens based on close collaboration between industry and academia. Thus, this tutorial could be very useful for Masters/PhD students looking for interesting problems in the search industry.   

This tutorial can be considered an intermediate level tutorial where we assume the folks in audience to know some basic deep learning architectures. Prerequisite knowledge includes introductory level knowledge in deep learning, specifically recurrent neural networks models, and transformers. Also, basic understanding of natural language processing and machine learning concepts is expected.
