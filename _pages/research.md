---
layout: page
permalink: /research/
title: research
description: 
nav: true
nav_order: 1
---


My research is focused on developing AI-enabled software development techniques and tools in order to improve developers' productivity, make better data-informed decisions, and better improve the quality of software systems. His resaerch have contributed to various activities in software development, including <b>AI for Software Defects and Cybersecurity, AI for Code Review, AI for Agile, and Explainable AI for Software Engineering</b>.


Our society is now driven by software. However, software defects and technology glitches are very annoying and expensive, and they are very hard to detect and prevent. Errors in safety-critical systems could result in serious injuries and even death (e.g., massive overdose of radiotherapy of Therac-25, to an explosion of the Ariane 5 rocket). We want to prevent this as much as possible.


### Defect Prediction Technologies: Catching Software Defects Before Deployment. 


<center><a href="https://www.monash.edu/it/news/2020/world-first-bughunter-arc-decra-fellow-develops-ai-that-can-detect-defects-faster"><img width="100%" src="https://www.monash.edu/__data/assets/image/0004/2411662/bughunter.png"></a></center>


Imagine you are a developer working on a software project with million lines of code. Developers have to spend years and years reviewing and testing every single line of code, which is very time-consuming and inefficient. This leads to project overruns and high costs.

To address this problem, I develop **defect prediction technologies**, i.e., an AI/ML model that is trained on historical data to predict which files/commits are likely to be defective in the future. To date, defect prediction technologies are widely-used in many top software companies (e.g., <a href="https://www.zora.uzh.ch/id/eprint/25785/2/Zimmermann_Nagappan_Gall_Giger_Murphy_2009.pdf">Microsoft</a>, <a href="https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/41145.pdf">Google</a>, <a href="https://arxiv.org/pdf/1902.06111.pdf">Facebook</a>, <a href="https://aws.amazon.com/codeguru/">Amazon</a>, <a href="http://www.cse.yorku.ca/~zmjiang/publications/FSE2012_shihab.pdf">Blackberry</a>, <a href="https://www.researchgate.net/publication/303296550_A_study_of_the_quality-impacting_practices_of_modern_code_review_at_Sony_mobile">Sony</a>, <a href="https://www.researchgate.net/publication/350853761_The_Impact_of_Data_Merging_on_the_Interpretation_of_Cross-Project_Just-In-Time_Defect_Models">Huawei</a>, <a href="https://dl.acm.org/doi/10.1145/3368089.3417048">Alibaba</a>, <a href="https://ieeexplore.ieee.org/document/7202954">Cisco</a>, <a href="https://techcrunch.com/2019/02/12/ubisoft-and-mozilla-team-up-to-develop-clever-commit-an-ai-coding-assistant/">Ubisoft</a>).

**Goal:** The goal of my research is to invent the next-generation defect prediction technologies that are practical, explainable, and actionable for practitioners, enabling developers to find software defects faster (e.g., find 20% more defects before the testing phase begins) and enabling managers to better develop software quality improvement plans to prevent defects in the future. Potential benefits include the optimal cost saving of software quality assurance activities that are expensive and time-consuming. 

#### Making defect prediction models more practical, explainable, and actionable.

My research team aims to make defect prediction models more practical (i.e., precisely locate which lines are defective), more explainable (i.e., accurately explain why a file/commit is predicted as defect), and more actionable (i.e., accurately guide what developers should do or should not do in the future to mitgiate the risk of having defects).

1. **Line-Level Defect Prediction Techniques.** The current granularity level of defect predictions is still coarse-grained at the file level, leaving practitioners to spend unnecessary effort on inspecting 97%-99% clean lines that are actually not defective. Practitioners often asked which lines are actually defective.
  - <a href="https://www.computer.org/csdl/journal/ts/5555/01/09193975/1n0EsxgwzDy">Our TSE'21 paper proposed **LINE-DP**, the first line-level released-based defect prediction technique.</a>  
  - <a href="https://www.researchgate.net/publication/350061459_JITLine_A_Simpler_Better_Faster_Finer-grained_Just-In-Time_Defect_Prediction">Our MSR'21 paper proposed **JITLine**, the first line-level just-in-time defect prediction model for released-based scenarios.</a> 

