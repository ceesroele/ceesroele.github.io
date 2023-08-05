# Cees Roele @ github

Overview of my [repositories @github](https://github.com/ceesroele).

# Projects

## BART for Span Dection and Classification

Participation as *Team WVOQ* in SemEval 2021 Task 6: [Detection of Persuasion Techniques in Texts and Images](https://aclanthology.org/2021.semeval-1.7/)

(*WVOQ* stands for *Willard Van Orman Quine*, the 20th century philosopher of logic, language, and epistemology)

* Created an innovative system to simultaneously detect spans (fragments of texts) and classify them for 20 manipulative techniques of language use. It re-generated the input text and added XML-like markings to identify the range of predicted spans.
* Based on the LLM BART, used additional input from a simultaneously developed system based on RoBERTa, used ensemble technique to make predictions.
* Data exploration, pre-processing, developing multiple models in the research phase, and using metrics for repeated testing to determine the final best model.
* Github: [https://github.com/ceesroele/SemEval-2021-Task-6](https://github.com/ceesroele/SemEval-2021-Task-6)
* Github: [https://github.com/ceesroele/span_model](https://github.com/ceesroele/span_model) - generalisation of the code so it can also 
be used for other span detection / classification tasks.

Paper published in the SemEval 2021 conference proceedings: [BART for Span Detection and Classification](https://aclanthology.org/2021.semeval-1.32/)


## Persuasive techniques, sarcasm, and toxic language

* Application of pre-trained Large Language Models to classify text for different modes of expression
* Using the new-for-2022 spaCy "spans", a generalisation of NER-tagging allowing for custom classification and overlapping fragments
* Integrated custom F1-macro/F1-micro metrics for spans into spaCy
* Explained how to actually use the spaCy span visualizer such that the results are clear and 
  good looking (which they aren't out-of-the-box)
* Github persuasive techniques: [https://github.com/ceesroele/persuasion_spans](https://github.com/ceesroele/persuasion_spans)
* Github toxic spans: [https://github.com/ceesroele/toxic_spans](https://github.com/ceesroele/toxic_spans)
* Github sarcasm: [https://github.com/ceesroele/sarcasm_detection](https://github.com/ceesroele/sarcasm_detection)

Articles @medium:
* [Detecting Persuasion with spaCy](https://cees-roele.medium.com/detecting-persuasion-with-spacy-6b6beba51076)
* [Detecting Toxic Spans with spaCy](https://cees-roele.medium.com/detecting-toxic-spans-with-spacy-c5533786bbf8)
* [Custom Evaluation of Spans in spaCy](https://cees-roele.medium.com/custom-evaluation-of-spans-in-spacy-f1f2e7a99ad8)
* [Displaying spaCy Spans](https://cees-roele.medium.com/displaying-spacy-spans-fc3a43810524)

> spaCy / spans of text / classification / transformers / Large Language Models / RoBERTa / python


## Research on "Disinformation"

EUvsDisinfo is unique website in having over 15,000 articles published since 2015 which can be 
studied to understand how the notion of "disinformation" is used by the European Union.

* Scraped 15,000 articles, extracted information using BeautifulSoup, and explored their content
* Clustering TF-IDF with K-means using sklearn
* Used spaCy matcher, NER-parser, and part-of-sentence analysis to characterize clusters by a POS classified centroids, which makes it possible to compare clusters using as aspects Geographical, Group, and Organisation to compare entities, and Noun, Verb, and Adjective to compare actions & objects.
* Clustering the same data using BERTopic. Analysing clustering of topics over time.
* Created a "Term Score Matrix" as an efficient visualization of the words most representative for topics.
* Github: https://github.com/ceesroele/disinformation

@medium:
* [Exploring 'Disinformation' at EUvsDisinfo](https://cees-roele.medium.com/exploring-disinformation-at-euvsdisinfo-6cec6c7f05e2)
* [Disinformation Topics over Time](https://cees-roele.medium.com/disinformation-topics-over-time-5c9ec21300f9)
* [A Term Score Matrix for BERTopic](https://cees-roele.medium.com/a-term-score-matrix-for-bertopic-821e78e198ee)
* [Styling Complex Values in a Dataframe](https://cees-roele.medium.com/styling-complex-values-in-a-dataframe-7ebc5a17b3e7)

> python / pandas / BERTopic / spaCy / NER / sklearn / TF-IDF / K-means / BeautifulSoup / Jupyter / Seaborn


## Participated in contest for SemEval 2023

Participation as "Team Riga" in SemEval 2023 Task 3: ["Detecting the genre, the framing, and the persuasian techniques in online news in a multi-lingual setup"](https://propaganda.math.unipd.it/semeval2023task3/)

*(release to github forthcoming)*

Unfortunately, the dataset is not public, which reduces the reproducibility of my code and hence makes
publication less interesting.
    
* Created a multi-lingual system to classify texts in three types of classification.
* Feature engineering: using the different classification systems to add extra information to training the other ones.
* Data augmentation through machine translation.
* 6 languages for training and test, 3 more languages for zero-shot prediction.
* Data exploration: found that the distribution of classes is different for different languages, 
  suggesting cultural differences.
* Automated testing of different models/datasets

> RoBERTa / mBERT / Marian / python / transformers / parameter tuning / automated testing


# Various

## AutoKeras Search Space

[AutoKeras](https://github.com/keras-team/autokeras) is an Automatic Machine Learning system based on Keras/Tensorflow.

I found:
* Alternative search strategies like random search not working.
* The algorithm regularly got stuck in a local maximum
* Bloated memory use with large models
* Pre-selecting models is more promising, but then one can just as well use [Keras Tuner](https://keras.io/keras_tuner/)

For my explorations, see my [AK Searchspace repository](https://github.com/ceesroele/ak_searchspace)

> AutoKeras / Keras Tuner / python


# Study exercises

For a number of courses a publication of results at github was required.
I could delete these repositories as they serve no purpose beyond these courses, 
but for now they are still there.

## IBM Data Science

Introductory IBM set of 9 courses @Coursera (now only available as a combination of two Coursera "specializations")
* [Introduction to Data Science](https://www.coursera.org/specializations/introduction-data-science)
* [Applied Data Science](https://www.coursera.org/specializations/applied-data-science)

Capstone @github: [What kind of restaurant in Riga?](https://github.com/ceesroele/Coursera_Capstone)

> python / KMeans / FourSquare API / geocoding / Folium / Seaborn / Jupyter


## Johns Hopkins Data Science

Johns Hopkins set of 10 courses @Coursera on Data Science
* [Data Science](https://www.coursera.org/specializations/jhu-data-science)

> This is a good overview of Data Science with a healthy emphasis on statistics. The practica all used *R*.

Course assignments:
* [Getting and Cleaning Data](https://github.com/ceesroele/Getting-And-Cleaning-Data)
* [Exploratory Data Analysis](https://github.com/ceesroele/ExData_Plotting1)
* [R Programming](https://github.com/ceesroele/ProgrammingAssignment2) / [R ...](https://github.com/ceesroele/datasciencecoursera)
* [Reproducible Research](https://github.com/ceesroele/RepData_PeerAssessment1)
* [Practical Machine Learning](https://github.com/ceesroele/PracticalMachineLearning)
* [Developing Data Products](https://github.com/ceesroele/DevelopingDataProducts)

> R / statistics / machine learning / regression models / visualization / shiny / Rmarkdown / knitr
