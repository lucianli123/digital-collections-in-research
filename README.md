# Mass Digitization in Research Workflows

Code for the Culture at Scale project "Mass Digitization in Research Workflows"

## Data
[Download data here](https://uofi.box.com/s/qpvhd9w194obtglygywc8h5fy3uc6s7m)
1. full_meta.csv: post filtering articles, includes title, data author, full text, predicted scores for each subject, and if each digitized collection is mentioned in the article
2. tfidf_eng.csv: bag of words counts for each article
3. subj.csv: subject scores gfor each article generated with logistic classifiers trained on expert assigned labels.

## Code
1. api: discover and download using api and web scraping from open source journals
2. read_json: use downloaded Constellate files to generate metadata and text
3. semantic_scholar_download: discover and download using api access from semantic scholar search
4. topic model: use gensim topic modelling to remove non-English and likely false matches
5. pred: use logistic regression to generate subject likelihood predictions for each article
6. date_analysis: plot breakdowns of subject and topic by dates
7. word embeddings: use doc2vec to generate word embedding models for the corpus
