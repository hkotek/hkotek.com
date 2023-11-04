---
title: Placeholder title
layout: default
comments: true
permalink: /blog/temp/
categories:
  - gender, bias
tags:
  - gender, bias
---

For my [seminar on Demystifying LLMs](https://linguistics.mit.edu/24-s90-special-topics_exploring_language_technologies/) we've been thinking about what we can learn from Large Langauge Models (LLMs) about language or linguistics. So far the answer seems to be 'not too much', though I've been hoping to find effects that could meaningfully inform our theories. On the other hand, it's really not hard to find interesting effects with regard to hallucinations, bias, toxicity, misinformation, disinformation, etc., which teach us something deep and fundamental about the datasets the models are trained on.  

We recently explored multi-modal text-to-image models in class, specifically [DALL·E 2](https://openai.com/dall-e-2) and [Stable Diffusion XL](https://stablediffusionweb.com/).[^1] I was initially interested in whether there would be anything interesting to learn about how these models process language (spoiler: not much, but I'll say more below). It quickly became clear that it's much more interesting to think about ethics considerations with respect to these models. 

## Language understanding in text-to-image models
 
I was thinking it'd be interesting to think about how the models would deal with things like lexical ambiguity, structural ambiguity, vagueness, gibberish. The short version: it seems to me that the model isn't doing much beyond picking out the nouns and using their most common interpretation. 

For example, here is a side-by-side of "red apples and oranges" and "red oranges and apples": 
<img src="https://hkotek.com/stable_diffusion/red-apples-oranges" width="80%" />
<img src="https://hkotek.com/stable_diffusion/red-oranges-apples" width="80%" />

And here's "red apples and peppers" and "red peppers and apples"
<img src="https://hkotek.com/stable_diffusion/red-apples-peppers" width="80%" />
<img src="https://hkotek.com/stable_diffusion/red-peppers-apples" width="80%" />

These are simple examples of syntactic "bracketing" ambiguities: on one interpretation, "red" modifies the complex noun phrase while on the other "red" modifies the first noun alone: 
- red [oranges and apples]  //  red [apples and oranges]
- [red oranges] and apples // [red apples] and oranges

In the case of "red oranges and apples", on either bracketing, the oranges have got to be red, no way around it. For "red apples and oranges", there is a more sensible parse (only the apples are red) and a less sensible one (both fruit are red), so you'd expect to see the more sensible one given the likely training data. Nonetheless, we don't really see a difference. That led me to try "apples and peppers", since both can be red (or green), so I wondered if there'd be a difference there, but not really. 


 

I've written before about [**Gender bias and stereotypes in Large Language Models**](https://arxiv.org/abs/2308.14921), and I have some other related work on intersectional bias and on sensitive questions.   


&nbsp;

[^1]: Most the images included in this post were generated on October 30-31, 2023 on the free web version of Stable Diffusion XL. I tried some of the same prompts with Dall-E but ran out of free tokens. The observations I make here seemed to apply to Dall-E too, but I had much less data to work with so there may be other things I missed because of the limited prompts I could try. 