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
Turning to practical examples of the issue of the societal consequences of AI, the deployment of AI frequently leads to incidents known as digital-ethical incidents (DEIs), which have significant implications for both companies and society. The strategic importance for companies, which are by far the most prone to facilitate this kind of incidents and discrimination, of this issue is highlighted by a notable shift in responsibility, as non-technical executives now emerge as the primary persons in charge for AI ethics. This role has expanded significantly, rising from 15% in 2018 to 80% in 2022. Notably, 28% of surveyed executives now assert that AI ethics falls under the purview of the CEO, with 79% of CEOs indicating preparedness to act – an impressive increase from the previous 20% (IBM 2022). The analysis, based on the AI Incidents Database (AIIDB), reveals that these DEIs are primarily concentrated in the Tech sector (47%), followed by Automotive (14%) and Public (14%, Exh. 2). This, thus, justifies our focus on roles with a technical background, i.e. a software developer role. Furthermore, the registered instances of DEIs have seen a considerable increase since 2019 aligning again with the finding in the literature like Köchling and Wehner (2020) as well as Chen (2023). Reasons for DEIs stem from both dysfunctional (47% of cases) and discriminatory technologies (25%). However, organizations exhibit varying degrees of awareness and attentiveness to HR-AI incidents, with deliberateness (25%) and accidentality (75%) emerging as critical factors influencing the nature and impact of these incidents.

<p align="center"><b>Exhibit 2: DEI segmented by sector of development</b></p>
<p align="center">
 <img src="https://github.com/DBIA2023/DecodingBiasesinAI_grp5/assets/169889828/1a34f33a-f01e-4626-bfd8-0d41a9541b92" alt= "Exhibit 2: _DEI segemented by sector of development" >
<p/> 

### _Conclusion of Literature Review and Real-World Digital Ethical Incidents_
The issue of DEIs and AI-facilitated discrimination also entails HR Tech with DEIs in HR surging since 2018 (Exh. 3). Out of the 373 DEIs related to specific application domains, approximately 10% pertain to HR applications (Exh. 4). The risks associated with discriminatory or malfunctioning HR technology are notably heightened in the recruitment process (58%), as evidenced by incidents of application rejection due to gender discrimination (Exh. 10). Thus, our analysis focusses on recruitment technology as this part of HR Tech is – based both on our literature review and the AIIDB analyzed - the most prone to discrimination issues and bias. A survey conducted by a Harvard Business School team encompassing over 2,250 executives in the US, UK, and Germany revealed that the primary motivations for utilizing algorithmic tools were efficiency and cost savings. However, a striking 88% of executives acknowledged that their tools were rejecting qualified applicants, a figure that surged to 94% for middle-skilled workers (Fuller et al. 2021). A prominent example is Amazon's biased recruiting system in 2018, which systematically rejected qualified female applicants based on training data biased towards male employees. However, instances of discrimination based on parameters such as age, origin, immigrant status, and religion resulting in different kinds of harm (. 


