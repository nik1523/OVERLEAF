\documentclass[12pt]{report}	
%Doccument Class Specification
\setlength{\textwidth}{6.25in} % original 6.25 %Text Lenght SetUp
\setlength{\textheight}{8in}

\renewcommand{\baselinestretch}{1.3}	%Page Margin SetUp
\oddsidemargin 20pt    %  Left margin on odd-numbered pages.
\evensidemargin 20pt   %  Note that \oddsidemargin = \evensidemargin
\topmargin 0pt
\newcommand{\squeezeup}{\vspace{-0.6cm}}
%\renewcommand{\tableofcontents}{INDEX} 
\renewcommand*\contentsname{INDEX}
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
% Define Packages
\usepackage {graphics}
\usepackage {epsfig}

\usepackage{listing}
\usepackage{subcaption}
\usepackage[table,xcdraw]{xcolor}
\usepackage {graphicx}
\usepackage{titlesec}
%\usepackage{hyperref}
\usepackage{acronym}
\usepackage{url}
\usepackage{fancyhdr}
\usepackage{float}
\usepackage{fancybox}
\usepackage{xcolor}
\usepackage[left=3.81cm,top=2.54cm,right=2.54cm,bottom=3.175cm]{geometry}
\usepackage{pdfpages}
\usepackage[font=normalsize,labelfont=bf]{caption}


%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%Change Font Size Of Titles
\titleformat{\chapter}[display]
{\normalfont\large\bfseries\centering}{\chaptertitlename\ \thechapter}{14pt}{\large}
\titleformat{\section}{\normalsize \bfseries}{\thesection}{1em}{}
\titleformat{\subsection}{\normalsize \bfseries}{\thesubsection}{1em}{}
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
% Begin document "environment".


\begin{document}
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
	
%Title Page
	\begin{titlepage}   
