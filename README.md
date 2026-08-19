<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Amal Ben Khelifa | Software Engineer & IT Business Analyst</title>

    <meta name="description"
          content="Amal Ben Khelifa - Software Engineer and IT Business Analyst with experience in Java, Angular, application support and IT projects.">

    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap"
          rel="stylesheet">

    <style>

        /* =========================
           GENERAL
        ========================= */

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: "Inter", sans-serif;
            background: #f8fafc;
            color: #1e293b;
            line-height: 1.7;
        }

        a {
            text-decoration: none;
            color: inherit;
        }

        .container {
            width: 90%;
            max-width: 1150px;
            margin: auto;
        }

        section {
            padding: 90px 0;
        }

        .section-title {
            text-align: center;
            margin-bottom: 55px;
        }

        .section-title span {
            font-size: 14px;
            font-weight: 700;
            text-transform: uppercase;
            letter-spacing: 2px;
            color: #6366f1;
        }

        .section-title h2 {
            font-size: 36px;
            margin-top: 10px;
            color: #0f172a;
        }

        .section-title p {
            max-width: 650px;
            margin: 15px auto 0;
            color: #64748b;
        }


        /* =========================
           NAVBAR
        ========================= */

        header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background: rgba(255,255,255,0.95);
            backdrop-filter: blur(10px);
            border-bottom: 1px solid #e2e8f0;
            z-index: 1000;
        }

        nav {
            height: 75px;
            display: flex;
            align-items: center;
            justify-content: space-between;
        }

        .logo {
            font-size: 22px;
            font-weight: 800;
            color: #0f172a;
        }

        .logo span {
            color: #6366f1;
        }

        .nav-links {
            display: flex;
            gap: 30px;
            list-style: none;
        }

        .nav-links a {
            font-size: 14px;
            font-weight: 600;
            color: #475569;
            transition: 0.3s;
        }

        .nav-links a:hover {
            color: #6366f1;
        }

        .menu-btn {
            display: none;
            font-size: 25px;
            cursor: pointer;
        }


        /* =========================
           HERO
        ========================= */

        #home {
            min-height: 100vh;
            display: flex;
            align-items: center;
            padding-top: 100px;
            background:
                radial-gradient(circle at top right, #e0e7ff 0%, transparent 35%),
                #f8fafc;
        }

        .hero {
            display: grid;
            grid-template-columns: 1.2fr 0.8fr;
            align-items: center;
            gap: 60px;
        }

        .hero-content h1 {
            font-size: 54px;
            line-height: 1.15;
            color: #0f172a;
            margin-bottom: 20px;
        }

        .hero-content h1 span {
            color: #6366f1;
        }

        .hero-subtitle {
            font-size: 21px;
            font-weight: 600;
            color: #475569;
            margin-bottom: 20px;
        }

        .hero-description {
            max-width: 650px;
            color: #64748b;
            font-size: 17px;
            margin-bottom: 30px;
        }

        .hero-buttons {
            display: flex;
            gap: 15px;
            flex-wrap: wrap;
        }

        .btn {
            display: inline-block;
            padding: 13px 23px;
            border-radius: 8px;
            font-weight: 600;
            font-size: 14px;
            transition: 0.3s;
        }

        .btn-primary {
            background: #6366f1;
            color: white;
        }

        .btn-primary:hover {
            background: #4f46e5;
            transform: translateY(-2px);
        }

        .btn-secondary {
            border: 1px solid #cbd5e1;
            color: #334155;
            background: white;
        }

        .btn-secondary:hover {
            border-color: #6366f1;
            color: #6366f1;
        }

        .hero-card {
            background: white;
            border-radius: 20px;
            padding: 40px;
            box-shadow: 0 20px 50px rgba(15,23,42,0.08);
            border: 1px solid #e2e8f0;
            text-align: center;
        }

        .hero-avatar {
            width: 150px;
            height: 150px;
            margin: auto;
            border-radius: 50%;
            background: #e0e7ff;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 50px;
            font-weight: 800;
            color: #6366f1;
        }

        .hero-card h3 {
            margin-top: 25px;
            font-size: 22px;
            color: #0f172a;
        }

        .hero-card p {
            color: #64748b;
            margin-top: 5px;
        }


        /* =========================
           ABOUT
        ========================= */

        .about {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 60px;
            align-items: center;
        }

        .about-text h3 {
            font-size: 28px;
            color: #0f172a;
            margin-bottom: 20px;
        }

        .about-text p {
            color: #64748b;
            margin-bottom: 15px;
        }

        .about-highlights {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 15px;
        }

        .highlight {
            background: white;
            padding: 25px;
            border-radius: 12px;
            border: 1px solid #e2e8f0;
        }

        .highlight strong {
            display: block;
            font-size: 24px;
            color: #6366f1;
        }

        .highlight span {
            color: #64748b;
            font-size: 14px;
        }


        /* =========================
           EXPERTISE
        ========================= */

        .expertise-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 25px;
        }

        .expertise-card {
            background: white;
            padding: 30px;
            border-radius: 15px;
            border: 1px solid #e2e8f0;
            transition: 0.3s;
        }

        .expertise-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 30px rgba(15,23,42,0.08);
        }

        .expertise-icon {
            width: 50px;
            height: 50px;
            border-radius: 10px;
            background: #eef2ff;
            color: #6366f1;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 22px;
            margin-bottom: 20px;
        }

        .expertise-card h3 {
            margin-bottom: 12px;
            color: #0f172a;
        }

        .expertise-card p {
            color: #64748b;
            font-size: 14px;
        }


        /* =========================
           EXPERIENCE
        ========================= */

        .timeline {
            position: relative;
            max-width: 900px;
            margin: auto;
        }

        .timeline::before {
            content: "";
            position: absolute;
            left: 10px;
            top: 0;
            bottom: 0;
            width: 2px;
            background: #e2e8f0;
        }

        .timeline-item {
            position: relative;
            padding-left: 45px;
            margin-bottom: 45px;
        }

        .timeline-dot {
            position: absolute;
            left: 2px;
            top: 5px;
            width: 18px;
            height: 18px;
            border-radius: 50%;
            background: #6366f1;
            border: 4px solid #eef2ff;
        }

        .timeline-item h3 {
            color: #0f172a;
            font-size: 22px;
        }

        .timeline-item .company {
            color: #6366f1;
            font-weight: 600;
            margin: 5px 0;
        }

        .timeline-item .date {
            font-size: 13px;
            color: #94a3b8;
            margin-bottom: 15px;
        }

        .timeline-item p {
            color: #64748b;
            margin-bottom: 12px;
        }

        .timeline-item ul {
            padding-left: 20px;
            color: #64748b;
        }

        .timeline-item li {
            margin-bottom: 7px;
        }


        /* =========================
           PROJECTS
        ========================= */

        .projects-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 30px;
        }

        .project-card {
            background: white;
            border-radius: 15px;
            overflow: hidden;
            border: 1px solid #e2e8f0;
            transition: 0.3s;
        }

        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 35px rgba(15,23,42,0.08);
        }

        .project-header {
            background: #eef2ff;
            padding: 30px;
        }

        .project-header h3 {
            color: #0f172a;
            font-size: 23px;
        }

        .project-body {
            padding: 30px;
        }

        .project-body p {
            color: #64748b;
            margin-bottom: 20px;
        }

        .tags {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
        }

        .tag {
            background: #f1f5f9;
            color: #475569;
            padding: 6px 10px;
            border-radius: 6px;
            font-size: 12px;
            font-weight: 600;
        }


        /* =========================
           SKILLS
        ========================= */

        .skills-container {
            max-width: 950px;
            margin: auto;
        }

        .skill-group {
            margin-bottom: 30px;
        }

        .skill-group h3 {
            font-size: 18px;
            margin-bottom: 15px;
            color: #0f172a;
        }

        .skill-list {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }

        .skill {
            background: white;
            border: 1px solid #e2e8f0;
            padding: 10px 15px;
            border-radius: 8px;
            color: #475569;
            font-size: 14px;
            font-weight: 500;
        }


        /* =========================
           BUSINESS ANALYSIS
        ========================= */

        .analysis-box {
            max-width: 900px;
            margin: auto;
            background: white;
            border: 1px solid #e2e8f0;
            border-radius: 15px;
            padding: 45px;
        }

        .analysis-box p {
            color: #64748b;
            margin-bottom: 25px;
        }

        .analysis-list {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 15px;
        }

        .analysis-list div {
            padding: 15px;
            background: #f8fafc;
            border-radius: 8px;
            color: #475569;
            font-size: 14px;
        }


        /* =========================
           EDUCATION
        ========================= */

        .education-card {
            max-width: 800px;
            margin: auto;
            background: white;
            padding: 35px;
            border-radius: 15px;
            border: 1px solid #e2e8f0;
        }

        .education-card h3 {
            color: #0f172a;
            font-size: 22px;
        }

        .education-card .school {
            color: #6366f1;
            font-weight: 600;
            margin: 5px 0;
        }

        .education-card p {
            color: #64748b;
        }


        /* =========================
           CAREER GOALS
        ========================= */

        .career {
            background: #0f172a;
            color: white;
        }

        .career .section-title h2 {
            color: white;
        }

        .career .section-title p {
            color: #94a3b8;
        }

        .career-content {
            max-width: 800px;
            margin: auto;
            text-align: center;
        }

        .career-content p {
            color: #cbd5e1;
            font-size: 17px;
            margin-bottom: 30px;
        }

        .career-tags {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 10px;
        }

        .career-tag {
            padding: 10px 16px;
            border: 1px solid #475569;
            border-radius: 8px;
            color: #e2e8f0;
            font-size: 14px;
        }


        /* =========================
           CONTACT
        ========================= */

        .contact-container {
            max-width: 700px;
            margin: auto;
            text-align: center;
        }

        .contact-container p {
            color: #64748b;
            margin-bottom: 30px;
        }

        .contact-buttons {
            display: flex;
            justify-content: center;
            gap: 15px;
            flex-wrap: wrap;
        }


        /* =========================
           FOOTER
        ========================= */

        footer {
            background: #020617;
            color: #94a3b8;
            text-align: center;
            padding: 25px;
            font-size: 13px;
        }


        /* =========================
           RESPONSIVE
        ========================= */

        @media (max-width: 900px) {

            .hero {
                grid-template-columns: 1fr;
                text-align: center;
            }

            .hero-description {
                margin-left: auto;
                margin-right: auto;
            }

            .hero-buttons {
                justify-content: center;
            }

            .about {
                grid-template-columns: 1fr;
            }

            .expertise-grid {
                grid-template-columns: 1fr 1fr;
            }

        }


        @media (max-width: 700px) {

            section {
                padding: 70px 0;
            }

            .section-title h2 {
                font-size: 30px;
            }

            .hero-content h1 {
                font-size: 40px;
            }

            .nav-links {
                display: none;
                position: absolute;
                top: 75px;
                left: 0;
                width: 100%;
                background: white;
                flex-direction: column;
                padding: 25px;
                gap: 20px;
                border-bottom: 1px solid #e2e8f0;
            }

            .nav-links.active {
                display: flex;
            }

            .menu-btn {
                display: block;
            }

            .expertise-grid,
            .projects-grid {
                grid-template-columns: 1fr;
            }

            .analysis-list {
                grid-template-columns: 1fr;
            }

            .hero-card {
                padding: 30px;
            }

        }

    </style>