2. **Explainable Defect Prediction Techniques.** Existing defect prediction models have empowered software companies to support a wide range of improved decision-making and policy-making. However, such predictions made by defect models to date have not been explained and well-justified. Specifically, current defect prediction models still fail to explain why models make such a prediction and fail to uphold the privacy laws in terms of the requirement to explain any decision made by an algorithm. A lack of explainability of the predictions of defect models, hindering the adoption of defect models in practice. Practitioners often asked why a file is predicted as defective.
  - <a href="https://ieeexplore.ieee.org/document/9044387">Our TSE'21 paper suggested to use **LIME** to explain the predictions of defect models,</a> enabling managers to make data-informed decisions when developing software quality improvement plans. The results show that 65% of the practitioners agree that LIME is useful to help them understand why a file is predicted as defective.
  - We develop the first online book on <a href="http://xai4se.github.io/">Explainable AI for Software Engineering,</a> with a hands-on tutorial on how to make software analytics more <a href="https://www.researchgate.net/publication/350061459_JITLine_A_Simpler_Better_Faster_Finer-grained_Just-In-Time_Defect_Prediction">practical</a>, <a href="https://ieeexplore.ieee.org/document/9044387">explainable</a>, and <a href="https://www.researchgate.net/publication/349491978_SQAPlanner_Generating_Data-Informed_Software_Quality_Improvement_Plans">actionable</a>. Check out more info at <a href="http://xai4se.github.io">http://xai4se.github.io</a>. <a href="https://xai4se.github.io"><img height="50px" src="https://xai4se.github.io/_images/front-banner.png"></a>

\**This research project is financially supported by **Australian Research Council**'s Discovery Early Career Researcher Award (DECRA 2020-2023).*

<!-- <center><iframe width="560" height="315" src="https://www.youtube.com/embed/AdVqSdkT_ok" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe><iframe width="560" height="315" src="https://www.youtube.com/embed/bM2kOZJdBIE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></center> -->

#### Making defect prediction models that produce the most accurate predictions and reliable insights.

The successful deployment of defect prediction models relies heavily on an in-depth understanding of many intricate details that are associated with the analytical modelling process. However, due to the ubiquitous access to statistical and machine learning toolkits (e.g., R, Weka, Scikit-learn), many users of such modelling toolkits have limited knowledge about many important details (e.g., often missing to deal with correlated variables in defect models). Such limited knowledge often leads to major problems which in turn invalidate the results of software engineering studies and lead to the failure of defect prediction projects in practice. 

To address this problem, I develop many **practical guidelines** on how to build defect prediction models through empirical studies. In particular, I investigate how each of the key experimental components will impact the performance and the interpretation of defect prediction models. 

1. **Techniques for Mining Software Defects.** Poor quality or noisy defect datasets could lead to inaccurate predictions and insights. We found that techniques for generating ground-truth data is often not accurate, impacting the quality of defect datasets. 
 - <a href="https://ieeexplore.ieee.org/document/7194628">Our ICSE'15 paper suggested not to be concerned about issue report misclassification</a>.
 - <a href="https://ieeexplore.ieee.org/document/8811982">Our ICSE'19 paper suggested using **affected releases** (i.e., the actual software releases that are affected) to label whether a file is considered to be defective or clean, instead of the assumptions of a post-release window period (i.e., any defects that are fixed after 6 months)</a>.