\thisfancypage{\setlength{\fboxsep}{10pt}\doublebox}{}
		\vspace*{0.1in}
		\begin{center}
        { \bf {Academic Year 2023-24 }}\\
		%{ \bf {REPORT ON}}\\
		{ \bf {A REPORT ON}}\\
		%{ \bf {REPORT ON}}\\
		\vspace{0.2in}
		{\Large \bf {Analysis of the Effect of An ''Artificial Intelligence Chatbot', on Educational Program}}
		\\
		\vspace{0.2in}
{ Submitted by.}\\
{ \Large \bf Mr. Anurag Sanjay Jadhav}\\
{ of T.E. (Computer Engineering- Course 2019) having Examination Roll No. 13171 in partial fulfillment for the award of degree Bachelor of Engineering in Computer Engineering for Academic Year 2023-2024
}\\
\vspace{0.2in}
{\bf   Under the guidance of}\\
{\bf \Large \bf Prof.Shivaji Patil Sir}\\
		\vspace{0.2in}
	
		
		\begin{figure*}[h]
		\centerline{\psfig{figure=./collegelogo.jpg,width=1.4in,height=1.4in}}
		\label{atcres}
		\end{figure*}
		\vspace{0.2in}
		
		{\large \bf{ COMPUTER TECHNOLOGY DEPARTMENT}}\\ 
		{ \bf  Dr.D.Y.Patil College of Engineering  and Innovation,}\\ 
		{\bf  Varale, Talegaon,410507, India}\\ 
		\small{2023-2024}
		\end{center}
	\end{titlepage}
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

%Certificate
	\thisfancypage{\setlength{\fboxsep}{10pt}\doublebox}{}	
	\begin{titlepage}
		\begin{center}
		\begin{figure*}[h]
		\centerline{\psfig{figure=./collegelogo.jpg,width=1.4in,height=1.4in}}
		\label{atcres}
		\end{figure*}
		{\large \bf{ COMPUTER ENGINEERING}}\\
		{ \bf  Dr.D.Y.Patil College of Engineering  and Innovation}\\ 
		{\bf  Varale, Talegaon,410507, India}\\ 
		\vspace{0.2in}
		{\large\textbf{CERTIFICATE}}\\
		{\small This is to certify that report on }\\
		\vspace{0.2in}
		{\large \bf {“Analysis Of The Effect Of An Artificial Intelligence Chatbot on educational program”}}\\
		\vspace{0.2in}
%		{\small Enrollment No: 1700800160  }\\
		Submitted By  Mr. Anurag Sanjay Jadhav , of Third Year having Roll No. 13171, Div-A is a bonafide work completed under my supervision and guidance in partial fulfillment for award of degree of Bachelor of Engineering in the branch Computer Engineering of Dr. DY Patil College Of Engineering and Innovation
, Varale, Talegaon.\\ 

		\end{center}
	
		\vspace*{0.2in}
		\begin{table}[h]
		\begin{tabular}{clcll}
			\large \bf Prof.Shivaji Patil					& \hspace*{2.0in} & \large \bf Prof.Anita Shinkar &  &  \\
			(Seminar Guide)                      & 				& (Seminar Co-ordinator)                              &  &  \\
			           DYPCOEI, Varale.  &  				&  DYPCOEI, Varale.           &  &  \\
			                     & 				&                     &  & 
		\end{tabular}
		\end{table}

		\vspace*{0.2in}
		\begin{table}[h]
		\begin{tabular}{clcll}
			\large \bf Prof.Alpana Adsul	 					& \hspace*{1.9in} & \large \bf Prof.Suresh Mali &  &  \\
			(HOD Comp)          & 		& Principal                               &  &  \\
			DYPCOEI, Varale.                     & 				& DYPCOEI, Varale.                    &  & 
		\end{tabular}
		\end{table}
		
		\hspace*{0.4in}Place: Varale,Talegaon,Pune\\
		\hspace*{0.65in}Date:
	\end{titlepage}

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%


%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

\pagenumbering{roman} %Roman PageNumbers

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
% Acknowledgement
\thisfancypage{\setlength{\fboxsep}{10pt}\ovalbox }{}
\addcontentsline{toc}{chapter}{Acknowledgement}
\chapter*{ACKNOWLEDGEMENT}

\hspace*{0.3in}I would like to express my special thanks of gratitude to my internal guide 
  \textbf{Prof. Shivaji Patil} well as {\textbf{Prof. Alpana Adsul}, Head of Department who gave me the golden opportunity to do this seminar on the topic \textbf{“Analysis of the Effect of An Artificial Intelligence Chatbot Educational Program”}, which also helped me in doing so many new things.\\

\hspace*{0.3in}While doing this seminar, I had to take the help and guideline of some respected persons, who deserve our greatest gratitude. The completion of this seminar gives me much Pleasure. I would like to show our gratitude Prof.Shivaji Patil, Seminar Coordinator for giving me a good guideline for seminar throughout numerous consultations. I would also like to expand my deepest gratitude to all those who have directly and indirectly guided me in completing this seminar. Secondly, I would like to thank my friends for helping me with this seminar within the limited time frame\\ 

\hspace*{0.3in}I also extend sincere thanks to all the staff members of Department of Computer Engineering and Principal Suresh Mali, for helping me in various aspects.\\
\vspace{30mm} 
\begin{flushright}



\begin{minipage}{2.7 in}
\textbf{\large\bf Mr.Anurag Sanjay Jadhav}\\
CLASS: TE (Computer Engineering) 
ROLL NO: 13171
\\
 \end{minipage}\hfill
\end{flushright}


\newpage
%%%%%%%%%%%%
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

%Default Pages - Table of Content
\newpage
\thisfancypage{\setlength{\fboxsep}{10pt}\Ovalbox }{}
\addcontentsline{toc}{chapter}{Index}
\tableofcontents
\newpage
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

%Synopsis
\newpage 
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

\newpage
\pagenumbering{arabic}		%Page Numbering For Main Document

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

%Header And Footer
\fancyhf{}
\fancyhead[LE]{\leftmark}
\rhead[RO]{\scriptsize{}}
\cfoot[LE,RO]{\thepage\\\scriptsize{Dr.D.Y.Patil College of Engineering And Innovation ,Computer Engineering Department - 2023-2024}}
\pagestyle{fancy}
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
\newpage
\thisfancypage{\setlength{\fboxsep}{10pt}\ovalbox }{}
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

%Default Pages
\addcontentsline{toc}{chapter}{List of Figures}
\listoffigures

\newpage
\thisfancypage{\setlength{\fboxsep}{10pt}\fbox }{}
\chapter{Introduction}
\section{Introduction}
\hspace*{0.3in}\\  Along with the development of technology, such as big data, machine learning, and artificial intelligence (AI), intelligent services have been actively introduced in the field of information technology. AI has been initiated in clinical practice and nursing education because of the restrictions in education caused by the coronavirus disease (COVID-19) pandemic [1]. Moreover, conventional lessons have been converted into video lectures and non-face-to-face lessons. Thus, strategies for improving students’ self-directed learning, and efforts for promoting interactions between instructors and students are needed. This has led to a growing interest in using chatbots in the education field. A chatbot—also referred to as “a talking bot”—is a type of a software prominently emerging in the information technology feld [2], that can have verbal or written conversations with human users, and address their requests, using the question-and answer format [3].
   

\begin{figure}[htbp]
\captionsetup{font=scriptsize}
\centering {\includegraphics[width=2.9in, height=2.0in]{istock.jpg}}
\caption{Introduction.}
\label{fig}
\end{figure}

\newpage
\thisfancypage{\setlength{\fboxsep}{10pt}\fbox }{}
A chat bot also has various applications in the education field, as people can use it to learn without time and space restrictions [4]. It also improves the effect of self-directed learning as learners experience low levels of stress while engaging in conversations with a chat bot and repeated learning [5]. Furthermore, it facilitates immediate user feedback through conversations during the learning process, and provides customized contents based on the feedback [6]. Therefore, through AI technology, a chat bot can provide education to those who are unable to seek help from instructors because of problems, such as cost, manpower, and the COVID-19 pandemic [1, 7]. 
\thisfancypage{\setlength{\fboxsep}{10pt}\fbox }{}
\section {Background}
\hspace*{0.3in}Electronic fetal monitoring (EFM) involves attaching a device to the abdominal wall of pregnant women to continuously monitor and record fetal heart sounds through graphs. It is utilized to prevent fetal hypoxia and provide interventions at an early stage by observing changes in fetal heartbeat [8]. As a noninvasive method to assess fetal health, EFM is widely used in the obstetrics field [8]. However, it is difficult to interpret the graphs, which have been found to have low specifically, compared with the level of sensitivity [9]. Tus, healthcare providers and nursing students should be able to accurately install the device, interpret the graphs, and report abnormal patterns to the doctors. Regarding essential nursing techniques in maternal health nursing, education on installing EFM equipment and interpreting its results is required [10]. Additionally, during their training in the delivery room, nursing students learn about measuring vital signs (57.5), supportive touch in the frst stage of labor (42.7), patient transport (41.2), securing patient privacy (38.1), followed by interpretation of EFM results (33.1) [11]. Since EFM-related tasks, such as comprehending the correlation between fetal heartbeat and pressure in the womb, require professional knowledge and understanding, nursing students should be provided with sufficient learning and training in EFM prior to their training in the delivery room [12].
\\
In maternal health nursing, the learning goals associated with EFM are “explanation of the purpose and method of EFM,” “understanding of EFM results,” “purpose of the non stress test and manipulation of the machine,” and “performance of nursing techniques upon fetal asphyxia.”
\newpage
\thisfancypage{\setlength{\fboxsep}{10pt}\fbox }{}
These goals underline the expectations for nursing students, including to understand the purpose, method, and principles of EFM, and be equipped with the skills to perform EFM and interpret its results [13].
However, previous studies show that only supplementary materials for understanding and performing EFM are utilized in self-directed learning [12], and education on high facility simulation is provided, both of which, are inadequate for developing overall nursing skills [14], thus highlighting the need for various educational methods for nursing students’ education and training. In today’s society, where high-level knowledge and clinical judgment skills are required and evidence for clinical application is fast-changing, the importance of educational programs utilizing AI, that allow safe and efficient learning for nursing college students has been emphasized [1]. Therefore, applications of nursing education utilizing AI are needed. To date, studies regarding chatbots in the medical field have focused on its application in the anatomy class for medical students [15] and chatbot programs for managing mental health, learning achievement, and well-being of college students [16]. In particular, in a study targeting 4th grade medical students in Hong Kong, clinical history was obtained by talking with a virtual patient through a chatbot mobile app without time or geographical restrictions. Based on the results of this study, it is suggested that chatbot programs can be an alternative to the existing clinical practice methods [17]. However, few studies have assessed its effect in nursing education. In other educational fields, using chatbot has shown improvements in students’ knowledge, academic motivation, and learning satisfaction [18]. Therefore, developing chatbot educational programs and evaluating their effects in the field of nursing education are needed. In this study, we aimed to develop and evaluate the effect of an AI chatbot educational program for improving nursing college students’ EFM nursing skills.



\newpage
\thisfancypage{\setlength{\fboxsep}{10pt}\fbox }{}
\section{Research hypotheses}

1)	There will be differences in the EFM knowledge between the experimental group, which participated in the AI chatbot educational program, and the control group.

2)	There will be differences in the clinical reasoning competency for EFM between the experimental group and the control group.

3)	There will be differences in the confidence in assessing fetal health between the experimental group and the control group.