</head>


<body>


<!-- =========================
     NAVIGATION
========================= -->

<header>

    <div class="container">

        <nav>

            <a href="#home" class="logo">
                Amal<span>.</span>
            </a>

            <ul class="nav-links" id="navLinks">

                <li><a href="#home">Home</a></li>

                <li><a href="#about">About</a></li>

                <li><a href="#expertise">Expertise</a></li>

                <li><a href="#experience">Experience</a></li>

                <li><a href="#projects">Projects</a></li>

                <li><a href="#skills">Skills</a></li>

                <li><a href="#contact">Contact</a></li>

            </ul>

            <div class="menu-btn" id="menuBtn">
                ☰
            </div>

        </nav>

    </div>

</header>



<!-- =========================
     HOME
========================= -->

<section id="home">

    <div class="container">

        <div class="hero">

            <div class="hero-content">

                <h1>
                    Hi, I'm <span>Amal</span>
                </h1>

                <div class="hero-subtitle">
                    Software Engineer | IT Business Analyst
                </div>

                <p class="hero-description">

                    I bridge business needs and technical solutions through
                    software engineering, business analysis and IT project
                    collaboration.

                </p>

                <div class="hero-buttons">

                    <a href="#experience" class="btn btn-primary">
                        View My Experience
                    </a>

                    <a href="#contact" class="btn btn-secondary">
                        Contact Me
                    </a>

                </div>

            </div>


            <div class="hero-card">

                <div class="hero-avatar">
                    AB
                </div>

                <h3>
                    Amal Ben Khelifa
                </h3>

                <p>
                    Software Engineer
                </p>

                <p>
                    IT Business Analyst
                </p>

            </div>

        </div>

    </div>

