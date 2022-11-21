---
title: Alt-Ac informational interview questions
layout: default
comments: false
permalink: /blog/altac-informational-interview-questions/
categories:
  - academia, interviews
tags:
  - altac, interviews, jobs, tech, prepping
---

<script src="/js/zepto.min.js"></script>
<script>
Zepto(function($){
	$('a').each(function(i,dt){
		var that = $(this);

		if (!that.text().match(/^expand/))
			return;
		
		// for anchors that have text 'expand >>':

		var par = that.closest('h3');
		var desc = par.next();
		
//		while (desc.last().next().length && !desc.last().next('h1,h2,h3').length) {
//			desc.push(desc.last().next());
//		}
	
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


Exploring non-academic career paths can be daunting. There is so much out there, and at the same time where to even start. Other than reading posts such as this one, one key thing you can do to get started on your path is to conduct informational interviews. 

## What are informational interviews 

Informational interviews are informal chats with people of interest. They allow you to learn more about a person's role, career trajectory, or a company or industry that interests you. The goal of the chat is to conduct research --- *not* to apply for or ask for a job. Because they are chats that occur outside of an official job interview process, they can be more relaxed and allow you to ease into the habit of speaking to people in your prospective new industry and using the relevant terminology. 

## Who should I interview

You can interview anyone with a potentially interesting career path, and or anyone with a similar background to yours. You can find them through various networks: your school's alumni network, friends or family, former colleagues you met at conferences or other events, social media lists or groups, or even randomly on LinkedIn by searching relevant keywords. 

You don't necessarily need or want to speak to senior people in your intended field. You might get more time and attention from folks who have just recently started their careers. It is interesting and beneficial to hear the perspective of experienced leaders, but it is also important to hear from those who just recently got started and are doing work that is likely to be similar to what your first job might be like. 

Once you start conducting interviews, one key way you'll find new people to interview will be by asking your current interviewee if they know anyone else they can connect you with. 

## How should I prep

A lot of people are generous with their time. But to make maximal use of this time, and to leave them with a feeling that their time is valued, you should do some prep work. Spend a bit of time learning about the person through their public facing content, be it on LinkedIn, a private website, or social media. What is the person doing currently? Do they list a job title and short job description on a resume somewhere? Where did they go to school, what for, and when? Where are they located? Who do they work for? What previous jobs have they held? 

Use this information to prepare some questions ahead of time, and tailor the questions to the circumstances. For example, only people with certain types of experiences can answer questions about being an immigrant; and it might make less sense to ask someone about their experience getting their first job if it was 20 years ago -- it might be better to focus on recent experiences and/or how they approach career growth or hiring. 

You can also use this opportunity to practice some answers you will need to provide in job interviews as well: a short (2-3 minute) introduction to you background and relevant skills and what kind of job you're looking for, and a short explanation of what your academic field is ("e.g. what does a linguist do?", "why should we hire linguists into [Role]?").

## How long should an interview be

A typical meeting in the tech industry is 30 minutes long. I would suggest limiting your request to that, or less if you think that is sufficient. Spend just a short bit of time introducing yourself (you should have already done this in the email/DM requesting the interview), and make sure to lead with the questions that are most of interest. An interviewee may invite you to speak for longer than the intended time slot, but don't assume that will happen. So, be strategic about the structure of your questions. 

## What should I ask

As part of a *careers for linguists* workshop I've been teaching, we have developed a long set of questions I will reproduce below. We tweak the questions and pick just a subset every time we host an external speaker, to match the speaker's background and experience. I've organized these questions by topic, with a list of questions collapsed under the header which you can expand: 

A useful conversation starter: Tell me about yourself and what you do

### Questions about skills [**expand >>**]()
    * What skill(s) do you use most often in your (current or previous) job?
    * What kinds of knowledge/skills from your linguistic/academic training do you find useful in your job?
    * Are there specific skills you expect a new hire can learn on the job vs skills they definitely need to have before they apply for jobs in your area? 
    * How can teaching skills (and the love for teaching) be used in industry?

### Questions about the day-to-day in the job [**expand >>**]()
    * What does a typical week in your job look like? How much time do you spend in meetings? How much focus time do you get for core tasks? 
    * What tasks do you do? 
    * Whom do you talk to/report to on a regular basis? 
    * How collaborative is your job? 
    * What do you appreciate about your job and what do you wish could be different?
    * If your position is a research one, do you think that your results are also meaningful “for the theory” or only for practical implementation? 
    * Do your responsibilities include publishing? Is maintaining an academic presence a part of your job and/or is encouraged/supported by your employer? 
    * What was the most surprising or unexpected thing about transitioning out of academia? 
    * How do you feel about your workload and work-life balance in your company?
    * How has the remote / in-person landscape changed during covid?

### Questions about prepping [**expand >>**]()

    * What do you suggest a student focus on if they have 2-3 more years in their program? What if they only have a few months or need to apply now? 
    * (Tailored version of the above:) I have [X amount of time] to devote to prepping. What would you suggest I spend my time on? 
    * If you could go back to your grad school days, what would you change about it? 
    * Do you have any advice on networking?
    * Any resume advice? How do you approach making your academic projects and skills clear and relevant for your non-academic role? 
    * (Tailored version of the above:) I have done project XYZ, how do I best portray it in applications/resumes to convey the relevant content to a potential employer? 
    * (Where relevant:) Do I need to have a portfolio (e.g. for UX design jobs)? Can you point me to examples online that you like?
    * Do you have a favorite resource for learning X? 

### Questions about applications and interviews [**expand >>**]()

    * How did you find the jobs you applied for? Where did you look? 
    * When do you recommend someone start applying for jobs in your field? How much time ahead of when they want to start the job should they start looking? 
    * What was the process that landed you your first job like? 
    * How long did it take? How many jobs did you apply for? Did you apply all over or strategically? Did you have a referral? 
    * What was the interview process for your first/most recent job like? 
    * What was the timeline like? Was there a technical component? Thinking back, what do you wish you knew at the time but didn’t?
    * What did you do well in your initial job search and what would you have done differently? 

### Questions for anyone involved in hiring [**expand >>**]()

    * What do you hire linguists/[insert your specialty here] for?
    * What are the main things that are important for you to see in an interview?
    * What is one thing you wish candidates knew? 
    * What are common mistakes you see candidates make? 
    * Does anybody look at your coursework when you apply?
    * How do you approach a candidate's materials? How long do you typically spend on them? Do you click on any links in a resume? Do you do an additional online search?

### Questions about immigration [**expand >>**]()

    * If you were/are an international person or if you hire such people, can you tell me about the immigration process as it relates to your job or field? 
    * How long did it take to you get a visa? Was it guaranteed? Did you use OPT or CPT? Does the company sponsor everything? 
    * Which companies are likely to support visa applications? How does planning/applying change under these circumstances? 
    * Does it make sense to apply for jobs not at FAANG companies if you’re international?

### Questions about career growth [**expand >>**]()

    * Do you think your previous job(s) determine your path? 
    * How easy would it be to change directions if you wanted to, and how would you do that?
    * Do you have a sense for what your next job or position might be? 
    * How do you know when is a good time to look for your next job? 
    * Are you focused on promotion or developing skills or getting into management or getting established in your current role or something else? 

### Questions about leaves and disability [**expand >>**]()

    * What does maternity/family support look like at your company? 
    * How are disabilities treated at your company/in your industry? 

### Questions about compensation [**expand >>**]()

    * How much would you expect a linguist/[insert your specialty here] on their first job to make in your field? (a range is fine.) 
    * What benefits or other components should they negotiate for or look for in their offer? 
    * Do you have advice for negotiating a first offer? 
    * Are there deal breakers for you in negotiations? 

A useful conversation ender: do you know anyone else [with relevant skills, title, background, etc.] who you could connect me with? 


## What should I *not* ask 

Try to avoid vague questions. For example: "what's a typical day like" -- a lot of people don't have a typical day, so instead you might try something like "what was your last week at work like?" or "how much time do you spend in meetings and other administrative tasks vs focused on work tasks". You might phrase this differently and expect different answers from someone who is more senior and manages people (they may spend more time in meetings and less doing individual work), or from someone who is a contractor or consultant (they likely spend most of their time on their own work). Also avoid directly asking for a job, though if it feels appropriate you may ask if the interviewee happens to know of any relevant jobs. 

In general, a good rule of thumb for any interview is to only ask questions that make your interviewee feel good about themselves and to not ask questions that are embarrassing or unpleasant. People generally like talking about themselves; but if you don't know someone well, maybe don't ask them about a recent experience of being laid off unless they bring it up. Likewise, be strategic about asking about the corporate atmosphere at a company if you don't know what to expect (and ask yourself, is this relevant -- i.e., are you applying for a job there, or is it just a curiosity). 

Finally, in my opinion it is not only acceptable but important to ask about compensation. Especially if you are a minority (a woman, first gen, Black, an immigrant, etc.), you may not have other ways to access to this kind of information, and lacking it may lead you to harm yourself in negotiations down the line. But be mindful of how you approach this. Some people get very uncomfortable when discussing money, so you may want to leave this to the end of the conversation, after you've established some rapport, and you may want to phrase it as a general question ("how much should one expect to make", "what is a reasonable range for a salary for a first job in this field", "what are generally the compensation components I should expect in an offer") to help your interviewee get over any hesitation. 
 

## Final thoughts 

After the interview is done, please remember to thank your interviewee for their time and insights. This is important for maintaining the connection you just established, and is especially important if you hope to ask them for a referral one day if a job at their company opens up. It is also important in order to support and maintain the community within the field you are trying to break into. 

And when you are on the other side, having obtained a job in your new chosen field, consider opening yourself up to be an interviewee in similar contexts, to help lighten the load on those who are already engaged in this work. Even as a newbie, you will have already gained experience in prepping, interviewing, and starting to learn about a new field. This knowledge could be invaluable to the next person behind you  who is still casting about trying to understand how to get started themselves. 