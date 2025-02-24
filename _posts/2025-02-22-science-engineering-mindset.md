---
title: A Science vs Engineering mindset
layout: default
comments: true
permalink: /blog/science-engineering-mindset/
categories:
  - academia, altac, science, engineering, teamwork
tags:
  - academia, altac, 
---

I occasionally get asked variations on the common theme of "what are the biggest differences between Academia and Industry" or "what were some things you weren't expecting when you started your first industry job". While the latter is harder for me to remember clearly by now, the former is easier to answer. 

## An engineering mindset

The best way I am able to explain the main difference between industry and academia is as follows: 

> **If you have a theory that explains 98% of your data, but which fails to explain the remaining 2%, you unequivocally have the *wrong* theory. 
> On the other hand, if you have an engineering solution that covers 98% of use cases, but which fails to cover the remaining 2%, you probably have a *really great* solution.** 

Science and research often live in those small margins that differentiate one theory from the other. All of them will cover the "core" data pertaining to the relevant phenomenon of interest, and it's really not too interesting to spend time on them other than to show a baseline. The work is in those details, or in expanding the coverage to new cases and new details we didn't originally think about. 

My entire research program as a linguist focused on constructions that are incredibly rare in everyday usage, but where theories nonetheless make clear (and disparate) predictions. Those predictions allow us to distinguish one theory from another, and argue in favor or against prevailing theories---and perhaps also learn something deep about the underlying nature of Grammar in the process.[^1] 

Engineering work,[^5] on the other hand, often focuses on the major use cases the system is built for. There's always going to be a long tail of issues we may not cover with our general solution. But, (a) if it's not something anyone actually needs the system for, then who cares if it does something odd or just doesn't work? We may never "fix" those issues. And (b) if we do need to address these issues, we might just write some override, or special rule, to hard-code what we want the system to do, and call it a day. It's not ideal, but it works, and it doesn't make the general solution "bad" or "wrong".[^2] 

You may think that writing a list of exceptions means the system is obviously imperfect.[^3] On occasion, you can clearly point to how the solution doesn't align with scientific research. But imperfect doesn't necessarily mean wrong or bad. And pointing out that the solution doesn't align with Theory or (in the case of Language Models) *isn't how people do it* isn't usually helpful. It might get you marked as someone who doesn't prioritize the right things.

This is absolutely not to say that there is no room for insights from scientific research in industry. But **you have to learn how to pick your battles**, and you have to demonstrate how the research insights will practically support the engineering work that you are doing.[^4] You also have to learn how to speak to the non-specialists in a way that they can understand and relate to. If you can do this, I promise you'll be a rockstar! 


## Team work makes the dream work

Here's one more difference that's worth pointing out. In industry (specifically, in tech) **you always work in teams**. You bring your knowledge and expertise to a team of people who have distinct, sometimes overlapping expertise, but you don't all know all the same things  or have the same backgrounds. 

This helpfully means that ***you do not have to know (and do) All The Things***. It is fine and good to have someone help you do A Thing if you don't know how, but they do. For example, you shouldn't have to learn how to use a whole new system if you just need to use it once or twice. You shouldn't have to learn a new programming language to interact with a system that's generally peripheral to your job. There will be people around whose main job involves interacting with that system or language. There will be someone around who already knows how to understand the logs for that weird error you're facing. There will be people who already know what permissions you're missing to get That Thing to work. Often there will be people whose job is to schedule meetings or keep track of deadlines or submit reports or organize events, and so on. And likewise there will be things that you know how to do, but they don't. 

You should definitely learn the things that are key to your job. Sometimes you'll want to expand your skills and learn something that's technically outside your job description but you encounter frequently (or are simply interested in), especially if you're often blocked by needing someone else to do it for you. But probably more frequently you don't need it. You want to learn to identify when you need to get someone else to support you, and also learn who those people are, and get that help when you need it. 

And when you *do* learn something new, likewise there's usually no reason to start from scratch. There will often be documentation around, or a training; or you can inherit code from someone else, or use their work as a starting point for yours. And you can ask questions when you get stuck and get someone to show you things. You really don't have to do it all alone. Working in teams is great, actually. 

## Lots of other things

There are lots of other things I could add here. Briefly: 
- **The general length of a project**. In industry, you won't really have a project that's multi-year or even multi-quarter that's not well-defined and periodically re-assessed and re-scoped. Your academic projects can easily stretch into years with no one checking in on you; I don't know that that's such a good thing, though.
- **Feedback loops**. In industry, you'll mostly get feedback from internal people who want your project to succeed. They will often also help you fix whatever issue they are pointing out. In academia, feedback is often slower and is mostly external, from reviewers who aren't at all invested in your success and who are often just trying to find what's wrong with your work. I really *really* hated the nature of feedback in academia.
- **Product orientation**. In industry, if you're not on a pure research team, it may be harder to do something just because it's interesting.
- **Being tied to the product release schedule**. A corollary of the above, though even for me that's not always been a constant. I've had roles that are more removed from the release cycle and ones that are very strongly tied to it.
- **Independence**. I have lots of it in industry, I had lots of it in academia. Not everyone will, and it's a big trope of why academia is better, but let's be honest here. There are money and other practical considerations on both sides.

I can immediately think of 5 other things to add, but I think I'll stop here. 


&nbsp;

*As always on this blog, this is a very tech-centric perspective. It's also a very theoretical linguistics/social science perspective. Your Mileage May Vary.*

&nbsp;


#### Notes

[^1]: For example, multiple *wh*-questions that may be superiority-obeying or violating, and may or may not also contain an intervener ("which book didn't which student read?"). Or dispreferred readings of quantified statements ("most of the circles are blue" meaning something like "there are more blue circles than any other color, but perhaps less than 50% in total"). Given that they are generally super uncommon sentences, but people still have surprisingly consistent intuitions that you can bring out in a variety of experiments or in careful elicitation, you can learn quite a lot about Grammar by closely studying these judgment patterns.   
[^2]: One way in which it *may* be bad is if those exceptions disproportionately affect a particular group of users, or use cases that are commonly used by some group but not others. For example, if your system inherently works for white men better than it does for Black women, you should fix that in a comprehensive way, not using some patchwork. (If you got as far as identifying that's a problem and are using some manual fix in the meantime, you're probably already thinking ahead and are aware of potential obstacles to redoing the system as a whole, so I do acknowledge that those patches are not all bad, either.)
[^3]: In fact, at some point if there are too many of these exceptions, especially if they become contradictory or unmanageable, or if you are using them to patch over systemic biases, that may be a strong argument for redoing the system. (The very legit counter-argument always being "why mess with something that's already working?") All the same, the mere existence of some overrides doesn't make a system bad. 
[^4]: I'd be willing to bet my lunch money that the famous Fred Jelinek quote "Every time I fire a linguist, the performance of the speech recognizer goes up" is the result of him working with a small set of linguists who weren't picking the right battles. 
[^5]: I should probably write a whole post about what "engineering work" means in this context. It has a much broader definition than you might think, and it will probably apply to most work a linguist in tech will be doing. 