</section>



<!-- =========================
     ABOUT
========================= -->

<section id="about">

    <div class="container">

        <div class="section-title">

            <span>About Me</span>

            <h2>Who I Am</h2>

        </div>


        <div class="about">

            <div class="about-text">

                <h3>
                    Technology with a business perspective.
                </h3>

                <p>

                    I am a Software Engineer with experience in Java and
                    Angular development, IT projects and application support.

                </p>

                <p>

                    During my experience at Sofrecom, part of the Orange Group,
                    I worked on enterprise applications and digital solutions
                    in an Agile environment, collaborating with teams in
                    Tunisia and France.

                </p>

                <p>

                    My technical background allows me to understand complex
                    IT environments, while my interest in business analysis
                    helps me focus on understanding needs and finding
                    practical solutions.

                </p>

            </div>


            <div class="about-highlights">

                <div class="highlight">
                    <strong>Java</strong>
                    <span>Backend Development</span>
                </div>

                <div class="highlight">
                    <strong>Angular</strong>
                    <span>Frontend Development</span>
                </div>

                <div class="highlight">
                    <strong>IT</strong>
                    <span>Business Analysis</span>
                </div>

                <div class="highlight">
                    <strong>Agile</strong>
                    <span>Collaborative Projects</span>
                </div>

            </div>

        </div>

    </div>