4)	There will be differences in the interest in education between the experimental group and the control group.

5) There will be differences in the self-directed learning between the experimental group and the control group.

6)	The experimental group will have higher feedback satisfaction than the control group


\newpage
\thisfancypage{\setlength{\fboxsep}{10pt}\fbox }{}
\chapter{Literature Survey}

\section{Table of comparisons}
\begin{figure*}[h]
		\centerline{\psfig{figure=./dig1.png,width=5.9in,height=5.5in}}
		\label{atcres}
		\end{figure*}
		\vspace{0.2in}
\newpage
\thisfancypage{\setlength{\fboxsep}{10pt}\fbox }{}
\textbf{2.1	Summary of all papers}

     \textbf{Paper 1 (IEEE 2021):} Titled “Qualitative exploration of digital chatbot use in medical education: A pilot study” The study aims to assess the feasibility of implementing digital chatbots in medical education. This involves exploring whether digital chatbots can be effectively integrated into the existing educational framework.

     \textbf{Paper 2 (IEEE 2022):} The paper titled " Analysis of the effect of an artificial intelligence chatbot educational program on non-face-to- face classes: a quasi- experimental study “is to investigate and analyze the impact of an AI chatbot educational program on non-face-to-face (online or remote) classes

    \textbf{paper 3 (IEEE 2021):} Titled " Chatbot application in a 5th grade science course " The primary goal is to investigate how the use of a chatbot can enhance student engagement in a 5th-grade science course. It assesses whether chatbots can make learning more interactive, enjoyable, and motivating for young learners.





