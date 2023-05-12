# CV-and-Resume
My professional journey.

%-------------------------
% Rezume, a latex resume template for developers
% Author : Nanu Panchamurthy
% Based off of: https://github.com/sb2nov/resume
% License : MIT

% Hope this resume template helps you land an awesome job. If you found this helpful, please consider starring the github repo here, .
%-------------------------



%------------PACKAGES----------------
\documentclass[a4paper,11pt]{article}

\usepackage{verbatim} % reimplements the "verbatim" and "verbatim*" environments

\usepackage{titlesec} % provides an interface to sectioning commands i.e. custom elements

\usepackage{color} % provides both foreground and background color management

\usepackage{enumitem} % provides control over enumerate, itemize and description

\usepackage{fancyhdr} % provides extensive facilities for constructing headers, footers and also controlling their use

\usepackage{tabularx} % defines an environment tabularx, extension of "tabular" with an extra designator x, paragraph like column whose width automatically expands to fill the width of the environment

\usepackage{latexsym} % provides mathematical symbols

\usepackage{marvosym} % provides martin vogel's symbol font which contains various symbols

\usepackage[empty]{fullpage} % sets margins to one inch and removes headers, footers etc..

\usepackage[hidelinks]{hyperref} % removes color and shadow of hyperlinks

\usepackage[normalem]{ulem} % provides "\ul" (uline) command which will break at line breaks

\usepackage[english]{babel} % provides culturally determined typographical rules for wide range of languages
%-----------------------------------------

\input glyphtounicode % converts glyph names to unicode
\pdfgentounicode=1 % ensures pdfs generated are ats readable

%----------FONT OPTIONS-------------------
\usepackage[default]{sourcesanspro} % uses the font source sans pro
\urlstyle{same} % changes url font from default urlfont to font being used by the document
%-----------------------------------------


%----------MARGIN OPTIONS-----------------
\pagestyle{fancy} % set page style to one configured by fancyhdr
\fancyhf{} % clear all header and footer fields

\renewcommand{\headrulewidth}{0in} % sets thickness of linerule under header to zero
\renewcommand{\footrulewidth}{0in} % sets thickness of linerule over footer to zero

\setlength{\tabcolsep}{0in} % sets thickness of column separator in tables to zero

% origin of the document is one inch from the top and from and the left
% oddsidemargin and evensidemargin both refer to the left margin
% right margin is indirectly set using oddsidemargin
\addtolength{\oddsidemargin}{-0.5in}
\addtolength{\topmargin}{-0.5in}

\addtolength{\textwidth}{1.0in} % sets width of text area in the page to one inch
\addtolength{\textheight}{1.0in} % sets height of text area in the page to one inch

\raggedbottom{} % makes all pages the height of current page, no extra vertical space added
\raggedright{} % makes all pages the width of current page, no extra horizontal space added
%------------------------------------------


%--------SECTIONING COMMANDS---------
% \titleformat{<command>}
%   [<shape>]{<format>}{<label>}{<sep>}
%     {<before-code>}[<after-code>]

% command is the sectioning command to be redefined
% shape is the style of the font; scshape stands for small caps style
% format is the format to be applied to whole title- label and text; absent here
% label defines the label
% sep is the horizontal separation between label and title body
% before-code is the code to be executed before
% after-code is the code to be executed after

\titleformat{\section}
  {\scshape\large}{}
    {0em}{\color{blue}}[\color{black}\titlerule\vspace{0pt}]
%-------------------------------------


%--------REDEFINITIONS----------------
% redefines the style of the bullet point
\renewcommand\labelitemii{$\vcenter{\hbox{\tiny$\bullet$}}$}

% redefines the underline depth to 2pt
\renewcommand{\ULdepth}{2pt}
%-------------------------------------


%--------CUSTOM COMMANDS--------------
%\vspace{} defines a vertical space of given size, modifying this in custom commands can help stretch or shrink resume to remove or add content