</section>



<!-- =========================
     EXPERTISE
========================= -->

<section id="expertise">

    <div class="container">

        <div class="section-title">

            <span>Expertise</span>

            <h2>What I Do</h2>

            <p>
                Combining technical expertise, analytical thinking
                and collaboration.
            </p>

        </div>


        <div class="expertise-grid">


            <div class="expertise-card">

                <div class="expertise-icon">
                    ♢
                </div>

                <h3>
                    Business Analysis
                </h3>

                <p>

                    Understanding business needs, analyzing requirements,
                    identifying functional solutions and bridging the gap
                    between business and technical teams.

                </p>

            </div>


            <div class="expertise-card">

                <div class="expertise-icon">
                    ⚙
                </div>

                <h3>
                    IT Projects
                </h3>

                <p>

                    Project coordination, requirements analysis,
                    application support, incident analysis and
                    collaboration with stakeholders.

                </p>

            </div>


            <div class="expertise-card">

                <div class="expertise-icon">
                    &lt;/&gt;
                </div>

                <h3>
                    Software Engineering
                </h3>

                <p>

                    Developing and maintaining enterprise applications
                    using Java, Spring Boot, Angular, REST APIs
                    and modern development practices.

                </p>

            </div>

        </div>

    </div>

</section>



<!-- =========================
     EXPERIENCE
========================= -->

<section id="experience">

    <div class="container">

        <div class="section-title">

            <span>Experience</span>

            <h2>Professional Journey</h2>

        </div>


        <div class="timeline">


            <div class="timeline-item">

                <div class="timeline-dot"></div>

                <h3>
                    Software Engineer
                </h3>

                <div class="company">
                    Sofrecom – Orange Group
                </div>

                <div class="date">
                    2021 – Present · Tunisia
                </div>

                <p>

                    Working on enterprise applications and digital
                    solutions within an Agile/Scrum environment.

                </p>

                <ul>

                    <li>
                        Developed and maintained applications using
                        Java and Angular.
                    </li>

                    <li>
                        Analyzed functional requirements and translated
                        them into technical solutions.
                    </li>

                    <li>
                        Investigated and resolved application issues.
                    </li>

                    <li>
                        Collaborated with teams in Tunisia and France.
                    </li>

                    <li>
                        Participated in testing, code reviews and
                        application quality activities.
                    </li>

                    <li>
                        Contributed to application support and
                        incident resolution.
                    </li>

                </ul>

            </div>


            <div class="timeline-item">

                <div class="timeline-dot"></div>

                <h3>
                    Software Engineering Internship
                </h3>

                <div class="company">
                    Sofrecom – Orange Group
                </div>

                <div class="date">
                    February 2021 – September 2021
                </div>

                <p>

                    Contributed to the development and evolution of
                    enterprise applications while working in an Agile
                    and collaborative environment.

                </p>

            </div>

        </div>

    </div>

