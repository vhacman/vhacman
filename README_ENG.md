<div align="center">

# Hacman Viorica Gabriela
### 42 Roma Luiss · Generation Italy — Software Engineer & Java Full Stack Developer

[![Java](https://img.shields.io/badge/Java-21-ED8B00?style=flat&logo=openjdk&logoColor=white)](https://openjdk.org/)
[![Spring Boot](https://img.shields.io/badge/Spring_Boot-4.0.2-6DB33F?style=flat&logo=springboot&logoColor=white)](https://spring.io/projects/spring-boot)
[![Node.js](https://img.shields.io/badge/Node.js-339939?style=flat&logo=node.js&logoColor=white)](https://nodejs.org/)
[![C](https://img.shields.io/badge/C-00599C?style=flat&logo=c&logoColor=white)](https://en.wikipedia.org/wiki/C_(programming_language))
[![MySQL](https://img.shields.io/badge/MySQL-8.x-4479A1?style=flat&logo=mysql&logoColor=white)](https://www.mysql.com/)
[![MapStruct](https://img.shields.io/badge/MapStruct-1.6.3-E94E1B?style=flat&logo=java&logoColor=white)](https://mapstruct.org/)
[![JUnit5](https://img.shields.io/badge/JUnit-5-25A162?style=flat&logo=junit5&logoColor=white)](https://junit.org/junit5/)
[![Maven](https://img.shields.io/badge/Maven-3.9-C71A36?style=flat&logo=apachemaven&logoColor=white)](https://maven.apache.org/)

📖 **Read this in other languages:** 🇬🇧 English | [🇮🇹 Italiano](./README.md)

</div>

---

## About Me

From studying languages and cultures to writing code — my journey into tech started with curiosity and a desire for change. With a degree in **Languages and European Cultures (L11)** and years of experience in customer service and team management, I know how to work under pressure, solve problems on the spot, and communicate across different worlds.

Now I'm fully committed to software development: studying **low-level C/C++** at **42 Roma** and **enterprise Java** at **Generation Italy**, simultaneously.   I have learned that persistence beats perfection, every time.

---

## Featured Projects

### Grecos Pizzeria — Digital Menu & Admin Panel

[![Angular](https://img.shields.io/badge/Angular-21-DD0031?style=flat&logo=angular&logoColor=white)](https://angular.dev/)
[![Firebase](https://img.shields.io/badge/Firebase-Firestore_%2B_Auth_%2B_Hosting-FFCA28?style=flat&logo=firebase&logoColor=black)](https://firebase.google.com/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.9-3178C6?style=flat&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Bootstrap](https://img.shields.io/badge/Bootstrap-5.3-7952B3?style=flat&logo=bootstrap&logoColor=white)](https://getbootstrap.com/)
[![PWA](https://img.shields.io/badge/PWA-installabile-5A0FC8?style=flat&logo=pwa&logoColor=white)](https://web.dev/progressive-web-apps/)
[![Live](https://img.shields.io/badge/Live-grecospizzeria--47768.web.app-4CAF50?style=flat&logo=firebase&logoColor=white)](https://grecospizzeria-47768.web.app)

A full-stack web application built for **Grecos Pizzeria** (Rome, Italy): customers scan a QR code and browse the full menu on their phone, while staff manage everything from a secure admin panel — no app store required.

**Client:** Grecos Pizzeria (@grecos11) · **Version:** v1.9.0 · **Deployed:** March 2026

#### What it does

| Area | Features |
|------|----------|
| **Public Menu** | 6 categories (Antipasti, Pizze Rosse, Pizze Bianche, Focacce & Calzoni, Dolci, Bevande) · real-time allergen filter (14 EU allergens) · vegan/frozen indicators · sticky category navbar · "Specialità" tab for nightly specials · bottom-sheet dish detail · chip-based category cards with direct deep-links · Google/TripAdvisor review links |
| **Admin Panel** | Secure login · dish management (add/edit/toggle/delete) · ingredient availability · daily message banner · desktop & tablet two-column CSS Grid layout · maintenance mode · inline dish editing · SHA-256 hashed cash calculator password |
| **Reservations** | Weekly calendar (Thu/Fri/Sat/Sun) up to 12 months · daily KPIs (tables, covers, high-chairs) · add/edit/delete with confirmation · arrived toggle · walk-in bottom-sheet · real-time toast notifications · WhatsApp PNG sharing · PDF export (daily/monthly/yearly) · dynamic closure messages |
| **Takeaway Orders** | Smart autocomplete by category (startsWith filter) · per-order discount with automatic calculation · delivery toggle · free-time input · close orders toggle · PDF summary with daily revenue (daily/monthly/yearly) · dynamic closure messages |
| **Tools** | QR code generator with brand logo · dedicated QR per category (e.g. Dolci) · QR for Google/TripAdvisor reviews · Web Share API (native mobile share + clipboard fallback) |
| **Analytics** | Visit counter · device breakdown · peak hours · most-visited categories · top-10 most-viewed dishes · 7/30 day selector with auto-refresh every 3 min · Microsoft Clarity behavioral analytics (localhost filtered) |
| **Extras** | Summer/winter mode (auto open days) · closure periods with homepage banner · evening history archive · installable PWA with iOS/Android-specific install instructions · swipe-to-dismiss on all modals · IntersectionObserver scroll detection · Firestore production security rules (per-collection, admin-only writes) · `memoryLocalCache()` (replaces IndexedDB to prevent corruption) |

#### Architecture

```
Angular 21 (standalone components · signals · toSignal)
Firebase Firestore   — real-time menu & booking data (memoryLocalCache)
Firebase Auth        — admin authentication
Firebase Hosting     — CDN deployment with optimized cache headers
Bootstrap 5.3 + Angular Material 21
PDF generation       — jsPDF (offline-ready, no print dialogs)
Behavioral analytics — Microsoft Clarity (localhost filtered)
QR generation        — qrcode library (dynamic, downloadable PNG)
```

#### Evolution

| Version | Highlight |
|---------|-----------|
| v1.0.0 | Public menu (115 dishes), allergen filter, admin CRUD, fuori-menu, QR code, PWA |
| v1.1.0 | jsPDF export (availability, QR, evening archive) · advanced analytics (auto-refresh, scrollable charts, peak hours, device KPIs) · evening history archive |
| v1.2.0 | Full reservations (calendar, KPIs, real-time toasts, PDF) · takeaway autocomplete with auto-price · dish bottom-sheet · `memoryLocalCache` replaces IndexedDB |
| v1.3.0 | Specialità tab · branded QR codes · `?cat=` deep-links · Web Share API · WhatsApp · user manual PDF |
| v1.4.0 | Kitchen close confirmation + auto-reopen at 06:00 · Firestore per-collection security rules |
| v1.5.0 | Android/iOS responsive fixes · monthly/yearly PDF · walk-in bottom-sheet · WhatsApp PNG sharing · inline booking edit · swipe-to-dismiss modals |
| v1.6.0 | Predeploy auto-build hook · optimized cache headers · Microsoft Clarity localhost filter |
| v1.7.0 | Dynamic closure messages for reservations and takeaway popups |
| v1.8.0 | Desktop/tablet CSS Grid layout · menu view in dashboard · SHA-256 password-protected cash calculator |
| v1.8.1–v1.8.2 | Per-order discount · delivery toggle · automatic cash calculation · low-stock threshold ≤ 5 |
| v1.8.4–v1.8.5 | Booking form critical fixes (ViewEncapsulation) · maintenance mode · client-side Firestore sort |
| v1.9.0 | Google/TripAdvisor review QR codes · chip-category menu cards · IntersectionObserver scroll detection |

---

## Education & Training

---

### <img src="https://img.shields.io/badge/42-Roma_Luiss-2BA5DE?style=flat&logo=42&logoColor=white" alt="42 School"> Low-Level Programming & System Administration

**October 2024 – Present** · Peer-to-peer learning

![C](https://img.shields.io/badge/C-00599C?style=flat&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat&logo=cplusplus&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat&logo=gnubash&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)

**Skills acquired:** memory management, system calls, process & signal management, concurrent programming (threads, mutexes, semaphores), networking (TCP/IP, subnetting), graphics (MinilibX), C++ OOP & STL, Linux system administration.

| Project | Description | Technologies | Score |
|---------|-------------|-------------|:-----:|
| [Minishell](https://github.com/vhacman/minishell) | Complete shell with pipelines, redirections, built-ins | C, fork, pipe, execve | 100/100 |
| [Philosophers](https://github.com/vhacman/philo) | Dining philosophers — synchronization | C, pthread, mutex | 100/100 |
| [so_long](https://github.com/vhacman/so_long) | 2D game with MinilibX | C, MinilibX | 122/100 ⭐ |

[![All 14 projects →](https://img.shields.io/badge/All_14_projects_with_scores-2BA5DE?style=flat&logo=42&logoColor=white)](https://github.com/vhacman/42_RomaLuiss/blob/main/README.md)

[![vhacman's 42 stats](https://badge.mediaplus.ma/starryblue/vhacman)](https://github.com/oakoudad/badge42)

---

### <img src="https://img.shields.io/badge/Generation-Italy-FF6B35?style=flat&logo=java&logoColor=white" alt="Generation Italy"> Java Junior Full Stack Developer Bootcamp

**December 2024 – April 2025** · 500h official curriculum + self-study (15 weeks)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white)
![Spring](https://img.shields.io/badge/Spring-6DB33F?style=flat&logo=spring&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat&logo=springboot&logoColor=white)
![Hibernate](https://img.shields.io/badge/Hibernate-59666C?style=flat&logo=hibernate&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-005C84?style=flat&logo=mysql&logoColor=white)
![MapStruct](https://img.shields.io/badge/MapStruct-E94E1B?style=flat&logo=java&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)

**Key achievements:**
- **84+ projects** across 4 areas: fundamentals, business applications, Spring Boot, frontend
- **13 Spring Boot web applications** — REST APIs, JPA, Thymeleaf, MapStruct, Lombok
- **Custom ORM framework** built from scratch with Generic Repository Pattern and Full/Partial caching
- **Advanced design patterns**: Repository, IoC Container, ETL, State, Command, Chain of Responsibility, Lazy/Eager Loading
- **Healthcare scheduling algorithms**: smart calendar management with LinkedHashMap and advanced Comparators
- **Food delivery platform** evolved across two iterations (JavaEat v01 → v02) with MapStruct and ManyToMany relationships

#### Repositories

| # | Repository | Contenuto |
|---|------------|-----------|
| 00 | [00_libraries](https://github.com/vhacman/00_libraries) | Framework e librerie riutilizzabili (GenerationLibrary) |
| 01 | [01_fundamentals_examples](https://github.com/vhacman/01_fundamentals_examples) | Fondamenti Java e OOP — 12 moduli |
| 02 | [02_tickets_transportation](https://github.com/vhacman/02_tickets_transportation) | Sistemi di biglietteria e trasporti — 9 progetti |
| 03 | [03_Business_Applications](https://github.com/vhacman/03_Business_Applications) | Applicazioni gestionali enterprise — 43 progetti |
| 04 | [04_Exercises_Practice](https://github.com/vhacman/04_Exercises_Practice) | Esercizi supplementari — 4 progetti |
| 05 | [05_Spring-FrontEnd---FullStack](https://github.com/vhacman/05_Spring-FrontEnd---FullStack) | Spring Boot + REST API + Frontend — 16 progetti |
| 06 | [06_Angular-Frontend](https://github.com/vhacman/06_Angular-Frontend) | Angular 21 — 9 applicazioni |
| 07 | [07_FullStack-NodeJS-Angular](https://github.com/vhacman/07_FullStack-NodeJS-Angular) | FullStack Node.js + Express + SQLite + Angular |
| 08 | [08_FullStack-SpringBoot](https://github.com/vhacman/08_FullStack-SpringBoot) | FullStack Spring Boot + Angular — 3 progetti |
| 09 | [09_Database-MySql](https://github.com/vhacman/09_Database-MySql) | SQL fondamentali e query avanzate |

[![Technical Documentation](https://img.shields.io/badge/Technical_Documentation-Notes_&_Guides-181717?style=flat&logo=github)](https://github.com/vhacman/documentazioneTecnica)
&nbsp;
[![Course Materials](https://img.shields.io/badge/Course_Materials-Drive_Folder-4285F4?style=flat&logo=googledrive&logoColor=white)](https://drive.google.com/drive/folders/1f54Eu_EK2zw2XcMK-9qJH4ZErLXtV8Rj?hl=it)

---

## Soft Skills

| Area | Competenze |
|------|-----------|
| **Mindset** | Adattabilità · Mentalità di crescita · Zona di comfort · Persistenza |
| **Autogestione** | Gestione del tempo · Responsabilità personale · Proattività vs reattività |
| **Team** | Gruppo vs. squadra · Comunicazione · Collaborazione remota |
| **Tech Context** | Ruolo Scrum Master · AI generativa per il lavoro |
| **Agile & Scrum** | Sprint Planning · Sprint Backlog · Scrum Board · Roadmap · Cerimonie Agile |

#### Progetto di Gruppo — *"ShareSphere"*

Team project con metodologia Scrum completa: analisi delle richieste cliente, patto sociale del team, user story, sprint backlog, sprint planning, scrum board, roadmap, mockup desktop & mobile (homepage, profilo, pannello admin, blog, feedback) e resoconto sprint.

---

## Tech Skills

| Area | Technologies |
|------|-------------|
| **Backend** | ![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white) ![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat&logo=springboot&logoColor=white) ![Hibernate](https://img.shields.io/badge/Hibernate-59666C?style=flat&logo=hibernate&logoColor=white) ![MapStruct](https://img.shields.io/badge/MapStruct-E94E1B?style=flat&logo=java&logoColor=white) ![JUnit](https://img.shields.io/badge/JUnit-25A162?style=flat&logo=junit5&logoColor=white) ![Node.js](https://img.shields.io/badge/Node.js-339939?style=flat&logo=node.js&logoColor=white) ![Express](https://img.shields.io/badge/Express-000000?style=flat&logo=express&logoColor=white) |
| **Low-Level** | ![C](https://img.shields.io/badge/C-00599C?style=flat&logo=c&logoColor=white) ![C++](https://img.shields.io/badge/C++-00599C?style=flat&logo=cplusplus&logoColor=white) ![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat&logo=gnubash&logoColor=white) ![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black) |
| **Database** | ![MySQL](https://img.shields.io/badge/MySQL-005C84?style=flat&logo=mysql&logoColor=white) ![SQLite](https://img.shields.io/badge/SQLite-07405E?style=flat&logo=sqlite&logoColor=white) ![MySQL Workbench](https://img.shields.io/badge/MySQL_Workbench-4479A1?style=flat&logo=mysql&logoColor=white) ![DBeaver](https://img.shields.io/badge/DBeaver-3F2C53?style=flat&logo=dbeaver&logoColor=white) |
| **Frontend** | ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white) ![Angular](https://img.shields.io/badge/Angular-DD0031?style=flat&logo=angular&logoColor=white) |
| **Cloud & DevOps** | ![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat&logo=firebase&logoColor=black) ![PWA](https://img.shields.io/badge/PWA-5A0FC8?style=flat&logo=pwa&logoColor=white) |
| **Versioning & Tools** | ![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white) ![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white) ![Maven](https://img.shields.io/badge/Maven-C71A36?style=flat&logo=apachemaven&logoColor=white) ![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat&logo=postman&logoColor=white) |
| **IDE & Editor** | ![IntelliJ IDEA](https://img.shields.io/badge/IntelliJ-000000?style=flat&logo=intellijidea&logoColor=white) ![VSCode](https://img.shields.io/badge/VSCode-007ACC?style=flat&logo=visualstudiocode&logoColor=white) ![Eclipse](https://img.shields.io/badge/Eclipse-2C2255?style=flat&logo=eclipse&logoColor=white) ![Vim](https://img.shields.io/badge/Vim-019733?style=flat&logo=vim&logoColor=white) |
| **AI & Prompting** | ![Claude Code](https://img.shields.io/badge/Claude_Code-CC785C?style=flat&logo=anthropic&logoColor=white) ![Kilo Code](https://img.shields.io/badge/Kilo_Code-6C47FF?style=flat&logo=visualstudiocode&logoColor=white) ![ChatGPT](https://img.shields.io/badge/ChatGPT-74aa9c?style=flat&logo=openai&logoColor=white) ![Gemini](https://img.shields.io/badge/Gemini-8E75B2?style=flat&logo=googlegemini&logoColor=white) ![Perplexity](https://img.shields.io/badge/Perplexity-20808D?style=flat&logo=perplexity&logoColor=white) ![Lovable](https://img.shields.io/badge/Lovable-FF3D6B?style=flat&logo=htmx&logoColor=white) |
| **Productivity** | ![Notion](https://img.shields.io/badge/Notion-000000?style=flat&logo=notion&logoColor=white) ![Discord](https://img.shields.io/badge/Discord-5865F2?style=flat&logo=discord&logoColor=white) ![Canva](https://img.shields.io/badge/Canva-00C4CC?style=flat&logo=canva&logoColor=white) ![Microsoft Office](https://img.shields.io/badge/Microsoft_Office-D83B01?style=flat&logo=microsoft&logoColor=white) |

**Design Patterns:** `Repository` · `MVC` · `IoC / DI Container` · `Factory` · `Strategy` · `State` · `Command` · `Chain of Responsibility` · `Template Method` · `Custom ORM` · `Reflection` · `Lazy/Eager Loading` · `ETL` · `DTO/Mapper`

---

## GitHub Statistics

<div align="center">

![Profile Views](https://komarev.com/ghpvc/?username=vhacman&label=Profile+views&color=0e75b6&style=for-the-badge)

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=vhacman&show_icons=true&theme=tokyonight&hide_border=true&count_private=true&include_all_commits=true)

![GitHub Streak](https://github-readme-streak-stats.herokuapp.com/?user=vhacman&theme=tokyonight&hide_border=true)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=vhacman&layout=compact&theme=tokyonight&hide_border=true&langs_count=8)

![GitHub Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=vhacman&theme=tokyo-night&hide_border=true&area=true)

![GitHub Trophies](https://github-profile-trophy.vercel.app/?username=vhacman&theme=tokyonight&no-frame=true&row=1&column=7)

</div>


## Academic Background

| | |
|---|---|
| **Generation Italy** | Java Junior Full Stack Developer Bootcamp · Dec 2024 – Mar 2025 |
| **42 Roma Luiss** | Software Engineering (C/C++, Low-Level, Systems) · Mar 2024 – Present |
| **Università e-Campus** | Languages and European Cultures L11 · 2022 – 2024 · 95/110 |
| **Future Academy** | Master in Social Media Management · 2022 – 2023 |
| **Linguistic High School** | Italian, English, German, French · 2013 – 2018 · 95/100 |

---

## Languages

🇷🇴 Romanian — Native &nbsp;|&nbsp; 🇮🇹 Italian — Native &nbsp;|&nbsp; 🇬🇧 English — Intermediate High (B2) &nbsp;|&nbsp; 🇩🇪 German — Intermediate &nbsp;|&nbsp; 🇫🇷 French — Intermediate

---

## Connect

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Viorica_Gabriela_Hacman-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/viorica-gabriela-hacman-63a412267/)
[![Email](https://img.shields.io/badge/Email-hacmanvioricagabriela%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:hacmanvioricagabriela@gmail.com)
[![42 Profile](https://img.shields.io/badge/42_Intra-vhacman-2BA5DE?style=for-the-badge&logo=42&logoColor=white)](https://profile.intra.42.fr/users/vhacman)
[![FreeCodeCamp](https://img.shields.io/badge/FreeCodeCamp-DevGabi98-0A0A23?style=for-the-badge&logo=freecodecamp&logoColor=white)](https://www.freecodecamp.org/DevGabi98)

</div>

---

> *"One step at a time, always learning"*

<div align="center">

⭐️ [vhacman](https://github.com/vhacman) · Ladispoli, Rome, Italy

</div>