% resumeItem renders a bullet point
\newcommand{\resumeItem}[1]{
  \item\small{#1}
}

% commands to start and end itemization of resumeItem, rightmargin set to 0.11in to avoid the overflow of resumetItem beyond whatever resumeItemHeading is being used
\newcommand{\resumeItemListStart}{\begin{itemize}[rightmargin=0.11in]}
\newcommand{\resumeItemListEnd}{\end{itemize}}

% resumeSectionType renders a bolded type to be used under a section, used as skill type here, middle element is used to keep ":"s in the same vertical line
\newcommand{\resumeSectionType}[3]{
  \item\begin{tabular*}{0.96\textwidth}[t]{
    p{0.15\linewidth}p{0.02\linewidth}p{0.81\linewidth}
  }
    \textbf{#1} & #2 & #3
  \end{tabular*}\vspace{-2pt}
}

% resumeTrioHeading renders three elements in three columns with second element being italicized and first element bolded, can be used for projects with three elements
\newcommand{\resumeTrioHeading}[3]{
  \item\small{
    \begin{tabular*}{0.96\textwidth}[t]{
      l@{\extracolsep{\fill}}c@{\extracolsep{\fill}}r
    }
      \textbf{#1} & \textit{#2} & #3
    \end{tabular*}
  }
}

% resumeQuadHeading renders four elements in a two columns with the second row being italicized and first element of first row bolded, can be used for experience and projects with four elements
\newcommand{\resumeQuadHeading}[4]{
  \item
  \begin{tabular*}{0.96\textwidth}[t]{l@{\extracolsep{\fill}}r}
    \textbf{#1} & #2 \\
    \textit{\small#3} & \textit{\small #4} \\
  \end{tabular*}
}

% resumeQuadHeadingChild renders the second row of resumeQuadHeading, can be used for experience if different roles in the same company need to added
\newcommand{\resumeQuadHeadingChild}[2]{
  \item
  \begin{tabular*}{0.96\textwidth}[t]{l@{\extracolsep{\fill}}r}
    \textbf{\small#1} & {\small#2} \\
  \end{tabular*}
}

% commands to start and end itemization of resumeQuadHeading, lefmargin for left indent of 0.15in for resumeItems
\newcommand{\resumeHeadingListStart}{
  \begin{itemize}[leftmargin=0.15in, label={}]
}
\newcommand{\resumeHeadingListEnd}{\end{itemize}}
%-------------------------------------------


%__________________RESUME____________________
% You can rearrange sections in any order you may prefer
\begin{document}

%-----------CONTACT DETAILS------------------
% Make sure all the details are correct, you can add more links in the first row of second column if needed

\begin{tabular*}{\textwidth}{l@{\extracolsep{\fill}}r}
  \textbf{\Huge Satvikkumar Patel\vspace{2pt}} & % row = 1, col = 1
  Location: Valsad, Gujarat, India \\ % row = 1, col = 2
\href{https://www.linkedin.com/in/satvik-patel-433655164/}{\uline{Linkedin}} $|$ % row = 2, col = 2
\href{https://github.com/Satvik3799}{\uline{GitHUB}} $|$ % row = 2, col = 2
 
  Email: \href{emmm}{\uline{emmm}} $|$ % row = 2, col = 2
  Mobile: +91 12345 67890\\ % row = 2, col = 2
\end{tabular*}
%--------------------------------------------


%-----------SUMMARY--------------------------
% Keep this short, simple and straigth to point

\section{Embedded Hardware Design Developer}
\small{
I am an experienced Embedded Hardware Design developer with over \textbf{1 years of experience} where my responsibilities included \textbf{Selecting components for the concept Hardware, Designing logic of the concept hardware, Creating schematics and designing PCBs, Discussions with PCB manufacturers for the manufacturability of the PCB, Testing and Debugging the assembled hardware.} I have \textbf{ranked 3751 out of 45833} students in a national level examination, GATE 2023, and have been offered to pursue M.tech in Digital Techniques and instrumentation specialization at \textbf{IIT BHU}, one of the top 10 university in India, this year. Before I start my studies I was hoping to get a push by interning at your firm.}
}
%--------------------------------------------


%--------------SKILLS------------------------
% Add or remove resumeSectionTypes according to your needs

\section{Technical Skills}
  \resumeHeadingListStart{}
    \resumeSectionType{Languages}{:}{Python (\textit{Novice}), Verilog (\textit{Novice})}
    \resumeSectionType{Microcontrollers}{:}{Dialog Semicondutor - DA14531, Espressif ESP32 series - ESP32-S3, ESP32-S2, EPS32-D0WD, ESP32-U4WDH}
    \resumeSectionType{Softwares}{:}{Altium designer (\textit{Proficient}), Xilinx Vivado (\textit{Novice}), Orcad spice (\textit{Novice})}
    \resumeSectionType{General Tools}{:}{GitHUB, Sublime text editor, Arduino IDE, MS Office tools, Notion}
  \resumeHeadingListEnd{}
%--------------------------------------------


%-----------EXPERIENCE-----------------------
% Distill all your talking points to small bullet points which follow the pattern "challenge-action-result" for maximum efficiency. Try to quantify (use numbers) your points whenver possible, highlist words of importance

\section{Experience}
\resumeHeadingListStart{}
  \resumeQuadHeading{Embedded Hardware Design Developer}{Mar 2022 -- Mar 2023}
  {VEGG (an iOT company)}{On site -- Surat, Gujarat, India}
    \resumeItemListStart{}
      \resumeItem{ Designed and developed multiple hardware according to concept from selecting components and logic brainstorm to board bring-up using different platforms such as \textbf{Altium Designer, Arduino IDE, ESP IDE}} 
      \resumeItem{Worked with assembly team, PCB manufacturers and clients to realise a product. }
      \resumeItem{some of the products I have worked on are listed below:
      }
    \resumeItemListEnd{}

%   \resumeQuadHeading{Backend Developer}{Aug 2021 -- Nov 2022}
%   {Anycompany}{Anycity, Anystate, Anycountry}
%     \resumeItemListStart{}
%       \resumeItem{Worked with \textbf{MVC frameworks} to develop robust and scalable backends}
%       \resumeItem{Troubleshot and \textbf{fixed bugs} and issues in the backend to ensure \textbf{smooth operation} of the applications}
%     \resumeItemListEnd{}

%   \resumeQuadHeadingChild{Backend Developer Intern}{Jan 2021 -- Aug 2021}
%     \resumeItemListStart{}
%       \resumeItem{Assisted senior web developers in the design and development of websites using \textbf{HTML, CSS, and JavaScript}}
%     \resumeItemListEnd{}
% \resumeHeadingListEnd{}
%---------------------------------------------


%-----------EDUCATION-------------------------
% Mention your CGPA, if its good, in the first row of second column

\section{Education}
  \resumeHeadingListStart{}
    \resumeQuadHeading{Institute of infrastructure Technology Research And Management (IITRAM)} {7.24/10}
    {Bachelor of Engineering in Electrical Engineering}{2017 -- 2021}
    
  \resumeHeadingListEnd{}
  % \resumeHeadingListStart{}
  %   \resumeQuadHeading{Government Polytechnic Ahmedabad} {Ahmedabad, Gujarat, India}
  %   {Diploma in Electronics and Communication}{2016 -- Dec 2019}
  % \resumeHeadingListEnd{}
%---------------------------------------------


\section{Self learning Courses}
  \resumeHeadingListStart{}
  
    \resumeQuadHeading{Online courses} 
    \resumeItem{}
    \resumeItem{Introduction to Programming with MATLAB by Vanderbilt University - Coursera.}
    \resumeItem{Build a Modern Computer from First Principles: From Nand to Tetris (Project-Centered Course) by Hebrew University of Jerusalem - Coursera.}
    
    \resumeItem{Programming for Everybody (Getting Started with Python) by University of Michigan - Coursera.}
    
    \resumeItem{VSD - Physical Design Flow - Udemy.}
    
   
    \resumeQuadHeading{Reference Books}
    \resumeItem{}
    \resumeItem{Digital Design and Computer Architecture (ARM Edition) by Sarah L. Harris and David Money Harris}
    \resumeItem{Electronic Devices and Circuit theory by Robert L. Boylstad and Louis Nashelsky}
    \resumeItem{Digital Design with an introduction to Verilog HDL by Morris M. mano and Michael D. Ciletti}
    \resumeItem{OPAmp for everyone by Ron Mancini (Texas Instruments)}
 
  \resumeHeadingListEnd{}



%-----------PROJECTS--------------------------
% Use resumeQuadHeading if four elements are feasible (ex: demo video link), else use resumeTrioHeading. Keep the bullet points simple and concise and try to cover wide variety of skills you have used to build these projects

\section{Projects}
  \resumeHeadingListStart{}
    \resumeTrioHeading{\href{https://project1.com}{\uline{Project 1}}}{React.js, Redux, PHP, MySQL Git}{\href{https://proect1.com/source-code/}{\uline{Source Code}}}
      \resumeItemListStart{}
        \resumeItem{Designed and developed a clean and modern website using \textbf{HTML, CSS, and JavaScript}}
        \resumeItem{Optimized website for \textbf{speed and user experience}}
        \resumeItem{Utilized \textbf{responsive design} to ensure compatibility across all devices}
        \resumeItem{Deployed on GitHub pages via GitHub Actions}
      \resumeItemListEnd{}

      \resumeTrioHeading{Project 2}{Node.js, Express, JavaScript, Git}{\href{https:project2.com/source-code}{\uline{Source Code}}}
      \resumeItemListStart{}
        \resumeItem{A \textbf{CRUD application} exposed using a RESTful API made with Node.js}
        \resumeItem{Exposed POST, GET, PATCH and DELETE HTTP methods using \textbf{Express}}
      \resumeItemListEnd{}
  \resumeHeadingListEnd{}
%--------------------------------------------


%----------------OTHERS----------------------
% You can add your acheivements, accolades, certifications etc. here.

%\section{Certifications} % \resumeItemListStart{}
%    \resumeItem{\href{https://dummy-certification.com}{\uline{Certified Web Developer by the W3C}}}
 %   \resumeItem{\href{https://dummy-certification.com}{\uline{Microsoft Certified: Azure Developer Associate}}}
%    \resumeItem{\href{https://dummy-certification.com}{\uline{AWS Certified Developer - Associate}}}
 % \resumeItemListEnd{}
%--------------------------------------------

\end{document}