</section>



<!-- =========================
     PROJECTS
========================= -->

<section id="projects">

    <div class="container">

        <div class="section-title">

            <span>Projects</span>

            <h2>Selected Projects</h2>

            <p>
                A selection of projects that reflect my technical
                and analytical experience.
            </p>

        </div>


        <div class="projects-grid">


            <!-- PROJECT 1 -->

            <div class="project-card">

                <div class="project-header">

                    <h3>
                        Echat – Messaging Platform
                    </h3>

                </div>

                <div class="project-body">

                    <p>

                        Worked on a messaging platform within the
                        Orange ecosystem, supporting digital
                        conversations and customer interactions.

                    </p>

                    <p>

                        My contribution included frontend development,
                        API integration, troubleshooting and
                        collaboration with Orange France teams.

                    </p>

                    <div class="tags">

                        <span class="tag">Angular</span>

                        <span class="tag">TypeScript</span>

                        <span class="tag">RxJS</span>

                        <span class="tag">Java</span>

                        <span class="tag">REST APIs</span>

                        <span class="tag">LivePerson</span>

                        <span class="tag">Jenkins</span>

                        <span class="tag">Jira</span>

                    </div>

                </div>

            </div>


            <!-- PROJECT 2 -->

            <div class="project-card">

                <div class="project-header">

                    <h3>
                        Billing Application – UI Modernization
                    </h3>

                </div>

                <div class="project-body">

                    <p>

                        Contributed to the modernization of user
                        interfaces for a billing application serving
                        consumer customers.

                    </p>

                    <p>

                        Worked on frontend development, REST API
                        integration, testing and troubleshooting
                        while collaborating with the technical team.

                    </p>

                    <div class="tags">

                        <span class="tag">Angular</span>

                        <span class="tag">Java</span>

                        <span class="tag">Spring</span>

                        <span class="tag">REST APIs</span>

                        <span class="tag">Maven</span>

                        <span class="tag">Jenkins</span>

                        <span class="tag">Git</span>

                    </div>

                </div>

            </div>

        </div>

    </div>

</section>



<!-- =========================
     SKILLS
========================= -->

<section id="skills">

    <div class="container">

        <div class="section-title">

            <span>Skills</span>

            <h2>Technical Skills</h2>

        </div>


        <div class="skills-container">


            <div class="skill-group">

                <h3>
                    Development
                </h3>

                <div class="skill-list">

                    <span class="skill">Java</span>
                    <span class="skill">Spring Boot</span>
                    <span class="skill">Angular</span>
                    <span class="skill">TypeScript</span>
                    <span class="skill">JavaScript</span>
                    <span class="skill">RxJS</span>
                    <span class="skill">REST APIs</span>
                    <span class="skill">SQL</span>

                </div>

            </div>


            <div class="skill-group">

                <h3>
                    Tools & DevOps
                </h3>

                <div class="skill-list">

                    <span class="skill">Git</span>
                    <span class="skill">GitHub</span>
                    <span class="skill">Maven</span>
                    <span class="skill">Jenkins</span>
                    <span class="skill">SonarQube</span>
                    <span class="skill">Docker</span>
                    <span class="skill">Postman</span>
                    <span class="skill">Jira</span>

                </div>

            </div>


            <div class="skill-group">

                <h3>
                    Methods
                </h3>

                <div class="skill-list">

                    <span class="skill">Agile</span>
                    <span class="skill">Scrum</span>
                    <span class="skill">Business Analysis</span>
                    <span class="skill">Functional Analysis</span>
                    <span class="skill">Application Support</span>
                    <span class="skill">Problem Solving</span>

                </div>

            </div>

        </div>

    </div>

