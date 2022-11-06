---
title: Interview questions
layout: default
comments: false
permalink: /blog/academic-interview-questions/
categories:
  - academia, interviews
tags:
  - academia, interviews, jobs, long-list, short-list, linguistics, syntax, semantics
---

<script src="/js/zepto.min.js"></script>
<script>
Zepto(function($){
	$('a').each(function(i,dt){
		var that = $(this);

		if (that.text() != 'expand >>')
			return;
		
		// for anchors that have text 'expand >>':

		var par = that.closest('p');
		var desc = par.next();
		
		while (desc.last().next().length && !desc.last().next('h1,h2,h3').length) {
			desc.push(desc.last().next());
		}
	
		that
		.attr('href','#')
		.on('click', function() {
			desc.toggle();
			return false;
		});
		
		desc.toggle();
	});
});
</script>

Between 2014 and 2019 I went on the North American academic job market for 6(!) cycles. I applied broadly to jobs in theoretical syntax and semantics, experimental/psycholinguistics, SLACs as well as research institutions. I also applied to a handful of jobs in Europe and the UK. I had quite a bit of success, with a total of 29 long-lists and 12 short-lists. I have written separately about [**my experiences on the job market**](\my-academic-journey); I have a lot to say.

Me being me, I took contemporaneous notes from the majority of interviews I did. I've been sitting on them for years and I've finally decided I should just put them out there for others to use. The academic job market is an absolute horror show (again, the topic of another post), and if this can help at least *someone* not feel so overwhelmed, I will count that as a great success. 

Below are 26 distinct lists. I don't provide the names of institutions but instead summarize the type of job and department. I've collapsed the lists so the main page is manageable, but you can click on each list to expand the questions. In the majority of cases the questions are paraphrases rather than verbatim what was asked, since I took notes after the fact. 


Short list questions
--------------------



Long list questions
-------------------

### Long-list interview with for a TT job in semantics [**expand >>**]()

  - current/future plans
  - teaching: what all can you teach? (give full list)
  - how would you teach UG semantics?
  - how about grad semantics?
  - questions about one of my published papers
  - questions about a choice I made in my teaching demo
  - what are your strengths and weaknesses (by teaching, research, service)
  - how do you fit with department
  - work on endangered languages
  - what course would you teach that philosophy majors might take
  - living in CITY (fit)
  - what are your hobbies
  - questions for us


### Long-list interview with a UK-based university for a lecturer (TT-equivalent) job in psycholinguistics [**expand >>**]()

  - Why SCHOOL
  - What research overlap do you have with other faculty
  - What methods do you know, how did you learn them?
  - What can you teach of those techniques?
  - What do you consider to be your most important paper
  - What course would you propose for undergrads
    - How to come up with topics
  - Conversion MA students with no background have 6 months for a project; how would you help them choose a topic? 
  - Questions for us

