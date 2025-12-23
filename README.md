\documentclass[10pt, a4paper]{article}

% Packages:
\usepackage[
    a4paper,
    top=1.25cm,
    bottom=1.25cm,
    left=1.5cm,
    right=1.5cm,
]{geometry}
\usepackage{titlesec}
\usepackage{tabularx}
\usepackage{array}
\usepackage[dvipsnames]{xcolor}
\usepackage{enumitem}
\usepackage{fontawesome5}
\usepackage{amsmath}

% --- FONT CONFIGURATION: SOURCE SANS PRO (Modern & Clear) ---
\usepackage[default]{sourcesanspro} 
\usepackage[T1]{fontenc}
\usepackage[utf8]{inputenc}
\usepackage{microtype} % Optimizes character spacing for clarity
% -----------------------------------------------------------

\usepackage[
    pdftitle={Kevin Zheng's CV},
    pdfauthor={Kevin Zheng},
    colorlinks=true,
    urlcolor=MidnightBlue,
    linkcolor=MidnightBlue
]{hyperref}

% Define Colors
\definecolor{darkblue}{RGB}{0, 0, 80}

% Formatting Sections
\titleformat{\section}
  {\vspace{-4pt}\raggedright\large\color{darkblue}\bfseries\uppercase}
  {}{0em}
  {}
  [\color{darkblue}\titlerule \vspace{-5pt}]

% Custom Commands
\newcommand{\resumeItem}[1]{
  \item\small{
    {#1 \vspace{-2pt}}
  }
}

\newcommand{\resumeSubheading}[4]{
  \vspace{-1pt}\item
    \begin{tabular*}{0.97\textwidth}[t]{l@{\extracolsep{\fill}}r}
      \textbf{#1} & \textit{\small #2} \\
      \textit{\small #3} & \textit{\small #4} \\
    \end{tabular*}\vspace{-5pt}
}

\newcommand{\resumeProjectHeading}[2]{
    \vspace{-1pt}\item
    \begin{tabular*}{0.97\textwidth}{l@{\extracolsep{\fill}}r}
      \textbf{#1} & \textit{\small #2} \\
    \end{tabular*}\vspace{-5pt}
}

\renewcommand\labelitemi{$\vcenter{\hbox{\tiny$\bullet$}}$}

\newenvironment{resumeItemList}{\begin{itemize}[leftmargin=0.15in, label={}]}{\end{itemize}}

% Remove page numbers
\pagestyle{empty}

% Improve Line Spacing for Readability
\linespread{1.05}

\begin{document}

%----------HEADER----------
\begin{center}
    {\Huge \color{darkblue} \textbf{Zhejian(Kevin) Zheng}} \\ \vspace{6pt}
    \small
    \faMapMarker* \ Sydney, NSW \ \ $\diamond$ \ \ 
    \faPhone \ \href{tel:+61491763561}{+61 491 763 561} \ \ $\diamond$ \ \ 
    \faEnvelope \ \href{mailto:zj.zheng1@gmail.com}{zj.zheng1@gmail.com} \ \ $\diamond$ \ \ 
    \faGithub \ \href{https://github.com/Zhejian-Zheng}{github.com/Zhejian-Zheng} 
    \faLink \ \href{https://zhejian-homepage.vercel.app/}{zhejian-homepage.vercel.app/}
\end{center}

%-----------EDUCATION-----------
\section{Education}
\begin{resumeItemList}
  \resumeSubheading
    {University of New South Wales (UNSW)}{Jan 2023 -- Feb 2026}
    {Bachelor of Computer Science}{Sydney, Australia}
  \begin{itemize}[leftmargin=0.15in, label={}, itemsep=1pt, topsep=2pt]
    \item \small \textbf{WAM:} 78 (Distinction)
    \item \small \textbf{Relevant Coursework:} Artificial Intelligence; Computer Networks; Advanced C++; Object-Oriented Programming; Database Systems; Software Construction; Algorithm Design and Analysis; Human Computer Interaction; Web Front-End Programming.
  \end{itemize}
\end{resumeItemList}


%-----------SKILLS-----------
\section{Technical Skills}
    \begin{itemize}[leftmargin=0.15in, label={}]
      \small{\item{
        \textbf{Languages}{: Python (\textit{proficient}), C (\textit{proficient}), Java (OOP, \textit{working knowledge}), JavaScript/TypeScript (\textit{working knowledge}), C++ (\textit{intermediate}), Rust (\textit{intermediate}), SQL} \\
        \textbf{Backend}{: Node.js, Express, FastAPI, Flask} \\
        \textbf{Frontend}{: React, Next.js, vanilla Javascript, Tailwind CSS, HTML5, CSS3} \\
        \textbf{Databases}{: PostgreSQL, MongoDB} \\
        \textbf{Tools}{: Git, Docker, Linux, AWS (S3), Vercel, Unreal Engine, figma}
      }}
    \end{itemize}


%-----------EXPERIENCE-----------
\section{Work Experience}
  \begin{resumeItemList}

    \resumeSubheading
      {Jobgen.ai $|$ \emph{ Python, Playwrigh, MongoD, AWS S3, RESTful API, Git}}{May 2025 -- Aug 2025}
      {Backend Developer Intern}{Remote / Sydney}
      \begin{itemize}[leftmargin=0.15in]
        \resumeItem{This project uses Python and Playwright to build a job information collection pipeline, extracting and structuring job data from publicly available web sources, and aggregating and improving collection efficiency and stability.}
        \resumeItem{Design and implement a RESTful backend API that supports real-time filtering, pagination, and response shaping on the frontend, improving the search experience and API usability.}
        \resumeItem{Optimize MongoDB indexes for core query scenarios to improve database access performance; and integrate AWS S3 for scalable storage and management of static resources/attachments.}
        \resumeItem{Improve code reliability through unit testing and ensure continuous delivery quality by using Git and CI/CD processes in team collaboration.}
      \end{itemize}

  \end{resumeItemList}

%-----------PROJECTS-----------
\section{Projects}
  \begin{resumeItemList}
  
    \resumeProjectHeading
      {\textbf{AirBrB} $|$ \emph{React, TypeScript, REST APIs, Jest}}{Nov 2025}
      \begin{itemize}[leftmargin=0.15in]
        \resumeItem{Developed a full-stack home booking platform featuring JWT authentication, listing management, and real-time booking engines.}
        \resumeItem{Implemented complex search algorithms supporting multi-condition filtering (location, date ranges, price) and rating-based sorting.}
        \resumeItem{Built a dedicated Host Dashboard to visualize revenue data using charting libraries and manage booking approvals.}
      \end{itemize}

    \resumeProjectHeading
      {\textbf{Legal Youth Prototype} $|$ \emph{React, TypeScript, Node.js, Tailwind CSS}}{Aug 2025}
      \begin{itemize}[leftmargin=0.15in]
        \resumeItem{Developed a full-stack educational platform designed to make legal resources accessible to youth audiences.}
        \resumeItem{Built an interactive "Ask AI" feature using React and Express to provide real-time answers to common legal questions.}
        \resumeItem{Designed a responsive, mobile-friendly UI using Tailwind CSS, adhering to accessibility (a11y) best practices.}
      \end{itemize}

    \resumeProjectHeading
      {\textbf{Balatro Game Engine} $|$ \emph{Rust, Systems Programming}}{Mar 2025}
      \begin{itemize}[leftmargin=0.15in]
        \resumeItem{Re-architected the scoring logic of a complex roguelike game using Rust, prioritizing memory safety and zero-cost abstractions.}
        \resumeItem{Utilized Rust's ownership and borrowing model to eliminate runtime errors and ensure thread-safe execution.}
      \end{itemize}

    \resumeProjectHeading
      {\textbf{BitTrickle} $|$ \emph{Python, Socket Programming, TCP/UDP}}{Oct 2024}
      \begin{itemize}[leftmargin=0.15in]
        \resumeItem{Constructed a Peer-to-Peer (P2P) file sharing system supporting concurrent file transfers via multi-threading.}
        \resumeItem{Implemented a central directory server to manage active peer listings, featuring automatic "heartbeat" cleanup.}
      \end{itemize}
       
  \end{resumeItemList}
\end{document}
