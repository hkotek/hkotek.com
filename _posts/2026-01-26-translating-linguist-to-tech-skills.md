---
title: Translating academic linguistic skills to tech skills
layout: post
comments: true
permalink: /blog/translating-linguist-skills-to-tech-skills/
categories:
  - altac
  - academia
tags:
  - altac
  - academic
  - jobs
  - linguistics
  - prep
  - resumes
---

There were several excellent presentations at this year's [**LEXING**](https://www.lsadc.org/lexing). In a talk titled *Linguists are Exceptional Inductive Reasoners – A Case Study on Skill Relevance in Enterprise Software*, [**Maggie Baird**](https://www.linkedin.com/in/maggie-baird-167129102/) laid out a mapping between her everyday work as a linguist on an engineering team developing a generative AI product and three tasks commonly carried out by academic linguists. It resonated with me --- it's also very true of my job and skills. In this post, I spell out my version of Maggie's ideas.[^1] 

The gist: \<tech skill\> is like \<linguist skill\>
- [Designing annotation projects *is like* designing human subjects studies](#designing-annotation-projects-is-like-designing-human-subjects-studies)
- [Training annotators *is like* writing experiment guidelines](#training-annotators-is-like-writing-experiment-guidelines)
- [Creating a taxonomy *is like* developing a linguistic theory](#creating-a-taxonomy-is-like-developing-a-linguistic-theory)
- [Designing an evaluation *is like* writing problem sets](#designing-an-evaluation-is-like-writing-problem-sets)
- [Doing error analysis *is like* doing linguistic analysis](#doing-error-analysis-is-like-doing-linguistic-analysis)
- [Data analysis *is like* data analysis](#data-analysis-is-like-data-analysis)


## Designing annotation projects *is like* designing human subjects studies

Linguists in tech companies often work on **data annotation projects**, whose results serve as either training or evaluation data for machine learning models. The projects themselves may vary depending on the company's needs. Some examples of projects include (a) identify entities in a text and classify them into types such as person, group, business, or event; (b) read a question+response pair and decide how helpful the response is; (c) ask a question about an image that can't be answered from the text alone without access to the image; (d) listen to a synthetic voice, decide how natural it sounds, and tag problematic parts with relevant flags.   

The skills associated with this kind of work are similar to the skills used in **experimental study design**.

div.compact-list ol li ul {
  padding-left: 1em !important;
  margin-top: 0 !important;
  margin-bottom: 0 !important;
}

<div class="compact-list">
1. Understand project goals: what the data will be used for, how, and by whom
2. **Operationalize** the problem:
    - define label space (see [taxonomy](#creating-a-taxonomy-is-like-developing-a-linguistic-theory) below)
    - decide on the number of datapoints per label
    - identify data sources
    - sample/compile data
3. **Design** the project:
    - simple to teach to large/untrained annotators
    - ensures consistent, accurate data collection
    - fits budget and timing constraints
4. Create the project in your **tool**:
    - visual design elements
    - minimize effort via spatial layout
    - ordering of items
    - allow annotators to change previous answers?
5. Identify **annotator skills**:
    - write guidelines (see [training annotators](#training-annotators-is-like-writing-experiment-guidelines) below)
    - create practice items
    - set minimum participation requirements (language, age, region, accuracy, ...)
    - define appropriate compensation
</div>

Other linguists, such as those who engage in **elicitation work**, **ethnographic work**, **corpus work**, or **formal theoretical work** also engage in at least part of this process. Really, any scientifically driven exploration will require operationalizing a problem and determining an appropriate label space, perhaps also recruitment of speakers and setting of a task and payment. They differ in that these tasks often happen with the experimenter in the room or in a small group setting (or with the experimenter being the only person in the room), whereas larger studies such as annotation studies most often involve naive workers who experimenters have a limited ability to train or provide feedback to. 

I believe this is the most direct skillset I took with me from my academic work into my industry job. I want to stress in particular the earlier ideation parts: *understand the goals of the project* -- projects in my industry job are frequently initiated by external needs of other engineering groups. The work of clearly defining what the goal of the project is and how the data will be used is key, and is something that in my experience a lot of engineers struggle with, both in explaining in words what they need and in being able to generalize beyond 1-2 examples they have in their heads. Finding generalizations, edge cases, the right examples, and the right categories to use, are all things linguists excel at.  


## Training annotators *is like* writing experiment guidelines

The data annotation projects described [above](#designing-annotation-projects-is-like-designing-human-subjects-studies) are often staffed by 3rd party workers of some kind. These workers may be full-time employees hired and trained specifically for the annotation work, they may be contractors hired through a vendor company, or they may work on a project on a situational basis without any additional training or opportunity for feedback (such as Amazon Mechanical Turk or Prolific workers). In all cases, these workers will require some training before participating in an annotation project. 

In the case of long-term workers, such as FTEs or contractors who are dedicated to the work full time, there will likely be an initial training and certification stage to ensure a shared knowledge base. In the case of situational workers, this is not possible. In both cases, annotation project designers will include **guidelines** and perhaps **practice items** along with their task. The goal of the guidelines is to ensure a basic understanding of the project; good guidelines will describe the tool and steps involved in the task, define concepts and labels, answer frequently asked question, and provide some examples of how to use the labels in the context of the task. 

The skills associated with this kind of work are again similar to the skills used in **experimental study design** and to an extent in **elicitation study design**.

1. Understand the **technical goals** of the project
2. Communicate goals to a **non-technical audience**
3. Identify key concepts and skill-appropriate **definitions**
4. Provide a comprehensive set of **examples** to support generalization

We write these annotation guidelines with the understanding that they may be the only way we can communicate with the crowd, but also knowing that the crowd is likely not to read the content as carefully as we wrote it (or at all, perhaps). Therefore, we also invest a lot in the study design itself to make it natural and to try to avoid pitfalls, misinterpretations, or alternative paths to solving the problem than we intend. We provide examples in the hopes that at least those are skimmed, and we consider carefully the right length, visual design, and content, that we include. 

The creation of annotation project guidelines is similar the creation of guidelines for experimental work. To an extent, they are also similar to the prep work needed for **elicitation studies**, to ensure the right content and form of communication with consultants, as well as careful task design to ensure maximal likelihood of yielding usable results, as discussed in the previous section [above](#designing-annotation-projects-is-like-designing-human-subjects-studies). 


## Creating a taxonomy *is like* developing a linguistic theory

A **taxonomy**, or **ontology**, is a structured framework that defines the categories, labels, and relationships used to annotate data. The resulting label space should comprehensively cover all relevant data, often with minimal or no overlap between labels. Definitions and relationships should be consistent, unambiguous, and aligned with the goals of the dataset, ensuring that different annotators---and consequently models---interpret the data in the same way.

Linguists are often hired as taxonomists, and though they may initially be confused about why we are considered so appropriate for this role, I think that our training and disposition gives us an excellent preparation for this kind of work. 

8. Understand how annotated data will be used in training and evaluation, including impacts on bias, performance, and generalization
1. Break complex data into clear categories, hierarchies, and relationships
2. Write clear, unambiguous definitions that annotators (and models) can interpret consistently
3. Understand how annotators actually apply labels (and how models learn them); balance theoretical neatness with practical usability
4. Handle edge cases, overlaps, and exceptions; refine labels to reduce ambiguity and noise
5. Iterate, test, and evolve taxonomies based on feedback, data drift, or model performance
6. Collaborate across stakeholders---annotators, engineers, researchers, product teams---incorporating feedback without losing coherence
7. Maintain guidelines, change logs, and versioning to keep the taxonomy stable and auditable


If we return to the examples in the [first section](#designing-annotation-projects-is-like-designing-human-subjects-studies) of this post, I mentioned several types of annotation projects, including (a) identify entities in a text and classify them into types such as person, group, business, or event; ... (d) listen to a synthetic voice, decide how natural it sounds, and tag problematic parts with relevant flags. These types of projects may come with predefined ontologies, or you may need to define or refine them. [Named Entity Recognition](https://en.wikipedia.org/wiki/Named-entity_recognition) is a common task in NLP, which has well established categories such as person, organization, location, event, date/time expressions, measurements, and more. You may need to adapt this label space, expand, or constrain it, to fit the needs of the model you are working on. Likewise if you are working on tagging parts of synthetically generated speech for problems, you may develop a set of tags such as "pitch is too low", "duration is too long", "lacks aspiration", or "segments overlap", and you may consider how to define and adapt those tags for use by naive labelers.[^2]

To me, this is very much like theory development. You step into a new dataset that someone has collected; you spend some time exploring it, identifying generalizations and edge cases; you start experimenting with a proposal to explain the data; you may collect some more data where you think something might be missing or multiple hypotheses could be correct. You might use labels like "grammatical/ungrammatical" or "natural/unnatural". You may use labels like {CP, TP, vP, VP} or {epistemic, deontic, root, circumstantial, possibility}. If there's an existing label space that works, you may use it and just refine the definitions, hierarchies, or relations. If there's a portion of the data that isn't explained, you may define a new label or redefine the entire (or a part of the) existing label space. You might argue that what you're seeing actually isn't a modal at all, but an evidential. That the language you're looking at motivates a new type of phase. That the pronoun in this Austronesian language is really a logophor, but we have to redefine what logophors are so they apply not only to more common ones found in African language but also to these new ones you just discovered. 

The ability of linguists to take a messy, unstructured dataset, and impose structure on it, to identify what is relevant and what is not, to iterate and refine the definitions, to find the edge cases, generalizations, and exceptions, is a rare and very useful skill.


## Interlude 

The three sections above --- designing annotation projects, creating annotation guidelines, creating taxonomies --- are interrelated. We might often engage in all three at once as part of our job. But sometimes you do just one but not the others: you're given an existing taxonomy and the best you can do is add some examples but you can't really change the labels or definitions because they've been used for a long time and there are existing dependencies. Or you're given a project design and you're asked to write the guidelines. Or you design the project and work with a team of trainers/writers whose job is to work with the crowds. Linguists are frequently employed in all these types of jobs. 

## Designing an evaluation *is like* writing problem sets

**Model evaluation** is the process of systematically assessing how well a model performs on defined tasks using representative test data and appropriate metrics, in order to measure accuracy, robustness, and whether the model meets its intended objectives and real-world requirements. An evaluation is designed by first clearly defining the task and success criteria, including what behaviors or outcomes the model should exhibit. Appropriate metrics and benchmarks are then selected to measure those goals, along with a representative and well-controlled dataset that reflects real-world use cases and edge cases. Finally, evaluation protocols are specified---such as data splits, baselines, and error analysis methods---to ensure results are reliable, interpretable, and actionable.

There are various parts of this work that are similar to the work of a linguist, in particular when designing a problem set or an exam to assess the training and knowledge of students. 

<div class="compact-list">
1. Translate high-level goals into clear tasks, success criteria, and measurable outcomes
   - determine which metrics are appropriate, what they capture, and trade-offs
   - understand what “good” performance looks like for the task
2. Select or construct representative evaluation datasets
   - include core cases, edge cases, and known failure modes
   - ensure consistency, reproducibility, and correctness in datasets and metrics
3. Interpret results, identify patterns in errors, and distinguish signal from noise (see [error analysis](#doing-error-analysis-is-like-doing-linguistic-analysis) below)
4. Clearly communicate evaluation design, results, limitations, and implications to stakeholders
</div>

One important aspect of evaluating a model is the design of the evaluation dataset: to perform an evaluation, we must construct or select a dataset that would allow us to measure the right metrics for our model. This **golden dataset** will have highly confident labels, which can then be compared to model predictions and errors can be analyzed. We may select an existing, external *benchmark* dataset, which will allow us to compare ourselves to other models on a leaderboard; or we may design a dataset to specifically target our model and data needs, for example focusing on the most common user experiences expected for the model, perhaps even using customer data, if available. My own work often involves the design and construction (and localization) of targeted datasets.

Hand in hand with dataset(s) design, we also define what **metrics** to measure and report. We may compute some common ML metrics such as *precision*, *recall*, and *F1*, as well as task-specific metrics such as *word error rate*, *BLEU score*, *perplexity*, *human preference rate*, *R^2*, *Mean Absolute Error*, etc. We might also use metrics with customizable, often complex definitions, such as *helpfulness rate* and *harmfulness rate*. Metrics can be as tailored as needed, and defined to fit specific internal needs. They may also vary by task or dataset --- for example, what would be considered a "helpful" virtual assistant might be different from a "helpful" search algorithm. And different companies may set different definitions for what they consider "helpful" for their own virtual assistant, for example, which may differ from direct competitors.

The design of a golden dataset is similar to the design of a problem set for an exam or homework assignment. We select data that we think is representative of the knowledge or behavior we want to test. We ensure we cover the breadth of the concepts we are interested in, including both easy, center-of-the-distribution cases, as well as difficult, edge cases. We also develop a solution guide that contains the right answers. We further decide how to score the solution: some errors will be more costly than others. We decide how to deal with recurring or cascading errors. 

Finally, we may report outcomes, provide feedback, and generate **insights** from the solutions we have received. A TA might want to report back to an instructor about unclear concepts, or make suggestions about how to teach something differently, add examples, add more exercises, change the order of presentation of materials, etc. Students might be presented with feedback that highlights their errors and makes suggestions for what to focus on to improve. And through the course of doing this work, we may also discover errors in our own work: maybe we weren't as clear in our task definitions as we thought; maybe actually some of our golden labels are wrong; maybe our study materials (guidelines, existing training data) don't cover some cases that came up in the task. We'll communicate our findings differently depending on what how we diagnose the problems.


## Doing error analysis *is like* doing linguistic analysis

One important aspect of doing an evaluation is **error analysis**: the systematic process of examining a model's mistakes to understand why errors occur, identify patterns or edge cases, and uncover weaknesses in the model, data, or annotation. The results of error analysis inform improvements in data quality, model design, annotation guidelines, or evaluation metrics to guide more effective iterations. 

The skills involved in this task are, once again, very relevant to the linguist's life and work: 

<div class="compact-list">
1. Define **scope and goals**
   - specify the model, data, and types of errors to analyze
2. **Identify and organize** incorrect predictions
   - group mistakes by type, feature, or context
   - diagnose **root causes**: determine if errors arise from data, model, or ambiguity
   - measure pattern **frequency and impact** to prioritize improvements
3. Focus on the most frequent or high-impact errors
4. Apply changes, re-evaluate, and track progress over time
</div>

This work is quite similar to how I approach solving a problem set or doing linguistic analysis. I often adopt a bottom-up approach: (a) start from specific interesting datapoints, (b) form a hypothesis about why they are behaving a certain way, (c) test my hypothesis with more data, (d) iterate until I have a proposal. If I'm developing a theory, I'll want to refine my definitions and proposal to account for all the data, and test again to ensure that I'm now able to explain all my data. When I encounter outliers or edge cases, I consider different reasons why things look odd. Maybe my gloss is wrong. Maybe the sentence is actually ambiguous and my speaker got a different reading than I intended. Maybe I suspect a participant in my experiment found some way to cheat and I should exclude all data from them. Maybe my theory is wrong.

In the context of model evaluation, when I do error analysis, I consider several sources for errors in model performance. Some errors may be traced back to annotator error, which I may then trace back to gaps in the guidelines, conflicting examples, confusing definitions, poor task design, inadequate training, or laziness of annotators. We might then fix our golden labels and also iterate on our design and definitions, as needed. Some errors may be due to ambiguity in our taxonomy definitions. Other errors might be due to model performance, which we may then trace back to gaps or skews in training data, ambiguity or confusion in how the model prompt was written, limitations in the model architecture, insufficient fine-tuning, or unexpected edge cases in the input data. If this is the issue, we might engage in some prompt optimization (aka prompt engineering), or we might audit our training data to decide if any changes are needed. We take both the frequency and severity of issues into account. Very mild and unlikely errors will garner less attention than major, frequent ones. 

## Data analysis *is like* data analysis

To state the obvious, if you perform data analysis on your experimental/computational results, you're doing the kind of analysis you might also do in a tech job. The most common language for data analysis in tech is *python*, whereas you might be more used to working in R in academia, but the concepts are the same. It's advisable to take the time to learn the basics of python syntax, so you can translate your skills into a more employable language. 

Likewise if you're building models, using neural nets, experimenting with LLMs, using other computational tools, those are skills that will be directly relevant to a tech job. 

&nbsp;

**Now it's your turn: What other skills should I add?**

&nbsp;

#### Notes

[^1]: [Here](hkotek.com/Baird-LEXING2026.pdf) is Maggie's original abstract as it appears on the LSA program (saved locally because LSA has a way of deleting or moving content around). Maggie is of course not responsible for any of the ideas I introduce here, but the credit for this idea is all hers. Her original proposal is: 
    - Training and Annotation IS LIKE Developing Elicitation Plans
    - Evaluation IS LIKE Writing Problem Sets
    - Error Analysis IS LIKE Doing Morphophonological Analysis

I've made quite a lot of changes to the first part. To me, designing annotation tasks is more like engaging in behavioral experimentation, where the goal is to teach a large set of naive participants to do the same thing, than elicitation, which is often 1:1 and involves an experimenter present in the room, unlike most annotation projects I work on.

[^2]: I totally just made this faux-phonetic label set up, and I'm not a p-side person, so please don't yell at me. 