2. **Techniques for Analysing Software Defects.** Defect datasets are highly imbalanced with a defective ratio of <10%. Defect models trained on class imbalance datasets often produce inaccurate models. 
  - <a href="https://ieeexplore.ieee.org/document/8494821">Our TSE'19 paper suggested to consider using **optimised SMOTE** to improve the predictive accuracy, i.e., handling the class imbalance of the training datasets prior to training the defect models</a>. 
  - <a href="https://ieeexplore.ieee.org/document/8608002">Our TSE'21 paper suggested to handle **colliniearity and multicollinearity** when interpreting defect models (i.e., understanding what are the most important variables)</a>. 
  - <a href="https://ieeexplore.ieee.org/document/8530020">Our ICSME'18 paper suggested to **avoid using existing automated feature selection techniques (e.g., Stepwise Regression)** if the goal is to interpret defect prediction models, as they fail to mitigate correlated features and are dependent on random seeds.</a>
  - <a href="https://link.springer.com/article/10.1007/s10664-020-09848-1">Our EMSE'21 paper suggested **AutoSpearman** is the best automated feature selection technique for handling collinearity and multi-collinearity.</a>

3. **Techniques for Predicting Software Defects.** There exist a large number of off-the-shelf classification techniques that can be used with a large number of possible combination of hypereparameter settings that can be configured. Sadly, practitioners often asked which techniques and which settings should be used.
  - <a href="https://ieeexplore.ieee.org/document/7886914">Our ICSE'16 paper suggested to explore various classification techniques and hyperparameter settings. **Optimised random forest** and optimised extreme gradient boosting trees often produce the most accurate defect prediction models.</a>
  - <a href="https://ieeexplore.ieee.org/document/8263202">Our TSE'19 paper suggested to always **optimize the hyperparameter settings** of defect prediction models (e.g., using Grid Search, Random Search, Genetic Algorithm, Differential Evolution).</a>
  - <a href="https://ieeexplore.ieee.org/document/7497471">Our TSE'17 paper suggested to use the **Scott-Knott ESD test** to identify the best classification techniques that are statistically significantly different with non-negligible Cliff's |delta| effect size.</a>
  - <a href="https://ieeexplore.ieee.org/document/7497471">Our TSE'17 paper suggested to estimate the accuracy of defect prediction models using **out-of-sample boostrap** model validation techniques when defect datasets are very small (i.e., EPV < 10).</a>


4. **Techniques for Explaining Software Defects.** 
  - <a href="https://ieeexplore.ieee.org/document/8608002">Our TSE'21 paper suggested **ANOVA Type-II** should be used for explaining the defect prediction models (built using regression models), instead of using ANOVA Type-I.</a> -->

\*\**This research project is financially supported by <a href="">**Japan Society for the Promotion of Science**'s Research Fellowship (JSPS DC2 2016-2018, 4,800,000 JPY)</a>, <a href="http://www.candc.or.jp/">**NEC C&C Research Grant** for Non-Japanese Researchers (2014-2015, 1,500,000 JPY)</a>.* 

His research is focused on developing AI-enabled software development techniques and tools in order to improve developers' productivity, make better data-informed decisions, and better improve the quality of software systems. His resaerch have contributed to various activities in software development, including AI for Software Defects and Cybersecurity, AI for Code Review, AI for Agile, and Explainable AI for Software Engineering.


<!-- ## AI for Software Defects and Cybersecurity (ARC DECRA Project, 2020-2023)

<center><a href="https://www.monash.edu/it/news/2020/world-first-bughunter-arc-decra-fellow-develops-ai-that-can-detect-defects-faster"><img width="100%" src="https://www.monash.edu/__data/assets/image/0004/2411662/bughunter.png"></a></center>

I invent an AIBugHunter 2.0 tool, the first practical AI-powered tool that can detect, localize, explain and suggest vulnerability repairs in IDE during the software development stage–not just discover vulnerabilities at the end of the software development lifecycle, which is likely to reduce the cost of vulnerability discovery, speed up software development cost, and developers’ productivity. Currently, the tool is publicly available in Microsoft’s Visual Studio Marketplace. AIBugHunter is built on top of various approaches. For example, LineVul [MSR’22, a Special Issue Invitee] is a Transformer-based line-level vulnerability localization. VulRepair [ESEC/FSE’22] is a T5-based automated vulnerability repairs. He has discovered as many as 348 vulnerabilities in safety-critical Free Open-Source Software (FOSS) systems. These vulnerabilities are considered as the Top-25 most dangerous CWE types in 2021 (e.g., CWE-190 Integer Overflow, CWE-787 Out of bound Write, CWE-20 Improper Input Validation). These findings highlights the strong potential impact of his LineVul in real-world practices, providing a world-most accurate vulnerability discovery approach to help security analysts to discover vulnerabilities faster, enabling software organizations to immediately react to the cyber attacks, and protecting cyber attacks from national and international's cyberinfrastructure. His work also received strong attention from various media (e.g., Gizmodo, Australian Cyber Security Magazine, TechXplore, Cybersecurity Connect, Australian Computer Society).</p>