| ![Exhibit 3: Culminated Development of DEIs in HR as of 03/2023](https://github.com/DBIA2023/DecodingBiasesinAI_grp5/assets/169889828/b881d0f7-4903-437e-9b2d-6c08d8c0ae2f) | ![Exhibit 4: DEI segmented by scope of Application](https://github.com/DBIA2023/DecodingBiasesinAI_grp5/assets/169889828/1fbaf189-bac7-46c0-af64-564e9ccbf33f) |
|:--:|:--:|
| **Exhibit 3: Culminated Development of DEIs in HR as of 03/2023** | **Exhibit 4: DEI segmented by scope of Application** |

### _Limitations and Research Gaps_
Consistent with the observations made by Köchling and Wehner (2020) as well as Chen (2023), our literature review highlights a notable dearth of quantitative investigations pertaining to the potential adverse implications, such as biases and discriminatory practices, within the realm of HRM Tech. To address this lacuna, our study aims to bridge this research gap by undertaking a quantitative inquiry into HRM technology, with a specific emphasis on the recruitment domain, particularly the utilization of curriculum vitae (CV) screening procedures. Our scrutiny of extant literature reveals a conspicuous susceptibility to discriminatory practices within this domain. A recurring thematic concern across the reviewed literature is the discussion and documentation of discriminatory incidents, predominantly centered on gender biases. Furthermore, considerations related to age, as well as peripheral discussions surrounding race, ethnicity, and origin, occasionally inferred through proxies such as nomenclature and educational background, also emerge as pertinent themes. These findings align with the exhaustive systematic literature reviews conducted by Köchling and Wehner (2020) and Chen (2023), which collectively encompassed an analysis of over 3,500 scholarly articles within this domain. Subsequently, these identified parameters are further corroborated by real-world instances elucidated in subsequent sections of our discourse. Consequently, the synthesis of insights garnered from the literature review, alongside the parameters elucidated through a cursory examination of the regulatory landscape and quantitative analysis of case studies, informs the methodological framework of our study. This methodology is characterized by a concentrated emphasis on (1) the recruitment process, specifically the screening of curriculum vitae, and (2) the quantitative examination of discriminatory parameters, i.e. (a) gender, (b) age, (c) ethnicity and (d) origin.

## Qualitative Analysis

### Methodology 
Following advancements in Human Resources technologies, our research aims to uncover biases in CV screening software bolstered by AI. Despite claims of improved efficiency and unbiased selection processes by these new tools, we aim to test this assertion. Thus, we aim to check quantitatively the following hypotheses:
- Null Hypothesis: Talenteria CV assessment scores are independent of age, gender, ethnicity & origin.
- Null Hypothesis 1: Talenteria CV assessment scores are affected by candidate age.
- Null Hypothesis 2: Talenteria CV assessment scores are affected by candidate gender
- Null Hypothesis 3: Talenteria CV assessment scores are affected by candidate ethnicity.
- Null Hypothesis 4: Talenteria CV assessment scores are affected by candidate origin.

These hypotheses will help us investigate whether age, gender, ethnicity, or origin have any discernible impact on CV assessment scores within AI-driven CV screening software.

### Case Selection 
The first step was to choose un the specific software we will test. The tradeoff was to find software that has a significant presence in the market, which is primarily shaped by US startups and not yet consolidated with many new players emerging, and, at the same time, is affordable. We have chosen Talenteria. Talenteria is a CV screening tool that, as its webpage states, utilizes AI to score a talent pool in relation to suitable job searching criteria, enhancing recruitment reach and efficiency. It is highlighted that AI scoring is based only on candidate experience, skills, and education. In summary, they offer to reduce 75% of recruiters' time and remove bias with AI-powered resume screening and scoring. Other features of the tool can be found on the webpage talenteria.com. The chosen software also has a high reach within the industry, as it is embedded in an all-in-one HCM system for medium and large businesses - Lanteria HR, which has over 200K users in 40+ countries. Some well-known customers of the platform are Lufthansa, Warner, Leica, among others. A final advantage is that despite the high price tag of the software (over EUR 500 per month), we could access a free trial, with limitations in time but not in functionalities.
	A second decision for managing the scope of the research is determining the specific profile of workers we will test within the screening process. This is important because the software has flexible search rules, and candidates are evaluated based on sought-after abilities related to specific tasks of the future laborer. Based on the insights gleaned from our assessment of the AIIDB, which has indicated that a majority of discriminatory events and incidents (DEIs) occur within the technology sector, we have opted for a software development role as the designated profile for our testing endeavors. This choice aligns with the archetype profile prevalent within the sector. The sought profile is illustrated in Box 1.

```
Title: Software Developer
Description: We are currently seeking a talented and dedicated Software Engineer to become an integral member of our innovative technology team. The ideal candidate will have a passion for creating cutting-edge software solutions, demonstrate strong problem-solving skills, and have a solid understanding of computer science principles. This role involves collaborating with other engineers, developers, and stakeholders to develop, test, and maintain software applications that meet the needs and expectations of our clients. If you have a knack for tackling complex technical challenges and desire to work in a dynamic, fast-paced environment, we would love to hear from you.
Department: Product
Job Category: Technology and Science
Responsibilities:
1. Design, develop, and implement software solutions based on system specifications and other stakeholder requirements.
2. Write clean, maintainable, and well-documented code adhering to industry standards and best practices.
3. Collaborate with cross-functional teams, including product managers, designers, and other engineers, to define and shape the features and products.
4. Participate in code reviews to ensure code quality and mentor junior developers in software engineering techniques and principles.
5. Troubleshoot, debug, and upgrade existing systems to improve performance and resolve any issues that arise in the software.
6. Continuously learn and incorporate new technologies and methodologies to stay current in the field and enhance the software development practices within the organization.
Requirements:
1. Bachelor’s degree in Computer Science, Engineering, or a related technical field, or equivalent work experience.
2. At least 2 years of professional software development experience with proficiency in one or more programming languages (e.g., Java, C++, Python, JavaScript).
3. Solid understanding of object-oriented design, data structures, and algorithms.
4. Experience with the full software development lifecycle, including requirements gathering, design, coding, testing, and deployment.
5. Familiarity with software engineering tools and best practices (e.g., Git, unit testing, continuous integration, code reviews).
6. Exceptional problem-solving skills and the ability to work independently or as part of a team to meet project deadlines.
Employment Type: FULL-TIME
Location / City: Seattle
```

Box 1: Profile of the sought worker

### Data Gathering 
As we aim to unveil potential AI biases in the CVs screening software, the most focalized way is by controlling the inputs we provide to the software. For this purpose, we constructed numerous fake CVs that vary only in the variables we aim to test within our hypothesis, i.e. age, gender, and ethnicity.  Then, we use a common root for every CV, which is stated in Box 2.

```
Curriculum Vitae 
Name: [Varies by candidate]
Age: [Varies by candidate]
Email: [Name]@gmail.com 
Summary: Software Developer with 4 years of experience in developing web and mobile applications. Proficient in a range of programming languages, with a focus on frontend development. Eager to join a dynamic team where I can contribute to developing innovative software solutions. 
Education: Software Engineer, University: [varies by candidate] 
Experience: 
Software Developer 
Company: NextGen Apps Dates: 01 Jan 2021 – 28 Feb 2024 (3 years) 
Junior Developer 
Company: WebWorld Technologies Dates: 29 Dec 2019 – 30 Dec 2020 (1 year)
```

Box 2: Common root for fake CVs

By using common root, we input:

- Name: We prompted ChatGPT to provide the most common combination of first and last names by different ethnicities: White, Latino, African, and Asian. We used a balanced sample per ethnicity and gender. The sample was revised by hand, and we didn't use genderless names. Then, we randomly selected a name per candidate, and we marked in our database the ethnicity and gender associated with such iteration.
- Age:  We randomized every iteration with age between 25 and 59 years old.
- University: We used the university to double-check the influence of ethnicity in terms of the candidate's geographical origin. We faced the challenge of selecting universities from different parts of the world that provide the same level of education. Therefore, we chose universities within the range of 93 to 103 in the QS ranking, encompassing institutions from the US, Europe, Latin America, and Asia. The university was then randomly assigned through iteration.

After tailoring the CVs, we uploaded them to the platform and gathered the scores associated with each candidate. We performed this process five times: initially randomizing all variables by iteration, and then varying single variables individually to ensure a robust analysis. Then we gathered data by uploading the same CV 100 times, but changing the email, in order to check we are not receiving random scores.

| Dataset                    | Date Gathered | N (CVs) | Varying Variables       |
|----------------------------|---------------|---------|--------------------------|
| Dataset 1 (main study)     | 26.04.23      | 300     | Name (gender, ethnicity) |
|                            |               |         | Age                      |
|                            |               |         | University Name (geographical origin) |
| Dataset 2 (robustness)     | 09.05.23      | 100     | Age                      |
| Dataset 3 (robustness)     | 09.05.23      | 100     | Name (gender, ethnicity) |
| Dataset 4 (robustness)     | 09.05.23      | 100     | University Name (geographical origin) |
| Dataset 5 (robustness)     | 09.05.23      | 100     | No variation             |

Table 1: Overview of the data gathered


### Linear Regression 
After gathering our data, we performed an Ordinary Least Squares regression (OLS) to examine the influence of age, gender, and ethnicity on the candidates' scores. While our analysis doesn't establish causality, it indicates the significance of the statistical correlations, serving as an initial step for a causal study. Our full model is stated in Equation 1. Additionally, to check for algorithmic bias within the software, we expect that each regressor associated with our independent variables (age, gender, ethnicity, and origin) is not significant

<p align="center">
 <img src="https://github.com/DBIA2023/DecodingBiasesinAI_grp5/assets/169889828/fa5219c6-732a-4160-8ab3-e6986581bef5" alt= "Equation 1: _OLS Model", width= 768 length=361 >

<p/>
 
<p align="center"><b>Equation 1: OLS Model</b></p>

## Results 

### Main Results 

The analysis of Dataset 1, our primary dataset where all independent variables vary, reveals only marginal differences in CV scores across variation in our demographic factors, namely, name, age, and university of origin. 80% of the submitted CVs receive a score of 5.87/10, 12% a score of 6.20/10, and 6.3% a score of 5.53/10 (see exh 5). This suggests that name (and thus ethnicity and gender), age, and university of origin only have limited impact on the overall score, indicating a small effect size. It also reflects discretional jumps when variables vary.

<p align="center">
 <img src="https://github.com/DBIA2023/DecodingBiasesinAI_grp5/assets/169889828/31c14fae-bcb3-4d6f-b251-34a400128d5b" alt= "Exhibit 5: _Distribution of Scores, Dataset 1 (main study)" >

<p/>
 
<p align="center"><b>Exhibit 5: Distribution of Scores, Dataset 1 (Main Study)</b></p>

Yet, in order to account for the small observed variation in scores, we conducted OLS regression analysis and compared differences in average score for each category of each variable (see exh 5). While the distribution of scores approximated a normal distribution (see exh 5), a Shapiro test revealed deviations from normality assumptions. Nevertheless collinearity issues were not detected. We ran three regression models. After running Model A, the baseline, we enhanced the model by introducing additional variables. This involved disaggregating variables such as Global South and Global North into dummy variables for each respective university (Model B), as well as creating dummy age categories (Model C). This refinement significantly improved the fit of the model. For an overview of the results see table xyz.
Concretely, our regression models highlighted that the effects (1) of the majority of the variables on score are not significant, and (2) that the variables whose effect is significant contradict our initial hypothesis. First gender, age and geographical origin (Global North/South) did not significantly influence scores at the conventional significance level of 0.05. This also makes sense given that a comparison of mean score for each category of those variables highlighted a variation of average score of only 0.1 score points (see figure xyz). Candidates of African descent exhibited a statistically significant, albeit weak, positive effect on average scores, contrasting with the non-significance of other ethnicities (see figure xyz). This is surprising given that recruitment discrimination based on “global south” ethnicities is a recurring theme in the academic literature which however is largely qualitative. However, also our analysis of cases in the AIIB - from the cases collected in the database which relies on media coverage - empirically substantiates this claim.

<p align="center">
 <img src="https://github.com/DBIA2023/DecodingBiasesinAI_grp5/assets/169889828/abcb6fb7-49d6-4904-b469-da8ef223a987" alt= "Exhibit 6: _Varaition in mean scores for each (Dataset 1, Mainstudy)" >

<p/>
 
<p align="center"><b>Exhibit 6: Varaition in mean scores for each (Dataset 1, Mainstudy)</b></p>

<p align="center">
<img src="https://github.com/DBIA2023/DecodingBiasesinAI_grp5/assets/169889828/15172270-5a04-462e-ac44-35c31207bc41" alt= "Exhibit 7: _ Variation of mean score given university country (Dataset 1, Mainstudy)" >

<p/>
 
<p align="center"><b>Exhibit 7:  Variation of mean score given university country (Dataset 1, Mainstudy)</b></p>

Further, dissecting the data - that is the global region - by university of origin revealed surprising effects. While variation in mean scores were generally subtle, they reached up to 0.2 score points across universities (see exh 7). Unexpectedly, graduates from Freie Universität Berlin exhibited a weak, yet significant, negative association with CV scores, while Purdue University graduates in the US showed a similarly weak, but positive, effect (see exh 7). 

|                     |     A     |     B     |     C     |
|---------------------|-----------|-----------|-----------|
| Constant            | 5.8773*** | 5.9427*** | 5.9161*** |
|                     |   (0.041) |   (0.042) |   (0.031) |
| Men                 |   0.0087  |  -0.0256  |  -0.0273* |
|                     |   (0.018) |   (0.016) |   (0.016) |
| Latino              |   0.0099  |   0.0041  |   0.0069  |
|                     |   (0.024) |   (0.021) |   (0.021) |
| Asian               |   0.0100  |   0.0195  |   0.0144  |
|                     |   (0.024) |   (0.021) |   (0.021) |
| African             |  0.0683***|  0.0504***|  0.0497***|
|                     |   (0.024) |   (0.021) |   (0.021) |
| Age                 |  -0.0004  |  -0.0008  |           |
|                     |   (0.001) |   (0.001) |           |
| 20-29               |           |           |   0.0073  |
|                     |           |           |   (0.023) |
| 30-39               |           |           |   0.0246  |
|                     |           |           |   (0.021) |
| 40-49               |           |           |  -0.0352* |
|                     |           |           |   (0.021) |
| Uni Global South    |   0.0232  |           |           |
|                     |   (0.017) |           |           |
| Freie Universität   |           |  -0.1873***|  -0.1914***|
| Berlin, GER         |           |   (0.031) |   (0.031) |
| POSTECH, South Korea|           |  -0.0233  |  -0.0263  |
|                     |           |   (0.033) |   (0.033) |
| UC, Chile           |           |   0.0448  |   0.0428  |
|                     |           |   (0.031) |   (0.031) |
| Purdue University,  |           |   0.0832**|   0.0790**|
| US                  |           |   (0.034) |   (0.034) |
| R-Squared           |   0.039   |   0.019   |   0.275   |
| Adjusted R-Squared  |   0.019   |   0.245   |   0.260   |
| F-Statistic         |   1.962   |   9.026   |   8.459   |

- *,**,*** indicates significance at 90%, 95% and 99% respectively
- Standard error is reported in the brackets 
Table 2: Regression results for candidate CV scores

To summarize, despite the average consistency in scores across the tested demographic variables, some (sub-categories) of our demographic variables have a statistically significant effect across models. However, they seem somewhat arbitrary: Why should Freie Universität Berlin graduates be discriminated against? And why do we find - contrary to our assumptions (and maybe biases) that candidates from African descent do (marginally) better? Further, we notice that there is “random” variation at the individual level: For instance, we observe identical CVs - across all variables - receiving different scores, further suggesting potential arbitrariness in Talenterias CV assessment algorithm. Given these unexpected results, we thus deem it crucial to conduct a robustness check. 

### Robustness examination 
As further elaborated on in the methodology, we conducted a robustness examination focusing on isolating the effects of name (ethnicity and gender), age, and country of origin on the 9th of May. Thus, we created CVs with random selection of only one variable of those categories (See methodology above) and we gather 3 different dataset, one per independent variable, The choice was made to disentangle potential interactions between these variables and to validate the repeatability of our main study results. The results of our robustness check revealed notable discrepancies compared to our initial study. A striking observation was the substantial alteration in summary statistics of the score distribution (see table 3 for summary statistics and exh 8 for visualization). Notably, the median score shifted from 5.87 in the initial study to 7.33 in the robustness study, accompanied by significantly higher standard deviations. This strong change in scores occurred despite CVs being identical to the initial studies - and only one variable varying respectively. Particularly the increased standard deviation is surprising. In fact, our robustness examination included the submission of 100 identical CVs (see Dataset 5), which yielded the highest standard deviation (0.0938) and the widest range (6.66).
Hence, it seems that the algorithm of Talenteria changed between the 26.04.23 and the 09.05.23. Particularly striking was the substantial increase in standard deviation (and range) of scores, particularly evident in the scenario with no variation in submitted CVs. Given that in HR practices one seeks consistent and fair assessment of candidates, the significant alteration of the Talenteria algorithm between the initial study and the robustness check has to be assessed critically. Further, even at a given moment in time, we observe - especially in the robustness study - large variation in scores despite identical CV submissions. We will now continue to analyze whether these variations can be attributed to the variables we manipulated. Second, the (difference in) variation in CV scores we observe in each dataset can not be attributed to (1) age variation and (2) name variation. Concretely, for each dataset we compared the mean score for each category (see exh 9). For Dataset 2 - where we manipulated age - and Dataset 3 - where we manipulated name and thus gender and ethnicity, mean score for each respective age, gender or ethnicity category does not vary significantly: All scores being close to 7.5. We verified this by having non significant regressors in our respective OLS models. Again, on average, score variation is small, while on the individual level identical candidates might receive strongly differing results. 
The variation in average scores given university of origin is higher, ranging from 8.7 for graduates of Purdue University (US) to 7.2 for Freie Universität Berlin (Germany). While acknowledging the limitations of our sample size, our regression analysis corroborated the significant effects of graduation from specific universities, such as POSTECH in South Korea (positive effect) and Freie Universität Berlin (negative effect), aligning with our initial study findings (see table 4).

|         |   N   | Mean | Median |  Std  | Range |
|---------|-------|------|--------|-------|-------|
| Dataset 1 (All variation) |  300  | 5.88 |  5.87  | 0.155 |  1.2  |
| Dataset 2 (Age variation) |  100  | 7.51 |  7.33  | 0.686 | 2.56  |
| Dataset 3 (Name variation) |  100  | 7.42 |  7.33  | 0.738 | 2.56  |
| Dataset 4 (Uni variation) |  100  | 7.73 |  7.33  | 0.819 | 2.56  |
| Dataset 5 (No variation) |  100  | 7.48 |  7.33  | 0.938 | 6.66  |

Table 3: Summary statistics for score for each dataset

![exhibit 8](https://github.com/DBIA2023/DecodingBiasesinAI_grp5/assets/169889828/e9cc6f00-d9fd-401f-94cf-76ae9b00365a)

<p align="center">
<img src="https://github.com/DBIA2023/DecodingBiasesinAI_grp5/assets/169889828/e9cc6f00-d9fd-401f-94cf-76ae9b00365a" alt= "Exhibit 8: _Distribution of scores for each robustness study" >

<p/>
 
<p align="center"><b>Exhibit 8:  Distribution of scores for each robustness study (Dataset 1, Mainstudy)</b></p>

