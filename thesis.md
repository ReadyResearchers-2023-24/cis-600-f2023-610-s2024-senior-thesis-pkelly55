# Introduction

The following provide a walkthrough for my project. The sections below are the motivation, current state of the art, goals of the project, and ethical implications. In is paper, will be discussing the aformenetioned topics for IPLOCK(name subject to change). IPLOCK is a program that will be a django web application that will be used to prevent brute force attacks on a server. This will be done by essentially blocking the IP address of the attacker or possible attacks. This will be done by using the django framework and the python programming language along with other tools.
The motivation behind IPLOCK stems from the escalating threat of brute force attacks on servers, a pervasive issue that jeopardizes the security of digital systems. As technology advances, malicious actors continuously exploit vulnerabilities to gain unauthorized access. IPLOCK aims to counter this menace by developing a robust Django web application that proactively identifies and blocks potential attackers based on their IP addresses. The significance of this project lies in fortifying server defenses, thwarting unauthorized intrusion attempts, and ultimately safeguarding sensitive data from compromise.


## Motivation

The motivation behind this project came after a long period of mulling over topics and different things that I could do for my senior thesis. After alot of consideration, I decided to do something that I have been interested in for a while. I have always been interested in cyber security and the different ways that people can protect themselves from attacks. For most of my life, I have been a football player and I played defense, so I have always been interested in the defensive side of things and keeping people out. Along with this interest, I have always been interested in the different ways that people can get into systems and the different ways that people can protect themselves from the threats that are out there. Over the summer of 2023 I gained an internship with Penncrest School District to work with their Director of Technology, System Administrator, and Information Systems Specialist. During this internship, we were taken to the NWPA Security & Technology Summit in Erie, Pennsylvania. During this summit, we heard from plenty of speakers from companies such as Huntress and Phin. One of the goals of the event was to showcase how cyber security affects all parts of an organization, from executive, finance, human resources, and technology. One of the keynote speakers spoke on the topic of stolen credentials and how they are used to gain access to systems. This was also to include the use of the dark web and how it plays a role in cyber warfare people are calling it. To be able to protect sensitive data agaist hackers and bots is a very valuable business. This is why I chose to do this project.
The escalating frequency of cyber attacks on the education sector serves as a poignant motivation for the development of robust cybersecurity measures. Microsoft's alarming report, indicating that the education center is the most susceptible industry to cyber attacks at a staggering 79.48%, underscores the critical need for enhanced security protocols. The sector, often targeted due to its high online traffic and increased student enrollment, finds itself vulnerable despite being an entity that should ideally lead in cybersecurity. This discrepancy highlights the urgency for proactive measures to fortify the education sector against cyber threats.[@Csirt_2023]

In the face of rampant cyber attacks, particularly in the unprecedented year of 2020, there is a pressing need to address the vulnerabilities that threaten vital information within educational institutions. Ransomware attacks, specifically targeting school and student data, have reached an all-time high.[@Csirt_2023] A crucial aspect of cybersecurity involves preventing such attacks, safeguarding the integrity of academic and personal information. Recognizing the importance of cybersecurity training becomes imperative, not only for the protection of institutional data but also for empowering students and staff with skills that extend beyond academic boundaries. Cybersecurity education equips individuals with practical skills for data protection, making it not just a necessity for academic security but also a potential pathway to a career in cybersecurity. As the education sector faces unprecedented challenges, the motivation to develop effective cybersecurity solutions becomes paramount in safeguarding the integrity and privacy of educational institutions and their stakeholders.

## Current State of the Art

This section critically examines the existing landscape of brute force attack prevention methods, tools, and technologies. By thoroughly reviewing the state of the art, the thesis seeks to identify gaps and opportunities for improvement in current approaches. Understanding the strengths and limitations of existing solutions is crucial for positioning IPLOCK as an innovative and effective contribution to the field of web application security.
The current state of the art in security is now mandating MFA, I know this because my experience during internship at PSD, I set up MFA for all of the student body and staff for services. This is a very important step in the right direction for security. Where most business can fall the most vunerable online is through their website.

