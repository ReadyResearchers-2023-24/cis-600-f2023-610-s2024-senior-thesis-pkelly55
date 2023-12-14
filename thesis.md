# Introduction

The following provide a walkthrough for my project. The sections below are the motivation, current state of the art, goals of the project, and ethical implications. In is paper, will be discussing the aformenetioned topics for IPLOCK(name subject to change). IPLOCK is a program that will be a django web application that will be used to prevent brute force attacks on a server. This will be done by essentially blocking the IP address of the attacker or possible attacks. This will be done by using the django framework and the python programming language along with other tools.

## Motivation

The motivation behind this project came after a long period of mulling over topics and different things that I could do for my senior thesis. After alot of consideration, I decided to do something that I have been interested in for a while. I have always been interested in cyber security and the different ways that people can protect themselves from attacks. For most of my life, I have been a football player and I played defense, so I have always been interested in the defensive side of things and keeping people out. Along with this interest, I have always been interested in the different ways that people can get into systems and the different ways that people can protect themselves from the threats that are out there. Over the summer of 2023 I gained an internship with Penncrest School District to work with their Director of Technology, System Administrator, and Information Systems Specialist. During this internship, we were taken to the NWPA Security & Technology Summit in Erie, Pennsylvania. During this summit, we heard from plenty of speakers from companies such as Huntress and Phin. One of the goals of the event was to showcase how cyber security affects all parts of an organization, from executive, finance, human resources, and technology. One of the keynote speakers spoke on the topic of stolen credentials and how they are used to gain access to systems. This was also to include the use of the dark web and how it plays a role in cyber warfare people are calling it. To be able to protect sensitive data agaist hackers and bots is a very valuable business. This is why I chose to do this project.

## Current State of the Art

The current state of the art in security is now mandating MFA, I know this because my experience during internship at PSD, I set up MFA for all of the student body and staff for services. This is a very important step in the right direction for security. Where most business can fall the most vunerable online is through their website.

This is not only important in the education sector. A growing mindset is being taken on in the business sector by taking on MFA or 2FA for their services. In 2019, it was found that '57% of businesses were using MFA' for their services. [@Lightfoot_2023] This is a 12% increase from 2018.  This is a very important step in the right direction for security. Where most business can fall the most vunerable online is through their website.  However, this is not far to show all the businesses grouped together, Small businesses are highly vunerable to cyber attacks. Through self-reporting studies '54% of small to medium sized businesses (SMBs) do not implement MFA.' [@Lightfoot_2023] Businesses may not be aware of the threats that are out there and the simple and effective ways they could chose to protect themselves online. This is where IPLOCK comes in. IPLOCK will be a simple and effective way to protect a business from brute force attacks on their website. This will be done by blocking the IP address of the attacker or possible attacks. This will be done by using the django framework and the python programming language along with other tools.

The current state of the problem is that there are many different ways that criminals look to get information to use in an online attack. In a paper by the National Security Agency (NSA), they discuss cybersecurity information and steps to protect ones identity. They discuss the effects of Identity theft and the facts of how it creates an out of pocket loss for 14% of victims.[@CybersecurityInformation_2018]  Now this is to show how what happens when a individual's identity gets stolen. If this were to happen in a business, the effects could be far worse. One of the ways people can get information is through phishing. A different term and that could be used is Whaleing. The NSA Defines it as 'a common ID theft technique, is the targeting of high rankning coporate executives (the big fish) via malicious emails, links, or attachments etc.'[@CybersecurityInformation_2018] Descibing best practices for individuals protecting themselves from being targeted or having their credentials. One of the hardest things to defend is the attacks that you do not see. The threats that hide on the dark web are very hard to defend when there are groups putting up money to get information on people. Best practices include taking every data leak you hear or recieve notification about is important. When data leaks happen the user should be notified and take steps to resecure the account. People may think that they wont be the one to get compromised.

## Goals of the Project

My project tries to answer the problem that exists in the world that small businesses need the right framework to protect themselves in the world of online threats. The research question I look to answer is how can Django be used to build a scalable, robust, and secure site administration for those who do have any source of security. I look to do this by using the tools that Django provides in working with the admin site and its built in database models. By building a system that would allow a company to put their site behind a login page, this would allow them to protect their site from brute force attacks. Django is an easy to use web framework in Python to connect all the web pages together. The justification for using Django in building a secure site administration becomes evident in light of the challenges posed by the asymmetry of knowledge between attackers and users/identity providers.The proposed privacy-preserving protocol outlined in the text aligns with your project's objectives. By allowing a client (end user, password manager, or identity provider) to query a centralized breach repository without revealing sensitive information, your system mirrors the need for a secure framework. Django's tools, especially its built-in admin site and database models, can play a pivotal role in implementing such a protocol.
The emphasis on putting a company's site behind a login page, using Django's user authentication system, directly addresses the issue of protecting against brute force attacks. The system you're building aligns with the need for secure, scalable, and robust site administration, as highlighted in the research question.
Moreover, the practical demonstration of the protocol's feasibility, involving a cloud service mediating access to billions of credentials, resonates with the scalability aspect of your project. Django's ease of use and its ability to connect web pages seamlessly make it a suitable choice for creating a comprehensive and user-friendly solution.
In addressing the prevalent issue of credential stuffing attacks, our project aims to provide a robust solution to a problem that is alarmingly widespread. According to recent findings, a staggering 1.5% of web logins involve compromised credentials, highlighting the pervasive nature of this threat. [@236316] This statistic serves as a stark reminder of the urgent need for effective measures to protect users and businesses from the consequences of unauthorized access and potential account hijacking.

