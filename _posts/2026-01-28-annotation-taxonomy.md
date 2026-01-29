---
title: What is annotation? What is taxonomy?
layout: post
comments: true
permalink: /blog/what-is-annotation-taxonomy/
categories:
  - altac
tags:
  - altac
  - jobs
  - prep
  - tech
---

Some of the most common roles that routinely hire linguists in tech involve data annotation, evaluation, and taxonomy design. Roles can involve designing annotation projects, training annotators, creating and/or maintaining taxonomies, creating and/or maintaining guidelines, constructing, collecting, labeling, sampling, or otherwise analyzing properties of data. This post provides some quick definitions and examples of what these things mean in the context of a tech job. This post is a direct companion to my post about [**translating academic linguistic skills into tech skills**](https://hkotek.com/blog/translating-linguist-skills-to-tech-skills/), but can it be read as a standalone. Each section in this post lists to the corresponding section in the companion post and vice versa, for easier navigation.


## Data annotation projects

Linguists in tech companies often work on [**data annotation projects**](https://hkotek.com/blog/translating-linguist-skills-to-tech-skills/#designing-annotation-projects-is-like-designing-human-subjects-studies), broadly construed.[^1] These projects may involve the collection, generation, or labeling of data according to some criteria. The data can be text, image, audio, video, \<insert modality of choice here\>. Content can be short (e.g. URLs, wikipedia page titles, knowledge graph concepts) or longer (e.g. wikipedia page content, requests directed at an LLM, LLM-generated essays, ...), really as complex or simple as you can imagine.

The projects themselves may vary depending on the company's needs. Some examples of projects include (a) identify entities in a text and classify them into types such as person, group, business, or event; (b) read a question+response pair and decide how helpful the response is; (c) ask a question about an image that can't be answered from the text alone without access to the image; (d) listen to a synthetic voice, decide how natural it sounds, and tag problematic parts with relevant flags.   

The results of these data annotation projects will be used to improve the products developed by the company in some way. Often for linguists in tech the relevant products will be ML models. The data would serve as either training or [evaluation](#evaluation-design) data. Annotated data might also contribute to the development of a knowledge graph or taxonomy, or it could be used to help with prototyping of new products or as part of a user study, etc. 

The linguist's involvement in the project may also vary, from full ownership of the full process from ideation to implementation and analysis, or any part of the process. For example, one common setup is that ML engineers may come to a data annotation team with some data need, which may be more or less fleshed out. The linguist will then help with the design and execution. In some cases, there's more flexibility in the design and selection of the label space, and in others it may be inherited from others or pre-determined. Likewise, the design and tooling may be on the table, or you may have limited ability to make choices here. 

## Annotation guidelines 

The people who do the labeling on annotation projects are usually 3rd party workers of some kind. These workers may be full-time employees hired and trained specifically for the annotation work, they may be contractors hired through a vendor company, or they may work on a project on a situational basis without any additional training or opportunity for feedback (such as Amazon Mechanical Turk or Prolific workers). In all cases, these workers will require some training before participating in an annotation project. 

Linguists often engage in writing of [**annotation guidelines**](https://hkotek.com/blog/translating-linguist-skills-to-tech-skills/#training-annotators-is-like-writing-experiment-guidelines) and training of annotators. This is very similar to writing instructions for experimental studies, usually involving some description of the task and goal, a description of the tool, definitions, examples, FAQs. In case the annotators are not situational, linguists will often also engage in training and certification of the annotators, and may additionally engage in providing feedback to improve the annotators' work. If you've ever run an online/in-lab study involving a computer, and written up instructions for how to do the experiment, that's basically it.

We write these annotation guidelines with the understanding that they may be the only way we can communicate with the crowd, but also knowing that the crowd is likely not to read the content as carefully as we wrote it (or at all, perhaps). Therefore, we also invest a lot in the study design itself to make it natural and to try to avoid pitfalls, misinterpretations, or alternative paths to solving the problem than we intend. We provide examples in the hopes that at least those are skimmed, and we consider carefully the right length, visual design, and content, that we include. 

Guideline writing and annotation task design might often be the first place where clarification questions will come up: the task may not be well defined for some input types, or definitions may be conflicting, or the existing examples don't generalize well, or there's no appropriate label for some data, or there's more than one potential label. Linguists may at this point help with a project redesign, or expansion of existing definitions or datasets to address these questions. 


## Taxonomy design

A [**taxonomy**](https://hkotek.com/blog/translating-linguist-skills-to-tech-skills/#creating-a-taxonomy-is-like-developing-a-linguistic-theory), or **ontology**, is a structured framework that defines the categories, labels, and relationships used to annotate data. The resulting label space should comprehensively cover all relevant data, often with minimal or no overlap between labels. Definitions and relationships should be consistent, unambiguous, and aligned with the goals of the dataset, ensuring that different annotators---and consequently models---interpret the data in the same way.

If we return to the examples in the [first section](#data-annotation-projects) of this post, I mentioned several types of annotation projects, including (a) identify entities in a text and classify them into types such as person, group, business, or event; ... (d) listen to a synthetic voice, decide how natural it sounds, and tag problematic parts with relevant flags. These types of projects may come with predefined taxonomies, or you may need to define or refine them. [Named Entity Recognition](https://en.wikipedia.org/wiki/Named-entity_recognition) is a common task in NLP, which has well established categories such as person, organization, location, event, date/time expressions, measurements, and more. You may need to adapt this label space, expand, or constrain it, to fit the needs of the model you are working on. For example, if your product is in the music space, maybe you need detailed categories for different music genres and subgenres. If that's not your focus, maybe a simple `music_genre` label is sufficient for you. Likewise if you are working on tagging parts of synthetically generated speech for problems, you may develop a set of tags such as "pitch is too low", "duration is too long", "lacks aspiration", or "segments overlap", and you may consider how to define and adapt those tags for use by naive labelers.[^2]

Taxonomies can be designed for a variety of needs. For example, in the past several years, financial institutions have been hiring linguists as taxonomists, presumably to help them organize and structure data in systems that interact with users such as chat bot assistants. Taxonomies are crucial when constructing a knowledge graph, the representation that underlies how search engines like google and other information retrieval systems work. Really, any system that requires classification will require a taxonomy. There are a lot of resources around for taxonomy 101. [Here's one](https://www.nngroup.com/articles/taxonomy-101/) I liked recently.


## Evaluation design 

[**Model evaluation**](https://hkotek.com/blog/translating-linguist-skills-to-tech-skills/#designing-an-evaluation-is-like-writing-problem-sets) is the process of systematically assessing how well a model performs on defined tasks using representative test data and appropriate metrics, in order to measure accuracy, robustness, and whether the model meets its intended objectives and real-world requirements. This is yet another space that linguists tend to find themselves in, building on their analytical skills. 

An evaluation is designed by first clearly defining the task and success criteria, including what behaviors or outcomes the model should exhibit. Appropriate metrics are then selected to measure those goals, along with representative and well-controlled datasets that reflect real-world use cases and edge cases. Finally, evaluation protocols are specified---such as data splits, baselines, and error analysis methods---to ensure results are reliable, interpretable, and actionable.

One important aspect of evaluating a model is the design of the evaluation dataset: to perform an evaluation, we must construct or select a dataset that would allow us to measure the right metrics for our model. This **golden dataset** will have highly confident labels, which can then be compared to model predictions and errors can be analyzed. We may select an existing, external *benchmark* dataset, which will allow us to compare ourselves to other models on a leaderboard; or we may design a dataset to specifically target our model and data needs, for example focusing on the most common user experiences expected for the model, perhaps even using customer data, if available, as well as important edge cases we want to make sure we get right. My own work often involves the design and construction (and localization) of targeted datasets.

Hand in hand with dataset design, we also define what **metrics** to measure and report. We may compute some common ML metrics such as *precision*, *recall*, and *F1*, as well as task-specific metrics such as *word error rate*, *BLEU score*, *perplexity*, *human preference rate*, *R<sup>2</sup>*, *Mean Absolute Error*, etc. We might also use metrics with customizable, often complex definitions, such as *helpfulness rate* and *harmfulness rate*. Metrics can be as tailored as needed, and defined to fit specific internal needs. They may also vary by task or dataset --- for example, what would be considered a "helpful" virtual assistant might be different from a "helpful" search algorithm. And different companies may set different definitions for what they consider "helpful" for their own virtual assistant, for example, which may differ from direct competitors.

## Error analysis

One important aspect of doing an evaluation is [**error analysis**](https://hkotek.com/blog/translating-linguist-skills-to-tech-skills/#doing-error-analysis-is-like-doing-linguistic-analysis): the systematic process of examining a model's mistakes to understand why errors occur, identify patterns or edge cases, and uncover weaknesses in the model, data, or annotation. The results of error analysis inform improvements in data quality, model design, annotation guidelines, or evaluation metrics to guide more effective iterations. 

When I do error analysis, I consider several sources for errors in model performance. Some errors may be traced back to annotator error, which I may then trace back to gaps in the guidelines, conflicting examples, confusing definitions, poor task design, inadequate training, or laziness of annotators. We might then fix our golden labels and also iterate on our design and definitions, as needed. Some errors may be due to ambiguity in our taxonomy definitions. Other errors might be due to model performance, which we may then trace back to gaps or skews in training data, ambiguity or confusion in how the model prompt was written, limitations in the model architecture, insufficient fine-tuning, or unexpected edge cases in the input data. If this is the issue, we might engage in some prompt optimization (aka **prompt engineering**), or we might audit our training data to decide if any changes are needed. We take both the frequency and severity of issues into account. Very mild and unlikely errors will garner less attention than major, frequent ones. 


Based on the evaluation results and error analysis, we will often report outcomes, provide feedback, and generate additional **insights**. We might make recommendations regarding product readiness or prioritization of future work. We'll communicate our findings differently depending on what how we diagnose the issues.


## The gist

What a lot of these things will have in common is some of what makes linguistic training outstanding: (a) being comfortable with abstract reasoning; (b) identifying patterns and exceptions in data; (c) explaining the causes for those generalizations and outliers; (d) introspecting about how non-specialists interact with the data; (e) teaching non-specialists to do the same (language) task consistently and successfully. 


&nbsp;

#### Notes

[^1]: I use "annotation" very vaguely here. Data authoring isn't really annotation per se, though it often will come along with an annotation task (e.g. you write some text to some specifications, and you choose what labels it should be assigned). You might also see people use words like "labeling" or "grading", and annotators might also be called "analysts" or "labelers" or "graders". For our purposes, these terms are basically interchangeable. 


[^2]: I totally just made this faux-phonetic label set up, and I'm not a p-side person, so please don't yell at me. 