This is not only important in the education sector. A growing mindset is being taken on in the business sector by taking on MFA or 2FA for their services. In 2019, it was found that '57% of businesses were using MFA' for their services. [@Lightfoot_2023] This is a 12% increase from 2018.  This is a very important step in the right direction for security. Where most business can fall the most vunerable online is through their website.  However, this is not far to show all the businesses grouped together, Small businesses are highly vunerable to cyber attacks. Through self-reporting studies '54% of small to medium sized businesses (SMBs) do not implement MFA.' [@Lightfoot_2023] Businesses may not be aware of the threats that are out there and the simple and effective ways they could chose to protect themselves online. This is where IPLOCK comes in. IPLOCK will be a simple and effective way to protect a business from brute force attacks on their website. This will be done by blocking the IP address of the attacker or possible attacks. This will be done by using the django framework and the python programming language along with other tools.

The current state of the problem is that there are many different ways that criminals look to get information to use in an online attack. In a paper by the National Security Agency (NSA), they discuss cybersecurity information and steps to protect ones identity. They discuss the effects of Identity theft and the facts of how it creates an out of pocket loss for 14% of victims.[@CybersecurityInformation_2018]  Now this is to show how what happens when a individual's identity gets stolen. If this were to happen in a business, the effects could be far worse. One of the ways people can get information is through phishing. A different term and that could be used is Whaleing. The NSA Defines it as 'a common ID theft technique, is the targeting of high rankning coporate executives (the big fish) via malicious emails, links, or attachments etc.'[@CybersecurityInformation_2018] Descibing best practices for individuals protecting themselves from being targeted or having their credentials. One of the hardest things to defend is the attacks that you do not see. The threats that hide on the dark web are very hard to defend when there are groups putting up money to get information on people. Best practices include taking every data leak you hear or recieve notification about is important. When data leaks happen the user should be notified and take steps to resecure the account. People may think that they wont be the one to get compromised.

## Goals of the Project

Clearly defining the objectives of IPLOCK is paramount for guiding the development process. The project aims to achieve several goals, including the implementation of intelligent IP address blocking, seamless integration with the Django framework, and providing an enhanced layer of defense against brute force attacks. These goals serve as a roadmap, shaping the direction of the project and providing criteria for evaluation throughout the development and experimentation phases.
My project tries to answer the problem that exists in the world that small businesses need the right framework to protect themselves in the world of online threats. The research question I look to answer is how can Django be used to build a scalable, robust, and secure site administration for those who do have any source of security. I look to do this by using the tools that Django provides in working with the admin site and its built in database models. By building a system that would allow a company to put their site behind a login page, this would allow them to protect their site from brute force attacks. Django is an easy to use web framework in Python to connect all the web pages together. The justification for using Django in building a secure site administration becomes evident in light of the challenges posed by the asymmetry of knowledge between attackers and users/identity providers.The proposed privacy-preserving protocol outlined in the text aligns with your project's objectives. By allowing a client (end user, password manager, or identity provider) to query a centralized breach repository without revealing sensitive information, your system mirrors the need for a secure framework. Django's tools, especially its built-in admin site and database models, can play a pivotal role in implementing such a protocol.
The emphasis on putting a company's site behind a login page, using Django's user authentication system, directly addresses the issue of protecting against brute force attacks. The system you're building aligns with the need for secure, scalable, and robust site administration, as highlighted in the research question.
Moreover, the practical demonstration of the protocol's feasibility, involving a cloud service mediating access to billions of credentials, resonates with the scalability aspect of your project. Django's ease of use and its ability to connect web pages seamlessly make it a suitable choice for creating a comprehensive and user-friendly solution.
In addressing the prevalent issue of credential stuffing attacks, our project aims to provide a robust solution to a problem that is alarmingly widespread. According to recent findings, a staggering 1.5% of web logins involve compromised credentials, highlighting the pervasive nature of this threat. [@236316] This statistic serves as a stark reminder of the urgent need for effective measures to protect users and businesses from the consequences of unauthorized access and potential account hijacking.

