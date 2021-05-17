# **How to Paraphrase text in Python with PARROT**


<a href="https://github.com/PrithivirajDamodaran/Parrot"><img width="150" src="https://github.com/PrithivirajDamodaran/Parrot/raw/main/images/Logo.png"></a>

---

### Paraphrasing:- 
A paraphrase is a restatement of the meaning of a text or passage using other words. The term itself is derived via Latin paraphrasis from Greek παράφρασις, meaning "additional manner of expression". The act of paraphrasing is also called "paraphrasis".


### Parrot
Parrot is a paraphrase based utterance augmentation framework purpose built to accelerate training NLU models. A paraphrase framework is more than just a paraphrasing model.

### Why Parrot?
Huggingface lists 12 paraphrase models, RapidAPI lists 7 fremium and commercial paraphrasers like QuillBot, Rasa has discussed an experimental paraphraser for augmenting text data here, Sentence-transfomers offers a paraphrase mining utility and NLPAug offers word level augmentation with a PPDB (a multi-million paraphrase database). While these attempts at paraphrasing are great, there are still some gaps and paraphrasing is NOT yet a mainstream option for text augmentation in building NLU models....Parrot is a humble attempt to fill some of these gaps.

What is a good paraphrase? Almost all conditioned text generation models are validated on 2 factors, (1) if the generated text conveys the same meaning as the original context (Adequacy) (2) if the text is fluent / grammatically correct english (Fluency). For instance Neural Machine Translation outputs are tested for Adequacy and Fluency. But a good paraphrase should be adequate and fluent while being as different as possible on the surface lexical form. With respect to this definition, the 3 key metrics that measures the quality of paraphrases are:

Adequacy (Is the meaning preserved adequately?)
Fluency (Is the paraphrase fluent English?)
Diversity (Lexical / Phrasal / Syntactical) (How much has the paraphrase changed the original sentence?)
Parrot offers knobs to control Adequacy, Fluency and Diversity as per your needs.

What makes a paraphraser a good augmentor? For training a NLU model we just don't need a lot of utterances but utterances with intents and slots/entities annotated. Typical flow would be:

Given an input utterance + input annotations a good augmentor spits out N output paraphrases while preserving the intent and slots.
The output paraphrases are then converted into annotated data using the input annotations that we got in step 1.
The annotated data created out of the output paraphrases then makes the training dataset for your NLU model.
But in general being a generative model paraphrasers doesn't guarantee to preserve the slots/entities. So the ability to generate high quality paraphrases in a constrained fashion without trading off the intents and slots for lexical dissimilarity makes a paraphraser a good augmentor. More on this in section 3 below


## About me

**Piyush Pathak**

[**PORTFOLIO**](https://anirudhrapathak3.wixsite.com/piyush)

[**GITHUB**](https://github.com/piyushpathak03)

[**BLOG**](https://medium.com/@piyushpathak03)


# 📫 Follw me: 

[![Linkedin Badge](https://img.shields.io/badge/-PiyushPathak-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/piyushpathak03/)](https://www.linkedin.com/in/piyushpathak03/)

<p  align="right"><img height="100" src = "https://media.giphy.com/media/l3URDstnIjBNY7rwLB/giphy.gif"></p>