\newpage
\thisfancypage{\setlength{\fboxsep}{10pt}\fbox }{}
\chapter{Motivations and Objectives}
\section{3.1	Motivations:}
\hspace*{0.3in}The motivations behind conducting an analysis of the effect of an Artificial Intelligence (AI) chatbot educational program on non-face-to-face classes can be attributed to several key factors:
\\
\textbf{Technological Advancements:}

The rapid advancement of AI and natural language processing technologies has opened up new possibilities for enhancing education. Researchers and educators are motivated to explore how AI chatbots can be leveraged to improve non-face-to-face classes.
\\
\textbf{Pedagogical Innovation:}
\hspace*{0.3in}

The motivation to incorporate AI chatbots in education arises from the desire to innovate in pedagogy. Educators are interested in exploring new ways to engage students, provide personalized support, and enhance the learning experience in online or remote settings. \\
\textbf{Scalability and Accessibility:}
\hspace*{0.3in}AI chatbots offer the potential to provide scalable support to a large number of students. They can be available 24/7, making education more accessible and flexible for learners with varying schedules and needs. 
\textbf{Addressing Student Challenges:}

Many students in non-face-to-face classes face challenges related to self-regulated learning, time management, and access to resources. AI chatbots can be motivated by the goal of addressing these challenges and helping students succeed.
\newpage
\thisfancypage{\setlength{\fboxsep}{10pt}\fbox }{}
\textbf{Data-Driven Insights:}