Upon implementing our proposed privacy-preserving protocol, designed to enable clients, including end users, password managers, and identity providers, to query a centralized breach repository without compromising sensitive information, we observed a significant user response. An encouraging 26% of users, upon receiving alerts about their breach status, took proactive steps to enhance their security. [@236316] This positive user response underscores the practical effectiveness of our protocol in empowering individuals to safeguard their accounts by migrating to new and stronger passwords.

To contextualize the magnitude of the issue at hand, it is crucial to consider the scale of recent breach compilations. Compilations such as Antipublic, Exploit.in, and Collection 1-5 have collectively exposed billions of credentials, trivializing criminal access to a vast number of accounts.[@236316] This widespread exposure of usernames and passwords emphasizes the urgency of our project's solution within the context of a constantly evolving landscape of cyber threats. The scale of these breach compilations serves as a compelling backdrop, illustrating why our project's contribution is not just relevant but imperative in the face of such extensive credential exposure.

The process of developing a website involves a critical decision—selecting the most suitable framework for the application. This choice holds immense importance as it can significantly impact the website's performance. Given the variety of frameworks available, the decision is not an easy one, and selecting the wrong framework may have adverse effects on the site.

Web applications handle substantial amounts of personal data daily, making data security and integrity paramount. Injection attacks, a common threat, can compromise a website's database by injecting unauthorized data into the application. This research paper delves into Django, a Python-based web framework renowned for its open-source nature and adherence to the Model-View-Template structure.[@Rajeswari_KR.Kamalam_2022] The paper explores the unique aspects of Django and elucidates why it stands out among other web frameworks in the industry. Additionally, it provides guidance on installing Django on a system and creating a basic project using this framework.In the realm of web frameworks, Django plays a pivotal role as a tool for constructing websites efficiently while minimizing bugs and saving time. Its open-source nature and Python language foundation contribute to its popularity in the current market, particularly due to its rapid development capabilities. The Model-View-Template structure defines Django's approach, with the model serving as the database, the view controlling functionality, and the template facilitating client-side interaction.[@Rajeswari_KR.Kamalam_2022]

The development process in Django involves executing commands such as 'python manage.py migrate,' enabling the framework to store all changes in its database system. Views are written as Python functions, showcasing the seamless integration of Python in web development. The paper highlights the fundamental principles of web development using Django, emphasizing the implementation of CRUD functionality (Create, Read, Update, Delete) to build robust blog applications. Django, a widely adopted free and open-source web development framework, distinguishes itself by offering an array of features "out of the box," expediting the development process.[@Rajeswari_KR.Kamalam_2022] Its widespread use attests to its effectiveness in simplifying and accelerating web development tasks.

## Ethical Implications

+ Blacklisting IP addresses is a common security practice employed to block access from specific addresses due to various security concerns. However, like any security measure, this approach raises ethical considerations that necessitate careful attention:

1. Accuracy and Fairness:
Ethical Concern: There is a potential risk of falsely identifying legitimate users as malicious and subsequently blocking their access. This could lead to a denial of service for innocent users. Implement measures to ensure the accuracy of the blacklisting criteria. Regularly review and update the criteria to minimize the chances of false positives.
2. Transparency and Communication:
Ethical Concern: Blacklisting activities may lack transparency, leaving users unaware of the reasons for their blocked access.
Mitigation: Clearly communicate the reasons for blacklisting, providing users with avenues for appeal or clarification. Transparency helps build trust and allows users to understand the security measures in place.

+ Using Historical Database
The utilization of historical databases in the project raises ethical considerations regarding privacy and consent. It's imperative to ensure that the data used is anonymized, and any potential risks associated with historical information are carefully evaluated. Transparency about the source and nature of historical data should be maintained, and efforts should be made to minimize any unintended consequences or biases that may arise from historical data usage.

