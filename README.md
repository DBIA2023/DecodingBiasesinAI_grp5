# From Qualitative Fod to Quantitative Clarity: Assessing Bias in Talenteria's CV Scoring Algorithm

Decoding Biases in AI 
Sciences Po Paris - Spring 2024

Lukas BRAND, Tathagata CHAKRABORTY, David DÜPJOHANN, José ignacio DONOSO SALAS

## Table of Contents 

“The use of data-driven AI models in recruitment processes raises a host of thorny ethical issues, which demand forethought and diligent assessment on the part of both system designers and procurers.”

 By Dr David Leslie, director of ethics and responsible innovation research at The Alan Turing Institute


  ## Introduction
The advent of algorithmic hiring and the rise of HR tech platforms has completely changed traditional recruitment practices, promising efficiency, mitigating biases prevalent in hiring and streamline decision making protocols. However, as companies rely on automated systems for HR functions, concerns regarding biases inherent in autonomous systems have come to the forefront. Our research paper delves into the intricate landscape of exploring the biases within HR tech companies and their potential impact. First, we navigate through the general development trends in HR tech platforms, we examine the evolution of the tools being developed and adopted by organizations. Secondly, we analyze the market characteristics shaping the adoption and implementation of HR tech solutions, by scrutinizing market dynamics, we may discern how biases may be perpetuated or mitigated within different HR tech platforms. Furthermore, we delve into the origin of discrimination embedded within these platforms, as historical biases affect these autonomous systems, even though they were claimed to be neutral, exacerbating disparities in hiring. By exploring these central issues through our research, where we analyze Talenteria, a HR Tech Recruiting platform startup. Our research aimed to find out whether there are potential AI biases in their CV screening algorithms focusing on age, gender, ethnicity and origin. Finally, we are going to discuss our results and the limitations of our study accordingly.
 

  ## General Developments and Trends 