Educators and institutions are motivated to collect and analyze data generated by chatbot interactions to gain insights into student behavior and performance. Data-driven decision-making can lead to improvements in online course design and teaching strategies.

\textbf{Improved Engagement:}

One of the key motivations is to enhance student engagement. AI chatbots can offer interactive elements, answer questions, provide instant feedback, and initiate discussions, potentially increasing students' motivation to participate actively in their education.

\textbf{Personalization:}

Motivations include the desire to provide a more personalized learning experience. AI chatbots can analyze student data and adapt to individual learning styles and preferences, which can improve learning outcomes.

\textbf{Cost-Effectiveness:}
Institutions may be motivated by the potential cost-
effectiveness of chatbots in education. While there are upfront development costs, chatbots can reduce the administrative workload and support services required for non-face-to-face classes.

\textbf{Research and Assessment:}
Researchers are motivated to contribute to the growing body of literature on the effectiveness of AI chatbots in education. Conducting an analysis provides valuable insights into their impact and effectiveness.

\textbf{Competitive Advantage:}
Institutions and educational platforms may be motivated by a desire to stay competitive in the digital education landscape. The use of AI chatbots can be a selling point for attracting students.

\textbf{Accessibility and Inclusivity:}
Motivations may stem from the goal of making education more inclusive. Chatbots can be designed with accessibility features that benefit students with disabilities.

\textbf{Student Support:}
The motivation to provide continuous support to students is significant. Chatbots offer an avenue for students to seek assistance and clarification on course content at any time. Educational Technology

\textbf{Advancement:}
 The broader motivation is to advance the field of educational technology. Experimenting with AI chatbots in non-face-to-face classes contributes to ongoing research and development in this field.
 
\newpage
\thisfancypage{\setlength{\fboxsep}{10pt}\fbox }{}


\newpage
\thisfancypage{\setlength{\fboxsep}{10pt}\fbox }{}

\textbf{Proposed Approach}

\begin{figure}[htbp]
\captionsetup{font=scriptsize}
\centering {\fbox{\includegraphics[width=15cm, height=5.4in]{dig2.jpg}}}
\caption{Proposed Approach.}
\label{fig}
\end{figure}

\textbf{3.2	Objectives}  

   The objectives of conducting an analysis of the effect of an Artificial Intelligence (AI) chatbot educational program on non-face-to-face classes are multifaceted and typically include:

 \textbf{Assess Learning Outcomes:}
 
   To evaluate whether the use of AI chatbots in non-face-to-face classes leads to improved student learning outcomes, including academic performance, knowledge retention, and skill development.

\textbf{Enhance Student Engagement:}

   To measure the impact of chatbots on student engagement in non-face-to-face classes, assessing factors such as participation, interactivity, and motivation.

   \textbf{Evaluate Student Support:}

     To assess how effectively AI chatbots provide support to students, answering questions, offering guidance, and addressing concerns related to course content and assignments.

      \textbf{Analyze Student Satisfaction:}

       To gauge student satisfaction and perceptions regarding the chatbot program's usability, helpfulness, and overall experience in non-face-to-face classes.

