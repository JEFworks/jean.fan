---
layout: post
title: "Integrating LLM-Assisted Vibe Coding into the Classroom"
excerpt: "Like many computational professors, I've been fielding a lot of anxiety (from students and professors alike!) about AI replacing computational jobs. My response as a teacher: Try it. So this semester, I integrated LLM-assisted vibe coding into my upper-level undergraduate Genomic Data Visualization class. The outcome was surprisingly mixed. In this blog post, I reflect on what happened and how I plan to update the class in the future."
date: "March 15, 2026"
categories: [Commentary, Reflection, AI]
---

### Background

Like many computational professors, I've been fielding a lot of anxiety (from students and professors alike!) about AI replacing computational jobs. My response as a teacher: Ignorance is never an option. Try it out for yourself.

So this semester, I integrated LLM-assisted vibe coding into my upper-level undergraduate Genomic Data Visualization class. 

### Why This Class?

Genomic Data Visualization is an upper-level biomedical engineering course focused on teaching students the fundamentals of data visualization design, the mathematics of dimensionality reduction, and ultimately the critical thinking involved in interpreting high-dimensional biomedical data. We use coding, specifically in R, to apply what we learn to analyzing and communicating about spatially resolved omics data. 

But learning the mechanics of coding was never the central goal of the course; it's always been just the means to execute a design vision. I frankly don't care if students memorize ggplot2 syntax or theme() parameters. Students code to analyze complex biological data and render visualizations designed to communicate what they find. Coding was always just the vehicle, not the destination. 

So this seemed like an appropriate opportunity to introduce some AI augmentation, specifically through the use of LLMs-assisted vibe coding. 


### How I Structured The Class

The class has always been split into 2 parts per lesson: the first part is lecture about theory, and the second is the hands-on coding component to execute on the theory. During hands-on coding component, I live code and students follow along. 

But this year, during the hands-on coding component, I also prompted LLMs. At Hopkins, we have our own internal HopAI LLMs that students are able to freely use. Likewise, if a student prefers not to use LLMs, that is also possible as was the case in previous years since the live coding session provides everything the students need to complete their HW without the use of LLMs. So in that sense, LLM-assistance in coding was not mandatory. 

Throughout their HWs and projects, students then worked with real biological data and used data visualization to address exploratory questions. They were asked to explain their analysis and visualization design choices, submit their code, AND their LLM prompts (if any).


### The Good

Compared to previous years where LLM-assisted vibe coding was not permitted, this year, some students really excelled. My sense is that students who were previously bottlenecked by the ability to produce code were now thriving, creating compelling data visualizations with great design choices. And this is evident when I look at their prompts. They used AI to augment their learning and excel beyond the mechanics of coding, prompting things like "How can I create an outline only around my cluster of interest to harness the Gestalt Principle of Enclosure in R?" or "How can I make a ggplot where each point corresponds to a cell with the x and y coordinates corresponding to their physical space in the pos matrix, the point color saturation corresponds to the Ki67 log-scaled gene expression data from the mat matrix, and the outline of the cell corresponds to whether the cell belongs to cluster 2 based on my kmeans clustering?"

They did the thinking and had a clear and concrete vision on what they wanted to create. They simply used AI to execute their vision more efficiently. 


### The Same-Old-Same-Old

But producing data visualizations faster does not mean interpreting them correctly. Students still struggled (appropriately) with how to approach feature selection, dimensionality reduction, and ultimately making biological claims regarding the underlying data based on the visualizations they made. So in that sense, the learning challenges did not change much compared to previously years. 


### The Not-So-Good

Compared to previous years where LLM-assisted vibe coding was not permitted, this year, some students really struggled. I noticed students who struggled the most often used prompts like "Write R code given these assignment specifications." So my sense is that they used AI to effectively offloaded the thinking itself. These prompts resulted in completely incoherent data visualizations because LLMs (at least right now) do not look at the output and evaluate whether the data visualization or interpretation is correct. Sure, the LLM created *a* data visualization. But the identified clusters didn't match the identified upregulated genes didn't match the spatial patterns in the tissue. 

Poor grades followed along with explicit feedback that the interpretation was nonsensical. But I was frankly surprised that it didn't seem to deter this style prompting and the same mistakes repeated. 


### Additional Tensions

Compared to previous years where LLM-assisted vibe coding was not permitted, this year, some students designed genuinely clever new visualizations and analysis approaches. Again, no longer bottlenecked by the ability to produce code, they were able to ask more interesting questions and of course use code to create visualizations that addressed these questions. 

But compared to previous years, this year, more students defaulted to "conventional" data visualization designs (heatmaps, violin plots). They chose to justify design and analysis choices as "this is the standard way" (perhaps implicitly according to the LLMs.) Without a strong vision, these students became constrained by what the LLM suggested rather than pushing their own ideas.


### Final Take-aways and what I'm Changing Next Semester

I initially expected that this new LLM-assisted vibe coding would allow every student in the class to do better (make better visualizations, answer questions more deeply, explore more thoroughly, more quickly) compared to previous classes. And that enhancement would be reflected in the grade distribution. 

LLM-assisted vibe coding definitely enhanced...some students. Unexpectedly to me, vibe coding substantially widened the grade distribution. It effectively separated those who leveraged the tool to augment learning from those who didn't.

LLM-assisted vibe coding also forced the educational challenge to evolve from "How can I get students to code this?" to "How can I get students to think critically about what visualization do they actually want to make?" As a teacher, I'm freed from designing assignments around coding abilities and now able to design more interesting assignments around deeper inquiry. 

There are still definitely things I plan to change next semester. In particular, I plan to spend more time demonstrating in class why you shouldn't prompt in certain ways and explaining more explicitly why the LLM output is bad and incoherent. Likewise, I will spend more time encouraging students to take more risks to design new data visualizations not already well represented in the training data. 

But at least for now, I plan to keep LLM-assisted vibe coding as part of my class.