</section>



<!-- =========================
     BUSINESS ANALYSIS
========================= -->

<section>

    <div class="container">

        <div class="section-title">

            <span>Business Analysis</span>

            <h2>Bridging Business & Technology</h2>

        </div>


        <div class="analysis-box">

            <p>

                My technical background allows me to understand both
                business requirements and technical constraints.
                I enjoy working at the intersection of business and IT
                to help teams build useful and reliable solutions.

            </p>


            <div class="analysis-list">

                <div>
                    ✓ Requirements analysis
                </div>

                <div>
                    ✓ Business needs understanding
                </div>

                <div>
                    ✓ Functional analysis
                </div>

                <div>
                    ✓ Technical analysis
                </div>

                <div>
                    ✓ Stakeholder collaboration
                </div>

                <div>
                    ✓ Application improvement
                </div>

                <div>
                    ✓ Application support
                </div>

                <div>
                    ✓ Problem solving
                </div>

            </div>

        </div>

    </div>

</section>



<!-- =========================
     EDUCATION
========================= -->

<section>

    <div class="container">

        <div class="section-title">

            <span>Education</span>

            <h2>Academic Background</h2>

        </div>


        <div class="education-card">

            <h3>
                National Engineering Degree in Software Development
            </h3>

            <div class="school">
                Institut Supérieur d'Informatique – Tunisia
            </div>

            <p>

                Engineering degree focused on software development,
                information systems and software engineering.

            </p>

        </div>

    </div>

</section>



<!-- =========================
     CAREER GOALS
========================= -->

<section class="career">

    <div class="container">

        <div class="section-title">

            <span>Career Goals</span>

            <h2>What I'm Looking For</h2>

            <p>
                The next opportunity where I can create value,
                learn and grow.
            </p>

        </div>


        <div class="career-content">

            <p>

                I am looking for a collaborative environment where
                I can combine my technical background, analytical
                skills and interest in business needs to contribute
                to meaningful IT projects.

            </p>


            <div class="career-tags">

                <span class="career-tag">
                    IT Business Analyst
                </span>

                <span class="career-tag">
                    Senior IT Business Analyst
                </span>

                <span class="career-tag">
                    Functional Analyst
                </span>

                <span class="career-tag">
                    IT Project Analyst
                </span>

                <span class="career-tag">
                    Software Engineer
                </span>

                <span class="career-tag">
                    Application Support
                </span>

            </div>

        </div>

    </div>

</section>



<!-- =========================
     CONTACT
========================= -->

<section id="contact">

    <div class="container">

        <div class="section-title">

            <span>Contact</span>

            <h2>Let's Connect</h2>

            <p>

                Interested in working together or discussing
                an opportunity? Feel free to reach out.

            </p>

        </div>


        <div class="contact-container">

            <div class="contact-buttons">

                <!-- Replace your email -->

                <a
                    href="mailto:YOUR.EMAIL@EXAMPLE.COM"
                    class="btn btn-primary">

                    Email Me

                </a>


                <!-- Replace with your LinkedIn -->

                <a
                    href="https://www.linkedin.com/in/YOUR-LINKEDIN/"
                    target="_blank"
                    class="btn btn-secondary">

                    LinkedIn

                </a>


                <!-- Your GitHub -->

                <a
                    href="https://github.com/amal-ben-khelifa"
                    target="_blank"
                    class="btn btn-secondary">

                    GitHub

                </a>

            </div>

        </div>

    </div>

</section>



<!-- =========================
     FOOTER
========================= -->

<footer>

    © 2026 Amal Ben Khelifa. All rights reserved.

</footer>



<!-- =========================
     JAVASCRIPT
========================= -->

<script>

    const menuBtn = document.getElementById("menuBtn");
    const navLinks = document.getElementById("navLinks");

    menuBtn.addEventListener("click", () => {

        navLinks.classList.toggle("active");

    });


    document.querySelectorAll(".nav-links a").forEach(link => {

        link.addEventListener("click", () => {

            navLinks.classList.remove("active");

        });

    });

</script>


</body>
</html>