\newpage
\thisfancypage{\setlength{\fboxsep}{10pt}\fbox}{}
       \textbf{Understand Chatbot Use Patterns:}

        To analyze how students interact with the chatbot, examining usage patterns, common inquiries, and frequency of engagement.

        \textbf{Personalization and Adaptation:}

         To investigate the extent to which chatbots can personalize the learning experience for individual students, adapting to their unique needs and preferences.

         \textbf{Reduce Instructor Workload:}

         To determine if the chatbot program effectively reduces the administrative workload of instructors, allowing them to focus on more complex teaching tasks.

         \textbf{Assess Data-Driven Decision-Making:}

          To explore how data collected from chatbot interactions can be used for data-driven decision-making, course improvement, and providing timely support to students.

          \textbf{Evaluate Accessibility and Inclusivity:}

           To examine whether chatbots improve accessibility for all students, including those with disabilities, by offering features such as text-to-speech or speech-to-text capabilities.

           \textbf{Contribute to Research and Literature:}

            To contribute to the existing body of research and literature on the use of chatbots in educational contexts, providing valuable insights and findings for the academic community.

            \textbf{Inform Decision-Making:}

             To provide insights and evidence-based recommendations for educational institutions, instructors, and policymakers to make informed decisions regarding the integration and optimization of AI chatbots in non- face-to-face classes.

             \textbf{Enhance Student Learning Experience:}

              To assess the overall impact of chatbots on the student learning experience in non-face-to-face classes, including whether chatbots make learning more engaging, interactive, and efficient.

              \textbf{Evaluate Cost-Effectiveness:}

               To determine whether the benefits of implementing chatbots, such as improved student outcomes and reduced administrative costs, justify the initial investment in chatbot technology.

               \newpage
               \thisfancypage{\setlength{\fboxsep}{10pt}\fbox}{}













\newpage
\thisfancypage{\setlength{\fboxsep}{10pt}\fbox }{}
\chapter{Details of Design/Technology/Analytical/Analytical and/or Experimental Work}
\section{Architecture Diagram:}
\begin{figure*}[h]
		\centerline{\psfig{figure=./dig3.jpg,width=5.9in,height=5.0in}}
		\label{atcres}
		\end{figure*}
		\vspace{0.2in}
\newpage
\thisfancypage{\setlength{\fboxsep}{10pt}}\fbox{}
\section{Results}
  	\begin{figure*}[h]
		\centerline{\psfig{figure=./dig4.jpg,width=4.9in,height=2.5in}}
		\label{atcres}
		\end{figure*}
		\vspace{0.2in}

\begin{itemize}
    \item \textbf {Advantages:}
\end{itemize}

 \textbf{Enhanced Student Engagement: }

 Chatbots can provide interactive and engaging learning experiences, encouraging students to actively participate in non-face-to-face classes.
 
 \textbf{24/7 Availability:}

  Chatbots are available round the clock, providing students with instant access to information and support, making learning more flexible and accessible.

  \textbf{Personalized Learning:}

   AI chatbots can tailor content and resources to individual student needs, fostering a personalized learning experience.

   \textbf{Immediate Support: }

    Chatbots can provide immediate responses to student queries, offering assistance with coursework, assignments, or clarification on course content

    \textbf{Reduction in Instructor Workload: }

     Chatbots can handle routine administrative tasks, allowing instructors to focus on more complex teaching activities and providing more one-on-one support to students.
\newpage
\thisfancypage{\setlength{\fboxsep}{10pt}\fbox}{}
     \textbf{Data-Driven Insights:}

      	Chatbot interactions generate valuable data that can be used to assess student performance and engagement, leading to data-informed instructional decisions.
    \textbf{Improved Accessibility:	}

     Chatbots can be designed to accommodate diverse learning needs, including accessibility features for students with disabilities.

     \textbf{Cost-Efficiency: }

      Chatbots can reduce administrative costs associated with student support services and streamline communication processes.

    \textbf{Enhanced Student Retention: }

     Improved engagement, support, and personalization can contribute to higher student retention rates in non-face-to-face classes.

     \textbf{Instant Feedback: }

     Chatbots can provide immediate feedback on assignments and assessments, helping students identify and address areas where they may be struggling.

     \textbf{Scalability: }

      Chatbots can efficiently scale to accommodate a large number of students, ensuring consistent support and resources across diverse class sizes

    \begin{itemize}
        \item \textbf{Disadvantages:}
    \end{itemize}
    
      \textbf{Lack of Human Interaction: }
      

     Chatbots, by nature, lack the personal touch and human interaction that some students may require for a deeper understanding of complex concepts or emotional support.

    \textbf{Misunderstandings and Miscommunication}
    

      Chatbots may not always accurately understand or address student queries, potentially leading to misunderstandings and frustration.

      \textbf{Over-Reliance on Automation: }
      

       Students may become overly reliant on chatbots, which could potentially discourage critical thinking and problem-solving skills.

    \textbf{}