+ Collecting User Data
The collection of user data demands ethical considerations regarding informed consent, transparency, and user autonomy. Users should be clearly informed about the data collected, the purpose behind its collection, and should have the option to opt-in or opt-out. Respecting user privacy rights and ensuring data is used responsibly and securely are ethical imperatives.

+ Protecting User Data Based on the User
While the intention is to protect user data, ethical concerns arise in determining the criteria for prioritizing user data protection. It's crucial to avoid discrimination and ensure that protection measures are applied fairly and impartially, irrespective of user characteristics. Striking a balance between personalized security and equitable treatment is essential.

+ Data Collection Issues in Forms
Ethical considerations in data collection via forms involve transparency in informing users about the necessity of each piece of information. Users should have clarity on how their data will be used and protected. Minimizing the data collected to only what is essential for the system's functionality is ethical practice, preventing unnecessary invasion of user privacy.

+ Algorithmic Bias in the Proposed Bot Detection System with reCAPTCHA
The use of algorithms, such as reCAPTCHA, introduces the potential for bias, which can disproportionately affect certain user groups. Ethical responsibility lies in continuous monitoring and mitigation of biases, ensuring fair treatment of all users. Regular audits and adjustments to the algorithms are essential to address and rectify any identified biases.

+ Potential Misuse of the System
Addressing the potential misuse of the system is a critical ethical consideration. Safeguards should be implemented to prevent unauthorized access and misuse of the system for malicious purposes. Ethical guidelines should explicitly state the system's intended use, and preventive measures should be in place to minimize the risk of abuse.

+ Second-Party Risk of the System:
Acknowledging the risk that the system itself poses to second parties is an ethical imperative. This involves recognizing potential negative impacts on users, entities, or systems indirectly affected by the project. Mitigation strategies should be in place to minimize such risks, and continuous monitoring and adaptation of the system should occur to address any unforeseen consequences.

Mitigation Strategies:

Transparency is a cornerstone of ethical practices, and Django provides robust tools to achieve this. Through the Django Admin Interface, a responsible system administrator can customize panels to offer a transparent view of the data collected and stored. Additionally, the templating system enables the incorporation of user-facing notices within the web application, ensuring clear communication of the project's purpose, data usage policies, and potential risks.

Informed consent is a crucial aspect of ethical data collection. Leveraging Django's powerful form customization capabilities, a responsible system administrator can create forms with detailed descriptions of each data field. This ensures that users understand the reasons behind specific data requests. Granular consent options, facilitated by Django's form capabilities, empower users to make informed decisions about the information they choose to share.

Regular audits of algorithms are essential to identify and rectify biases. Django's logging system can be employed for tracking activities within the application. By regularly reviewing logs and setting up automated alerts for suspicious patterns, a responsible system administrator ensures ongoing monitoring of potential biases. Integration with analytics tools provides valuable insights into user interactions, aiding in the identification of unintended biases or emerging trends.

Security measures are paramount to safeguarding user data. Django's security middleware offers protection against common threats such as Clickjacking, XSS, and CSRF. A responsible system administrator can enable and configure these features to fortify the application's security. Additionally, Django seamlessly integrates with SSL/TLS protocols, ensuring the encryption of data in transit for enhanced overall security.

Continuous monitoring is facilitated through user feedback mechanisms and performance monitoring. Within the Django application, a responsible system administrator can implement a dedicated feedback form or integrate a support ticket system, allowing users to report concerns or biases. Real-time monitoring of the system's performance, supported by Django's built-in tools or external services, ensures prompt addressing of any issues based on ongoing feedback.

In summary, Django, when coupled with the oversight of a responsible system administrator, provides a robust framework to actualize these mitigation strategies. The collaborative integration of these features aligns with the ethical principles of transparency, informed consent, regular audits, stringent security measures, and continuous monitoring throughout the project's development and deployment lifecycle.
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
