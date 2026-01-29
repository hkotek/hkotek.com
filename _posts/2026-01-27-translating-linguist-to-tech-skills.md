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
  - tech
---

There were several excellent presentations at this year's [**LEXING**](https://www.lsadc.org/lexing). In a talk titled *Linguists are Exceptional Inductive Reasoners – A Case Study on Skill Relevance in Enterprise Software*, [**Maggie Baird**](https://www.linkedin.com/in/maggie-baird-167129102/) laid out a mapping between her everyday work as a linguist on an engineering team developing a generative AI product and three tasks commonly carried out by academic linguists. It resonated with me --- it's also very true of my job and skills. In this post, I spell out my version of Maggie's ideas.[^1] 

The gist: \<tech skill\> is like \<linguist skill\>
- [Designing annotation projects *is like* designing human subjects studies](#designing-annotation-projects-is-like-designing-human-subjects-studies)
- [Training annotators *is like* writing experiment guidelines](#training-annotators-is-like-writing-experiment-guidelines)
- [Creating a taxonomy *is like* developing a linguistic theory](#creating-a-taxonomy-is-like-developing-a-linguistic-theory)
- [Designing an evaluation *is like* writing problem sets](#designing-an-evaluation-is-like-writing-problem-sets)
- [Doing error analysis *is like* doing linguistic analysis](#doing-error-analysis-is-like-doing-linguistic-analysis)
- [Doing data analysis *is like* doing data analysis](#doing-data-analysis-is-like-doing-data-analysis)
- [More X *is like* Y](#more-x-is-like-y)


Also check out [**this companion piece**](https://hkotek.com/blog/what-is-annotation-taxonomy/), which describes in more detail what I mean by concepts like "annotation", "guidelines", "taxonomy", "evaluation", "error analysis". Each post can be read as a standalone, but I also cross-link between the corresponding sections of both posts, for easier navigation. 

## Designing annotation projects *is like* designing human subjects studies

Linguists in tech companies often work on [**data annotation projects**](https://hkotek.com/blog/what-is-annotation-taxonomy#data-annotation-projects/) in various capacities and at different part of the process. The skills associated with this kind of work are similar to the skills used in **experimental study design**.

<style>
.compact-list ol {
  padding-left: 1em;       /* reduce number indent */
  margin: 0;               /* remove extra vertical spacing */
  list-style-position: inside; /* numbers flush with text */
}

.compact-list ol li {
  margin: 0; 
  padding: 0;
}

.compact-list ol li ul {
  margin: 0; 
  padding-left: 0.8em;     /* nested bullets closer to number */
}
</style>

<div class="compact-list">
  <ol>
    <li>Understand project goals: what the data will be used for, how, and by whom</li>
    <li><strong>Operationalize</strong> the problem:
      <ul>
        <li>define label space (see <a href="#creating-a-taxonomy-is-like-developing-a-linguistic-theory">taxonomy</a> below)</li>
        <li>decide on the number of datapoints per label</li>
        <li>identify data sources</li>
        <li>sample/compile data</li>
      </ul>
    </li>
    <li><strong>Design</strong> the project:
      <ul>
        <li>simple to teach to large/untrained annotators</li>
        <li>ensures consistent, accurate data collection</li>
        <li>fits budget and timing constraints</li>
      </ul>
    </li>
    <li>Create the project in your <strong>tool</strong>:
      <ul>
        <li>visual design elements</li>
        <li>minimize effort via spatial layout</li>
        <li>ordering of items</li>
        <li>allow annotators to change previous answers?</li>
      </ul>
    </li>
    <li>Identify <strong>annotator skills</strong>:
      <ul>
        <li>write guidelines (see <a href="#training-annotators-is-like-writing-experiment-guidelines">training annotators</a> below)</li>
        <li>create practice items</li>
        <li>set minimum participation requirements (language, age, region, accuracy, ...)</li>
        <li>define appropriate compensation</li>
      </ul>
    </li>
  </ol>
</div>


Linguists who engage in **elicitation work**, **ethnographic work**, **corpus work**, or **formal theoretical work** also engage in at least part of this process. Really, any scientifically driven exploration will require operationalizing a problem and determining an appropriate label space, perhaps also recruitment of participants and setting of a task and payment. They differ in that these tasks often happen with the experimenter in the room or in a small group setting (or with the experimenter being the only person in the room), whereas larger studies such as annotation projects most often involve naive workers who experimenters have a limited ability to train or provide feedback to. 

I believe this is the most direct skillset I took with me from my academic work into my industry job. I want to stress in particular the earlier ideation parts: *understand the goals of the project* -- projects in my industry job are frequently initiated by external needs of other engineering groups. The work of clearly defining what the goal of the project is and how the data will be used is key, and is something that in my experience a lot of engineers struggle with, both in explaining in words what they need and in being able to generalize beyond 1-2 examples they have in their heads. Finding generalizations, edge cases, the right examples, and the right categories to use, are all things linguists excel at.  


## Training annotators *is like* writing experiment guidelines

The data annotation projects described [above](#designing-annotation-projects-is-like-designing-human-subjects-studies) are often staffed by 3rd party workers of some kind. Crowds will often be large and non-specialist, and therefore require [**guidelines**](https://hkotek.com/blog/what-is-annotation-taxonomy#annotation-guidelines/) and perhaps **practice items** along with the task. Guidelines ensure a basic understanding of the project; good guidelines will describe the tool and steps involved in the task, define concepts and labels, answer frequently asked question, and provide some examples of how to use the labels in the context of the task. 

A key goal of the guidelines is to ensure that a large crowd will be able to perform the same task consistently and correctly. The more complex the task, the more noise in the data. Noisy and conflicting data will reduce the likelihood an ML model will be able to learn the correct generalizations from the data. Garbage in, Garbage out. 

The skills associated with this kind of work are again similar to the skills used in **writing instructions for experimental studies**:

1. Understand the **technical goals** of the project
2. Communicate the goals to a **non-technical audience**
3. Identify key concepts and skill-appropriate **definitions**
4. Provide a comprehensive set of **examples** to support generalization

The creation of annotation project guidelines is also similar to the prep work needed for **elicitation studies**, to ensure the right content and form of communication with consultants, as well as careful task design to ensure maximal likelihood of yielding usable results, as discussed in the previous section [above](#designing-annotation-projects-is-like-designing-human-subjects-studies). 


## Creating a taxonomy *is like* developing a linguistic theory

A [**taxonomy**](https://hkotek.com/blog/what-is-annotation-taxonomy#taxonomy-design/), or **ontology**, is a structured framework that defines the categories, labels, and relationships used to annotate data. Linguists are often hired as taxonomists, and though they may initially be confused about why we are considered so appropriate for this role, I think our training and disposition gives us an excellent preparation for this kind of work. Specifically, our comfort with **abstract thinking** comes in very handy. 

<div class="compact-list">
  <ol>
    <li> Understand how annotated data will be used< in training and evaluation.</li>
    <li> Break complex data into clear <strong>categories, hierarchies, and relationships</strong>.</li>
    <li> Write clear, unambiguous <strong>definitions</strong> that annotators (and models) can interpret consistently.
      <ul>
        <li>understand how annotators actually apply labels (and how models learn them); balance theoretical neatness with practical usability</li>
        <li>handle edge cases, overlaps, and exceptions</li>
        <li>refine labels to reduce ambiguity and noise</li>
        <li>iterate, test, and evolve taxonomies based on feedback</li>
      </ul>
    </li>
    <li> Maintain <strong>documentation</strong>, change logs, and versioning to keep the taxonomy stable and auditable.</li>
  </ol>
</div>

To me, this is very much like theory development. You step into a new dataset that someone has collected; you spend some time exploring it, identifying generalizations and edge cases; you start experimenting with a proposal to explain the data; you may collect some more data where you think something might be missing or multiple hypotheses could be correct. You might use labels like "grammatical/ungrammatical" or "natural/unnatural". You may use labels like {CP, TP, vP, VP} or {epistemic, deontic, root, circumstantial, possibility}. If there's an existing label space that works, you may use it and just refine the definitions, hierarchies, or relations. If there's a portion of the data that isn't explained, you may define a new label or redefine the entire (or a part of the) existing label space. You might argue that what you're seeing actually isn't a modal at all, but an evidential. That the language you're looking at motivates a new type of phase. That the pronoun in this Austronesian language is really a logophor, but we have to redefine what logophors are so they apply not only to more common ones found in African language but also to these new ones you just discovered. 

The ability of linguists to take a messy, unstructured dataset, and impose structure on it, to identify what is relevant and what is not, to iterate and refine the definitions, to find the edge cases, generalizations, and exceptions, is a rare and very useful skill.


## Interlude 

The three sections above --- designing annotation projects, creating annotation guidelines, creating taxonomies --- are interrelated. We might often engage in all three at once as part of our job. But sometimes you do just one but not the others: you're given an existing taxonomy and the best you can do is add some examples but you can't really change the labels or definitions because they've been used for a long time and there are existing dependencies. Or you're given a project design and you're asked to write the guidelines. Or you design the project and work with a team of trainers/writers whose job is to work with the crowds. Linguists are frequently employed in all these types of jobs. I wrote a bit more about all three in [**this related post**](https://hkotek.com/blog/what-is-annotation-taxonomy/).


## Designing an evaluation *is like* writing problem sets

[**Model evaluation**](https://hkotek.com/blog/what-is-annotation-taxonomy#evaluation-design/) is the process of systematically assessing how well a model performs on defined tasks using representative test data and appropriate metrics, in order to measure accuracy, robustness, and whether the model meets its intended objectives and real-world requirements. An evaluation is designed by first clearly defining the task and success criteria, including what behaviors or outcomes the model should exhibit. Appropriate metrics are then selected to measure those goals, along with representative and well-controlled datasets that reflect real-world use cases and edge cases. Finally, evaluation protocols are specified---such as data splits, baselines, and error analysis methods---to ensure results are reliable, interpretable, and actionable.

There are various parts of this work that are similar to the work of a linguist, in particular when designing a problem set or an exam to assess the training and knowledge of students. 

<div class="compact-list">
  <ol>
    <li>Translate high-level goals into clear tasks, success criteria, and <strong>measurable outcomes</strong>
      <ul>
        <li>determine which metrics are appropriate, what they capture, and trade-offs</li>
        <li>understand what “good” performance looks like for the task</li>
      </ul>
    </li>
    <li>Select or construct representative <strong>evaluation datasets</strong>
      <ul>
        <li>include core cases, edge cases, and known failure modes</li>
        <li>ensure consistency, reproducibility, and correctness in datasets and metrics</li>
      </ul>
    </li>
    <li><strong>Interpret results</strong>, identify patterns in errors, and distinguish signal from noise (see <a href="#doing-error-analysis-is-like-doing-linguistic-analysis">error analysis</a> below)</li>
    <li>Clearly <strong>communicate</strong> evaluation design, results, limitations, and implications to stakeholders</li>
  </ol>
</div>

The design of an evaluation dataset and evaluation metrics is similar to the design of a problem set for an exam or homework assignment. We select data that we think is representative of the knowledge or behavior we want to test. We ensure we cover the breadth of the concepts we are interested in, including both easy, center-of-the-distribution cases, as well as difficult, edge cases. We also develop a solution guide that contains the right answers. We further decide how to score the solution: some errors will be more costly than others. We decide how to deal with recurring or cascading errors. We decide on a grade based on all of this. 

Finally, we may generate additional **insights** from the solutions we have received. A TA might want to report back to an instructor about unclear concepts, or make suggestions about how to teach something differently, add examples, add more exercises, change the order of presentation of materials, etc. We may also discover errors in our own work: maybe we weren't as clear in our assignment definitions as we thought; maybe actually some part of our solution was wrong; maybe our study materials don't cover some cases that came up in the task, and we should fix that for the next time we use the assignment. 



## Doing error analysis *is like* doing linguistic analysis

One important aspect of doing an evaluation is [**error analysis**](https://hkotek.com/blog/what-is-annotation-taxonomy#error-analysis/): the systematic process of examining a model's mistakes to understand why errors occur, identify patterns or edge cases, and uncover weaknesses in the model, data, or annotation. The results of error analysis inform improvements in data quality, model design, annotation guidelines, or evaluation metrics to guide more effective iterations. 

The skills involved in this task are, once again, very relevant to the linguist's life and work: 

<div class="compact-list">
  <ol>
    <li>Define <strong>scope and goals</strong>
      <ul>
        <li>specify the data, sources, and types of errors to analyze</li>
      </ul>
    </li>
    <li><strong>Identify and organize</strong> incorrect predictions
      <ul>
        <li>group mistakes by type, feature, or context</li>
        <li>diagnose <strong>root causes</strong>: e.g. determine if errors arise from data, model, or ambiguity</li>
        <li>measure pattern <strong>frequency and impact</strong> to prioritize improvements</li>
      </ul>
    </li>
    <li>Focus on the most frequent or high-impact errors</li>
    <li>Apply changes, re-evaluate, and track progress over time</li>
  </ol>
</div>

This work is quite similar to how I approach solving a problem set or doing linguistic analysis. I often adopt a bottom-up approach: (a) start from specific interesting datapoints, (b) form a hypothesis about why they are behaving a certain way, (c) test my hypothesis with more data, (d) iterate until I have a proposal. If I'm developing a theory, I'll want to refine my definitions and proposal to account for all the data, and test again to ensure that I'm now able to explain all my data. When I encounter outliers or edge cases, I consider different reasons why things look odd. Maybe my gloss is wrong. Maybe the sentence is actually ambiguous and my speaker got a different reading than I intended. Maybe I suspect a participant in my experiment found some way to cheat and I should exclude all data from them. Maybe my theory is wrong.


## Doing data analysis *is like* doing data analysis

To state the obvious, if you perform **data analysis** on your experimental/computational results, you're doing the kind of analysis you might also do in a tech job. The most common language for data analysis in tech is *python*, whereas you might be more used to working in R in academia, but the concepts are the same. It's advisable to take the time to learn the basics of python syntax, so you can translate your skills into a more employable language. 

Likewise if you're building **computational models**, using neural nets, experimenting with LLMs, using other computational tools, those are skills that will be directly relevant to a tech job. 


## More X *is like* Y

There are some parts of my job that I can sort of liken to stuff as I used to do as a linguist, maybe stretching it a little. 

1. **Abstract writing** is like the little project proposals I've written to get intern headcount.[^3]
3. **White papers** are like policy docs. I've had the chance to write some policy documentation in my job, mainly asking questions in the safety space ("what *should* an LLM do in Context A?"). Maybe you've written similar documents for your department, e.g. around how data from Native American or other speaker communities should be preserved and used; or how students in your department should be taught, etc.
2. **Budget management** is like budget management. If you do things like review and approve hours for a lab manager or plan a budget to pay for your data collection needs, that's something you may do in your tech job, too.
4. **Making a weekly lesson plan in your syllabus** is kinda like planning your project for the quarter. We tend to work in 2-week sprints that are much better defined, and we are constrained by external, sometimes not known and sometimes changing, deadlines. We may go through replans in the middle of the quarter to account for changing needs. But the general gist kinda works, maybe. 


## One last word

Notice one thing you did not hear me say here: **for the most part, the actual *content* and *topic* of your research do not matter**. Whether you're a syntactician who works on noun classes in Bantu or a semanticist who works on modality in West Greenlandic, or a phonologist who works on tone sandhi in ancient Thai, it's all the same if you're a theoretician, or an experimentalist, or a modeling person, or corpus person, etc. The level of abstraction I think is relevant is the tools and skills you use, not the specific content of your research. 

Corollary: likely, no one is going to care about the specific findings in your publications, or what your dissertation is about, etc. You may very well be asked to describe your research in an interview, and you should work to find the right level of detail to share (hint: less is more). But beyond that, it's very likely that your job will have a different subject matter and focus than anything you did before, and you'll learn that as you onboard and work on the team. 

&nbsp;

**Now it's your turn: What other skills should I add?**

&nbsp;

#### Notes

[^1]: [Here](hkotek.com/Baird-LEXING2026.pdf) is Maggie's original abstract as it appears on the LSA program (saved locally because LSA has a way of deleting or moving content around). Maggie is of course not responsible for any of the ideas I introduce here, but the credit for this idea is all hers. Her original proposal is: 
    - Training and Annotation IS LIKE Developing Elicitation Plans
    - Evaluation IS LIKE Writing Problem Sets
    - Error Analysis IS LIKE Doing Morphophonological Analysis
    
    I've made quite a lot of changes to the first part. To me, designing annotation tasks is more like engaging in behavioral experimentation, where the goal is to teach a large set of naive participants to do the same thing, than elicitation, which is often 1:1 and involves an experimenter present in the room, unlike most annotation projects I work on.

[^3]: Initially I thought about grant writing here, but I don't think I ever write documents that are quite that long or scrutinized. 