Technical Issues: }


   Chatbots can encounter technical glitches or errors that disrupt the learning process and cause frustration among students.
\newpage
\thisfancypage{\setlength{\fboxsep}{10pt}\fbox }{}
   \textbf{Privacy Concerns: }
   

    Gathering data for AI chatbot interactions raises privacy concerns, as students' personal information and learning behaviors may be collected and analyzed.

    \textbf{Bias and Fairness:}
    

    AI chatbots may inadvertently introduce biases in responses or recommendations, which can be a concern in educational settings, especially when addressing sensitive topics.

    \textbf{Learning Curve:}
    

     Students and instructors may require time to adapt to chatbot technology, potentially causing a learning curve and resistance to its adoption.

     \textbf{Limited Complexity: }
     

      Chatbots may struggle to handle highly complex or nuanced questions, making them less suitable for advanced or specialized topics.

    \textbf{Maintenance and Upkeep:}
    

      Ongoing maintenance and updates to chatbot programs are necessary, which can require resources and expertise.

      \textbf{Cost of Implementation:}
      

       The initial cost of developing, implementing, and maintaining a chatbot program can be a barrier for some educational institutions.

       \textbf{Loss of Instructor Jobs:}
       

        There may be concerns about the potential displacement of human instructors, particularly if chatbots are perceived as a complete substitute for teacher-student interactions.

       \newpage
       \thisfancypage{\setlength{\fboxsep}{10pt}\fbox}{}
       \chapter{Conclusions and Future Work}
       \section{Applications}

       \textbf{Enhanced Learning Experience:}

        Chatbots can provide students with instant access to course materials, resources, and answers to common questions, thereby improving the overall learning experience. They can offer personalized recommendations and reminders, helping students stay on track with their studies.

        \textbf{24/7 Availability:}

         AI chatbots are available around the clock, allowing students to seek help or information at any time, which can be especially beneficial for non-traditional students who may have varying schedules.


       \textbf{Immediate Feedback:}

     Chatbots can provide immediate feedback on assignments, quizzes, and assessments. This rapid feedback can help students identify and address areas where they may be struggling.

     \textbf{Reducing Instructor Workload:}

      Chatbots can answer routine or frequently asked questions, reducing the workload on instructors. This allows instructors to focus on more complex aspects of teaching.

      \textbf{Personalized Learning Paths:}

       AI chatbots can analyze student data and learning patterns to recommend personalized learning paths, helping students better understand and engage with the course content.

    \textbf{Student Engagement:}

     Chatbots can engage students with interactive activities and discussions. They can also send out reminders for upcoming assignments, exams, or class events.
     
     \newpage
\thisfancypage{\setlength{\fboxsep}{10pt}\fbox}{}      \textbf{Assistance for Students with Special Needs:}

       Chatbots can provide additional support to students with disabilities, such as text-to-speech and speech-to- text functionalities, making the course content more accessible.

        \textbf{Data-Driven Insights:}

         Chatbots can collect and analyze data on student interactions, which can be used to assess student performance, evaluate course effectiveness, and make data-driven improvements.

         \textbf{Challenges and Concerns:}

          While AI chatbots offer significant benefits, there are also concerns related to data privacy, technical issues, and the risk of over-reliance on automation, which could reduce the human element of education.

          \textbf{Enhanced Data Analytics:}

           Improved data analytics and machine learning will enable educators to gain deeper insights into student performance and learning behaviors, leading to more effective instructional design.

           \textbf{Integration of Chatbots with Human Instructors:}

            Hybrid models of education may evolve where chatbots complement human instructors, providing additional support and resources to enhance the learning experience.

            \textbf{Global Reach:}

             Chatbots have the potential to facilitate education for students around the world, transcending geographic and time zone barriers to make learning more global. 

              \textbf{Integration with Augmented and Virtual Reality (AR/VR):}

               Chatbots may become integral to AR/VR educational experiences, providing real-time assistance and information in immersive learning environments.

               \newpage
               \thisfancypage{\setlength{\fboxsep}{10pt}\fbox}{}
                 
                  
                  \section{Conclusion}

                  I studied this report, and I evaluated an AI chatbot educational program to enhance EFM nursing skills in nursing college students. Our findings hold significance as they present the potential of information and communications technology applications, such as chatbot, in the nursing education field. The chatbot program developed in our study had positive effects on the nursing college students’ interest in education and self-directed learning. Therefore, it can serve as an innovative and effective educational tool for improving students’ nursing skills, especially in non-face-to-face situations caused by the ongoing COVID- 19 pandemic. However, our study only evaluated the effect of the program in participants from only one college and selecting a non equivalent study design. As a post-test round was conducted on measurement variables in this study, we propose future studies with longitudinal design evaluating medium or long-term effects.

                  \newpage
                  \thisfancypage{\setlength{\fboxsep}{10pt}\fbox}{}

                  \chapter{References}
                  1. Buchanan C, Howitt ML, Wilson R,