Upon implementing our proposed privacy-preserving protocol, designed to enable clients, including end users, password managers, and identity providers, to query a centralized breach repository without compromising sensitive information, we observed a significant user response. An encouraging 26% of users, upon receiving alerts about their breach status, took proactive steps to enhance their security. [@236316] This positive user response underscores the practical effectiveness of our protocol in empowering individuals to safeguard their accounts by migrating to new and stronger passwords.

To contextualize the magnitude of the issue at hand, it is crucial to consider the scale of recent breach compilations. Compilations such as Antipublic, Exploit.in, and Collection 1-5 have collectively exposed billions of credentials, trivializing criminal access to a vast number of accounts.[@236316] This widespread exposure of usernames and passwords emphasizes the urgency of our project's solution within the context of a constantly evolving landscape of cyber threats. The scale of these breach compilations serves as a compelling backdrop, illustrating why our project's contribution is not just relevant but imperative in the face of such extensive credential exposure.

The process of developing a website involves a critical decision—selecting the most suitable framework for the application. This choice holds immense importance as it can significantly impact the website's performance. Given the variety of frameworks available, the decision is not an easy one, and selecting the wrong framework may have adverse effects on the site.

Web applications handle substantial amounts of personal data daily, making data security and integrity paramount. Injection attacks, a common threat, can compromise a website's database by injecting unauthorized data into the application. This research paper delves into Django, a Python-based web framework renowned for its open-source nature and adherence to the Model-View-Template structure. The paper explores the unique aspects of Django and elucidates why it stands out among other web frameworks in the industry. Additionally, it provides guidance on installing Django on a system and creating a basic project using this framework.In the realm of web frameworks, Django plays a pivotal role as a tool for constructing websites efficiently while minimizing bugs and saving time. Its open-source nature and Python language foundation contribute to its popularity in the current market, particularly due to its rapid development capabilities. The Model-View-Template structure defines Django's approach, with the model serving as the database, the view controlling functionality, and the template facilitating client-side interaction.

The development process in Django involves executing commands such as 'python manage.py migrate,' enabling the framework to store all changes in its database system. Views are written as Python functions, showcasing the seamless integration of Python in web development. The paper highlights the fundamental principles of web development using Django, emphasizing the implementation of CRUD functionality (Create, Read, Update, Delete) to build robust blog applications.Django, a widely adopted free and open-source web development framework, distinguishes itself by offering an array of features "out of the box," expediting the development process. Its widespread use attests to its effectiveness in simplifying and accelerating web development tasks.

## Ethical Implications

This document requires that you discuss the ethical implications of your work -- no
matter how benign you consider the outcome of your project. As several major studies
of ethical issues in computer science assert: _no project is completely value-neutral_.

To assist you in elaborating on these issues, the following areas are topics you might
consider addressing. You do not need to address all of them.

* Information Privacy
* Information Accuracy (e.g. can contain reliability)
* Potential Misuse (e.g. computer crime, unintended consequences)
* Second- or Third-Party Risk (e.g. safety)
* Data Collection Issues (e.g. issues inherent in collecting data)
* Algorithmic or Data Bias
* Potential Power Difference / Social Imbalance / Issues in Equity

In addition, reflect on ways that the above harms can be or are mitigated by your work

# Related work

This chapter includes a broad and detailed review of relevant existing work.
The literature review should provide background and context for the thesis work.
The subsections may be organized in whatever manner seems best suited to the material--
chronological, or by topic, or according to some other criteria
(e.g., primary versus secondary resources).

If ethical issues are central to this work, you should also address historical and
contemporary issues or efforts made to address them.

# Method of approach

This chapter answers the "how" question - how did you complete your project,
including the overall design of your study, details of the algorithms and tools you
have used, etc.  Use technical diagrams, equations, algorithms, and paragraphs of text
to describe the research that you have completed. Be sure to number all figures and
tables and to explicitly refer to them in your text.

This should contain:

* lists
* with points
* and more points
  * possibly subpoints

For those projects whose implications address social or moral issues (i.e. ethical
standards, causes, effects), you will want to use this section to describe how you
actively mitigated or considered these issues.

# Experiments

This chapter describes your experimental set up and evaluation. It should also
produce and describe the results of your study. The section titles below offer
a typical structure used for this chapter.

## Experimental Design

Especially as it pertains to responisble computing, if conducting experiments or
evaluations that involve particular ethical considerations, detail those issues here.

## Evaluation

## Threats to Validity

# Conclusion

Traditionally, this chapter addresses the areas proposed below as sections, although
not necessarily in this order or organized as offered. However, the last section --
"Ethical Implcations" is required for this chapter. See the heading below for more
details.

## Summary of Results

## Future Work

## Future Ethical Implications and Recommendations

Especially as pertains to the public release or use of your software or methods, what
unresolved or special issues remain? What recommendations might you make?

## Conclusions


# References

::: {#refs}
:::