Reference: https://marketplace.visualstudio.com/items?itemName=AIBugHunter.aibughunter


## AI for Code Review

I invent various AI approaches to support automated code reviewing activities from prioritisation to automated repairs. For example, JITLine [MSR’21] is an approach to help reviewers identify which code changes and which lines are most likely to be defective in the future. PyExplainer [ASE’21, ACM SIGSOFT Distinguished Paper Award] is an approach to explain why a model is predicted a given code change as defective. RevSpot [SANER’22] is an approach to help reviewers pinpoint the lines that need some attentions. CommentFinder [ESEC/FSE’22] is an approach to automatically recommend code review comments based on a given changed method. AutoTransform [ICSE’22] is an approach that aims to generate an approved version for a given code change. These approaches are likely to increase code review speed and reviewers' productivity.


## AI for Agile

I invent a Large Language Model (LLM, i.e., GPT2)-based model for Agile story point estimation that outperforms the state-of-the-art, which is recently published at IEEE Transactions on Software Engineering. Story point estimation is a task to estimate the overall effort required to fully implement a product backlog item. Various estimation approaches (e.g., Planning Poker, Analogy, and expert judgment) are widely-used, yet they are still inaccurate and may be subjective, leading to ineffective sprint planning. To address this challenge, he developes a GPT2SP approach, which employ a GPT-2 pre-trained language model with a GPT-2 Transformer-based architecture, allowing our GPT2SP models to better capture the relationship among words while considering the context surrounding a given word and its position in the sequence and be transferable to other projects, while being interpretable. The survey study with 16 Agile practitioners shows that our AI-based story point estimation with explanations is perceived as more useful and trustworthy than without explanations, highlighting the practical need of our Explainable AI-based story point estimation approach.

# Explainable AI for Software Engineering (XAI4SE)

<a href="https://xai4se.github.io"><img width="50%" src="https://xai4se.github.io/_images/front-banner.png"></a>

I have made seminal contributions to Explainable AI for software engineering, advancing the fundamentals of AI4SE approaches to be more practical, explainable, and actionable. Explainable AI for SE is a pressing concern for the software industry and academia. In the light of predictions made in SE contexts, practitioners would like to know Why has this code been generated? Why is this person best suited for this task? Why is this file predicted as defective? Why is this task required the highest development effort?, etc. CI Tantithamthavorn conducted a practitioner’s survey study [MSR’20] and found that explanations from AI/ML models in SE are critically needed, yet remain largely unexplored. His contributions are evidenced by various novel approaches to make AI4SE approaches more explainable and actionable to support vaiours SE tasks. For example, GPT2SP is an explainable GPT-based story point estimation [TSE’22], including an award-winning paper like PyExplainer [ASE’21, ACM SIGSOFT Distinguished Paper Award, CORE A*]. In addition, he developed the first online book and his tutorial on Explainable AI for Software Engineering at ASE’21 (CORE A*) (http://xai4se.github.io). His XAI4SE online book attracted 13,000+ pageviews from 83 countries worldwide and received positive responses from the SE community. His publications, books, and tutorials have informed many other studies and educated the SE community on the importance of explainability and its applications to software engineering. He is invited to be a guest editor of Explainable AI for Software Engineering at IEEE Software. Particularly, he led a challenge to the SE research community to not only look at the accuracy improvement, but also consider the explainability aspects, making automated software tools more practical, explainable, and actionable to be widely adopted in practice. He cares about making software engineering research more impactful and translatable. -->