Booth RG, Risling T, Bamford M.
Pre- dicted infuences of artifcial
intelligence on nursing education:
scoping review. JMIR Nurs.
2021;4(1):e23933.
https://doi.org/10.2196/23933.
2. Shorey S, Ang E, Yap J, Ng ED, Lau
ST, Chui CK. A virtual counseling
application using artifcial intelligence
for communication skills training in
nursing education: Development Study
[development study]. J Med Internet
Res. 2019;21(10):e14658.
https://doi.org/10.2196/14658.
3. Lee D, Park S. A developmental plan
for an English conversation learning
chatbot through the application of
elementary school English textbooks.
Korea Assoc Primary English Educ.
2019;25(4):79–100. https://doi.org/10.
25231/pee.2019.25.4.79.
4. Kaur A, Singh S, Chandan JS, Robbins
T, Patel V. Qualitative exploration of
digital chatbot use in medical education:
a pilot study. Digit Health.
2021;7:20552076211038150.
https://doi.org/10.1177/2055207621103
8151.
5. Stathakarou N, Nifakos S, Karlgren K,
Konstantinidis ST, Bamidis PD,
Pat- tichis CS, Davoody N. Students’
perceptions on chatbots’ potential and
design characteristics in healthcare
education. In: Mantas J, Hasman A,
Househ MS, Gallos P, Zoulias E,
editors. The importance of health
infor- matics in public health during a
pandemic Mantas. Amsterdam: IOS
Press; 2020. p. 209–12.
https://doi.org/10.3233/SHTI200531.
6. DeveciTopal A, DilekEren C,
KolburanGeçer A. Chatbot application
in a 5th grade science course. Educ Inf
Technol. 2021;26(5):6241–65. https://
doi.org/10.1007/s10639-021-10627-8.
7. Fryer LK, Thompson A, Nakao K,
Howarth M, Gallacher A. Supporting
self-efcacy beliefs and interest as
educational inputs and outcomes:
framing AI and human partnered task
experiences. Learn Individ Difer.
2020;80:101850.
https://doi.org/10.1016/j.lindif.2020.10
1850.
8. King TL, Parer JT. On electronic fetal
heart rate monitoring. J Obstet Gynecol
Neonatal Nurs. 2011;40(6):669–71.

\newpage
\thisfancypage{\setlength{\fboxsep}{10pt}\fbox}{}

https://doi.org/10.1111/j. 1552-
6909.2011.01291.x.
9. Knupp RJ, Andrews WW, Tita ATN.
The future of electronic fetal
monitor- ing. Best practice and research.
Clin Obstet Gynecol.2020;67:44–52.
https://doi.org/10.1016/j.bpobgyn.2020.
02.004.
10. Kim JI, Kang HS, Park SM, Ahn SH.
Current status of women’s health
nursing practicum and direction. Korean
J Women Health Nurs. 2014;20(2):173–
83.
https://doi.org/10.4069/kjwhn.2014.20.
2.173.
11. Kim YM, Chun N, Lee EH, Cho IS, Ahn
S, Kim JI, Hur MH, Lee SH, Lee HK,
Chung CW, Kang NM, Kim HW. 
                  
        
       

   
      

      





    


 

\end{document}