HR-tech platforms can assume a variety of functions, spanning from recruiting and onboarding to learning/skills management and termination processes (Exh. 1). Established HR Tech functions also include Payroll Management (Statista 2022) which is not examined in this paper as it is not prone to bias. Organizations have the option to procure these diverse functionalities from one or multiple developers or to develop them entirely in-house. However, the latter approach is generally not pursued in SMEs as development costs are deemed as too high. Thus, SMEs but even big companies like Goldman Sachs rely on solutions provided to them by developers and maybe tailored to their needs. The key-promises of HR Tech are that it empowers professionals by automating repetitive tasks, freeing time for strategic initiatives and innovation. By leveraging technology for recruitment and harnessing data-driven analytics, organizations enhance talent acquisition processes and make informed workforce decisions. This transformation not only boosts operational efficiency but also strengthens organizational agility, ensuring adaptability in an ever-evolving digital landscape (O'Connor 2020). 



<p align="center">
 <img src="https://github.com/DBIA2023/DecodingBiasesinAI_grp5/assets/169889828/9634548d-9f43-48b9-a9d1-452ae53a1e5e" alt= "Exhibit 1: _HR Tech Capacities", width= 768 length=361 >

<p/>
 
<p align="center"><b>Exhibit 1: HR Tech Capacities</b></p>
  

 
## Market Characteristics 
Looking at the characteristics of the overall market, the HR sector is experiencing significant growth, both in terms of personnel utilization and revenues. This trend is primarily driven by the increasing focus of many companies on their labor force, particularly in light of the skills shortage. Furthermore, the scope of HR responsibilities has expanded significantly to include tasks such as employee training, performance monitoring and rewarding, and assisting employees in adapting to policy changes (Statista 2022). In the United States, which represents the largest market for HR and HR Tech, approximately 700,000 individuals were employed in the HR sector as of 2019 (Statista 2022). Despite the sector's contraction during the COVID-19 pandemic (approximately -15% in 2020), the projected growth until 2025 stands at around 18% (Statista 2022). Particularly noteworthy is the resilience of HR-tech companies offering a broad spectrum of services, which swiftly rebounded from the pandemic-induced downturn and are growing disproportionately compared to traditional HR firms (Statista 2022). The overall HR tech market is estimated at 62.6 billion U.S. dollars in 2022 and forecast to increase to 91.8 billion U.S. dollars by 2026 with a CAGR of 10.1 percent (Statista 2022). The market is dominated by incumbents (both specialized and unspecialized established HR Tech companies, which hold a market share of 91.9% in 2022 and are expected to retain a significant share (89.8%) in 2026. Many incumbents are connected to larger firms. For example, the online recruiting platform LinkedIn is owned by Microsoft and enjoys both the financial and institutional support of one of the original tech giants. Yet, the growth of startups is estimated with a CARG of 13.8% until 2026 outperforming incumbents (9.7%) significantly. This growth prospect for startups is driven by innovative firms particularly in Recruiting Software that offer a wider range of HR functions as incumbents are largely focused on personnel M&P and connectivity services (Statista 2022). However, the recruiting segment, exhibiting a significant market share of startups (25% in 2022), was impacted by geopolitical tensions and the associated macroeconomic effects including a tightening of the labor market. This impacts European HR Tech firms stronger than their US competitors (Statista 2022).
In conclusion, an examination of prevailing market trends reveals that the forefront of innovation and research and development (R&D) efforts predominantly resides within the domain of recruiting and talent management, a sector notably influenced by the initiatives of startups and smaller enterprises. Conversely, incumbents in the industry traditionally prioritize activities related to payroll management, which, prima facie, exhibit a lesser susceptibility to algorithmic discrimination. Consequently, given the focus of our project on investigating biases within automated decision-making systems (ADMS), the relevance of incumbent players in payroll management is deemed limited. Accordingly, our attention is directed towards HR Tech Startups like Talenteria, a startup specializing in recruiting HR technology, comprising fewer than 50 employees. Obviously, focussing on one firm poses challenges to the generalizability of our findings, however still might provide a first glimpse in both the quality and proneness to algorithmic biases of the services offered. It is imperative to recognize, however, that a comprehensive evaluation of biases within HR technology is currently impractical, primarily due to the nascent and dynamic nature of the market, largely characterized by the proliferation of young startups and a lack of consolidation.

  ## Literature Review 
_Introduction to Discrimination and Digital Ethics_
With the development of autonomous decision making systems, and its integration into our daily lives– particularly within the realm of human resource technology and global hiring practices, their impact grows ever more pronounced.  However, with the integration of these systems in society, arises the pressing questions regarding automotive systems, behavioral attributes and other ethical dilemmas. The autonomous systems trained by the HR tech ecosystem are anything but neutral, instead run the risk of perpetuating prejudices, stereotypes (Cave & Dihal, 2020; Drage & Mackereth, 2022). The consequence being the marginalization of communities. An expanding corpus of literature highlights the risks and challenges involved in the development of algorithms used for hiring with the apparent intention of mitigating biases. However, with the adoption of such technologies engenders significant repercussions in terms of inclusivity and intersectionality during the hiring process (Lee, 2018; Raghavan et al., 2020; Sánchez-Monedero et al., 2020; Benjamin, 2019). The increasing dependence on algorithms stems from their capacity to facilitate decision making, a pivotal factor driving their widespread adoption (Lee, 2018). Which raises the question regarding the reliability of these systems, and adopting a moral perspective focusing ethical considerations, inclusivity and equity. Given the importance of AI-driven HRM and its impact on society and the economy, there have been several projects on the nexus of ethics and HR Tech examined below. However, notably absent is a quantitative assessment of this issue.

_Literature Review on HR Tech and Ethics_
| Authors (Year) | Title | Main Findings | Methods | Discrimination Parameters |
|----------------|-------|---------------|---------|--------------------------|
| Rodgers et al (2023) | An artificial intelligence algorithmic approach to ethical decision-making in human resource management processes | Introduces a Throughput model framework illustrating decision-making in HRM settings, emphasizing the role of perceptions, judgments, and information use on strategy selection. Proposes that algorithmic pathways crucially shape HRM strategies. Explores implications of integrating AI into HRM practices, emphasizing the importance of considering algorithmic ethical positions. | Comprehensive literature review encompassing ethical dimensions and challenges of AI integration in HRM. Identifies key themes such as solutionism, the ripple effect, formalism, portability, and framing. Applies Throughput model to analyze decision-making processes and ethical considerations in AI-driven HRM. | gender, age, race, school attended |
| Martínez & Fernández (2020) | AI and recruiting software: Ethical and legal implications | Underscores AI algorithms' capacity to discern contentious attributes such as race, gender, and age, highlighting concerns regarding potential biases and discriminatory practices. Advocates for oversight and regulation of AI systems to ensure adherence to employment legislation and safeguard civil liberties. Proposes a multi-agent software framework for auditing HR operations, prioritizing transparency, impartiality, and inclusivity. | Literature review of existing literature on contentious features measured in image and voice processing using AI techniques. Analysis of machine learning techniques for face and pattern recognition in HR domain. Discussion of ethical and legal implications of using AI in recruiting, focusing on bias, discrimination, and compliance with employment laws. | physical attractiveness, age, race, gender, sex, origin, ethnicity |
| Gupta & Mishra (2022) | Ethical Concerns While Using Artificial Intelligence in Recruitment of Employees | Identifies two critical ethical dilemmas in integrating AI into recruitment: subconscious bias within AI algorithms stemming from human developer inputs, and the imperative of safeguarding data privacy to mitigate risk of discriminatory practices. Emphasizes addressing ethical considerations in AI-driven recruitment to enhance organizational effectiveness and societal trust. | Systematic literature review of ethical concerns in AI-driven recruitment. Gathering information from articles, dissertations, research papers, and online resources. Synthesis of existing literature to draw conclusions regarding ethical challenges encountered by organizations integrating AI into recruitment processes. | Gender |
| Upadhyay & Khandelwal (2018) | Applying artificial intelligence: implications for recruitment | Highlights AI technology's revolutionization of traditional recruitment practices, automation of repetitive tasks, and enhancement of efficiency. Emphasizes understanding AI tools to mitigate unconscious bias and optimize recruitment strategies. AI-powered systems can be programmed to ignore common sources of bias such as names, schools attended, gender, age, and race, ensuring fair and unbiased candidate screening based solely on qualifications, skills, and experiences. | Comprehensive literature review focused on synthesizing insights from various scholarly sources including reports, articles, research papers, and other relevant literature. | names, schools attended, gender, age, race |
| Köchling, & Wehner (2020) | Discriminated by an algorithm: a systematic review of discrimination and fairness by algorithmic decision-making in the context of HR recruitment and HR development | Highlights a critical gap in understanding drawbacks of algorithmic decision-making in HRM. Emphasizes insufficient attention to risks of discrimination and unfairness despite adoption of algorithms to reduce biases. Discusses potential biases in algorithms based on flawed input data, advocating for transparency in decision-making process. | Systematic literature review utilizing established approaches to identify relevant literature through databases and manual searches. Utilizes predefined categories for data synthesis guided by Preferred Reporting Items for Systematic Reviews (PRISMA) recommendations. Conducts robustness check to verify completeness of literature review. | gender, age, ethnicity, sex, sexism, origin |
| Criado & Such (2019) | Digital Discrimination | Explores instances of digital discrimination across various dimensions including gender, race, income, location, and lifestyle. Argues digital discrimination often reproduces existing discrimination in offline world. Highlights unresolved issues necessitating cross-disciplinary approach focusing on quantitative assessments to define non-discrimination norms in algorithms and datasets. | Literature review and synthesis of existing research on digital discrimination across various dimensions. Comprehensive examination of academic studies, reports, and empirical evidence. Discusses methodologies for detecting and addressing digital discrimination. | gender, race, income, location, lifestyle, sexual orientation |
| Meijerink et al (2021) | Algorithmic human resource management: Synthesizing developments and cross-disciplinary insights on digital HRM | Offers insights into implementation of algorithmic HRM in organizations transitioning to digital HRM. Explores impact of algorithmic HRM on worker status and employment relationships. Delves into ethical dimensions of algorithmic HRM, raising concerns about discrimination, bias, and privacy infringements. | Editorial leveraging insights from other researchers in special issue on HRM. | gender, ethnicity, age |
| Chen (2023) | Ethics and discrimination in artificial intelligence-enabled recruitment practices | Contends that while AI presents benefits for recruitment, its implementation raises concerns regarding discriminatory practices. Interviewees highlight potential bias stemming from partial data used by AI algorithms and user unfamiliarity with interface operations. Recommends technical and management measures to mitigate algorithmic bias in hiring processes. | Systematic literature review focusing on studies published between 2013 and 2023. Utilizes reputable academic databases for literature search. Conducts qualitative analysis of interview data grounded in Grounded Theory. | gender, race, skin color, personality, origin, nationality, age, education level |

## Origins of Discrimination
An increasing stream within literature endeavors to uncover the origins of algorithm biases in automated HR processes. While specific studies on this aspect of HR are scarce, we can draw insights from broader trends that explain algorithm biases. In a review of this topic, the GreenLining Institute (2021) identifies five main reasons that elucidate the occurrence of these algorithm biases and can be applied to HR processes. Firstly, data biases pose a significant challenge in HR algorithms as the algorithms learn from previous hiring data, which may inherently be discriminatory. If the previous hiring decisions exhibited a bias towards male candidates, the algorithm trained on such data might favor male candidates, perpetuating gender bias in the hiring process. Algorithm Design Choices also attenuate biases when designing algorithms for HR applications. The developer’s decision when defining selection criteria or predicting job performance can introduce biases. Subjective judgements in algorithm design may favor certain demographic characteristics over others, leading to discriminatory outcomes. Implicit biases among developers further compound the issue of algorithmic biases. 
Furthermore implicit biases among developers may compound the issue of algorithmic bias in HR processes. These unconscious biases can inadvertently affect decision making during algorithm design and development, contributing to discrimination during candidate selection. Feedback loops in HR algorithms also contribute to the reinforcement of biases over time. If an algorithm consistently recommends candidates from certain demographic groups for certain job roles, it may continue to perpetuate stereotypes, leading to underrepresentation of certain groups in the workforce. Finally the lack of regulation and oversight in the development and deployment of HR algorithms contribute to this problem. In the absence of proper guidelines and monitoring, developers may not prioritize fairness and equity in algorithmic decision making procedures related to hiring, promotion or performance evaluation. This dearth of oversight can continue the biases in HR practices, hindering diversity and inclusivity in the workforce. 

## Digital Ethics Issues in Practice

### _Legal Landscape_
The issue of discrimination stemming from biased HRM Tech also raises substantive practical concerns and has attracted the attention of regulatory bodies. In response, regulatory frameworks have been enacted, particularly in the domain of labor law, aimed at mitigating the societal repercussions of presumed discriminatory practices. Furthermore, these regulations serve to corroborate the findings of the literature review from a practical standpoint. Consequently, adherence to non-discrimination statutes becomes imperative for AI-driven decision-making processes. It is imperative to acknowledge that biases inherent in training data or algorithmic design have the potential to inadvertently perpetuate discriminatory outcomes. Within this regulatory landscape, two pivotal legislative enactments emerge, which provide insight in relevant discriminatory parameters and the relevance of this issue as a whole, thus, informing our methodology.

### _The German Allgemeines Gleichbehandlungsgesetz/General Equal Treatment Act (AGG)_
The regulation assesses that direct or indirect discrimination, as defined by Sections 3(1) or 3(2) of the General Equal Treatment Act (AGG), may occur in recruiting practices (Mückl and Hillu 2024). Therefore, the German parliament has standardized various parameters of discrimination, which are presumed to occur regularly and are normatively assumed to be incompatible with fundamental values of fairness and discrimination protection. §1 defines the characteristics by the AGG to be protected as "race or ethnicity, gender, religion or belief, disability, age, or sexual identity."

### _Analysis of Real-World Digital-Ethical Incidents based on The AI Incidents Database (AIIIDB)_
Turning to practical examples of the issue of the societal consequences of AI, the deployment of AI frequently leads to incidents known as digital-ethical incidents (DEIs), which have significant implications for both companies and society. The strategic importance for companies, which are by far the most prone to facilitate this kind of incidents and discrimination, of this issue is highlighted by a notable shift in responsibility, as non-technical executives now emerge as the primary persons in charge for AI ethics. This role has expanded significantly, rising from 15% in 2018 to 80% in 2022. Notably, 28% of surveyed executives now assert that AI ethics falls under the purview of the CEO, with 79% of CEOs indicating preparedness to act – an impressive increase from the previous 20% (IBM 2022). The analysis, based on the AI Incidents Database (AIIDB), reveals that these DEIs are primarily concentrated in the Tech sector (47%), followed by Automotive (14%) and Public (14%, Exh. 6). This, thus, justifies our focus on roles with a technical background, i.e. a software developer role. Furthermore, the registered instances of DEIs have seen a considerable increase since 2019 aligning again with the finding in the literature like Köchling and Wehner (2020) as well as Chen (2023). Reasons for DEIs stem from both dysfunctional (47% of cases) and discriminatory technologies (25%). However, organizations exhibit varying degrees of awareness and attentiveness to HR-AI incidents, with deliberateness (25%) and accidentality (75%) emerging as critical factors influencing the nature and impact of these incidents.


<p align="center">
 <img src="https://github.com/DBIA2023/DecodingBiasesinAI_grp5/assets/169889828/c29c8952-eee6-4f08-b76c-52c313282edf" alt= "Exhibit 2: _DEI segemented by sector of development" >

<p/>
 
<p align="center"><b>Exhibit 2: DEI segmented by sector of development</b></p>
