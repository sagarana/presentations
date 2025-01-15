## UBC Library operational data 
### Overview for LIBR559S 
\
\
Jeremy Buhler, _Data Librarian_  
Meghan Waitt, _Library Data Analyst_

notes: Introductions 

---
<!-- .slide: data-background="lightblue" -->
### What we'll cover

- Types of operational data in academic libraries 
- Value of this data in workflows and planning 
- Guiding principles for handling data 
- Tools and skills that make this possible

notes: In the next 40 minutes or so, Meghan and I want to provide a non-technical introduction to (read list).
I encourage you to make this more interesting for everyone by engaging with us: feel free to interrupt us along the way with questions or observations.

---

<!-- .slide: data-background="cornsilk" -->
_Tableau report demonstration_

notes: _quick show-and-tell to get their interest early? Otherwise we won't show Tableau until much later_

---
### What do we mean by _operational data_?

Data generated in the course of library operations or collected to support operational needs <!-- .element: class="fragment" -->

notes: You're in an RDM class that focuses on data generated in the course of research and that is often managed by libraries. Unlike RDM, our work is limited to _operational data_ which has a different source and purpose. Here's a working definition of operational data (click to show, then read). Our data work is more like business analysis or operational support, though many of the skills and values are the same. 

---
### The _Library Data Team_

- generates reports for Library employees <!-- .element: class="fragment" -->
- compiles data for statistical surveys <!-- .element: class="fragment" -->
- manages operational data collection <!-- .element: class="fragment" -->
- maintains data reporting platforms <!-- .element: class="fragment" -->

notes: That amounts to a lot of data coming from many systems. At UBC Library, the Library Data Team is responsible for collecting and providing access to library operational data, as well as for generating reports and completing statistical surveys. Currently the Library Data Team consists of just Meghan (full time) and me (half time). I'm proud of what we're able to accomplish with just one and a half positions. _Click through bullet points_. Embedded in these tasks are many others related to maintenance, documentation, training, and workflow development.

---

#### Example: Annual Report to Senate 

![2023/24 Senate Report figures](media/senate_report.png)

<https://about.library.ubc.ca/news/publications/senate-report-2023-2024/> <!-- .element: class="small" -->

notes: at the most basic level, operational data compiled by the data team makes it into statistical surveys that allow for comparison among libraries, as well as reports like this UBC Library Annual Report to Senate. Behind each of those data points is a workflow - in some cases quite complex - to collect the relevant data from across the library system.

I refer to this kind of use as _basic_ because it's relatively static one-way reporting. It's important to communicate what we do, but a more in-depth and meaningful application of operation data - in my view - is to use it for assessing and planning services, and to improve internal workflows.  

---
<!-- .slide: data-background="lightblue" -->
## Types of operational data

---

- generated automatically by library systems 
- collected/compiled by library employees <!-- .element: class="fragment" -->


notes: broadly speaking, most operational data comes from two channels. _click to show_: a lot of the operational data is generated automatically by library systems, accounts, and platforms. Think about the Library Management Platform (LPM), or the older term Integrated Management System (ILS). This is the system at the heart of day-to-day library operations, that tracks the collection, acquisitions, use, and so on. Thousands of transactions are recorded per day and depending on the system might be available to library employees in a reporting interface, by querying a database directly, or through an API.

The other method is my collecting and compiling the data ourselves. Examples include gate counts, patron questions. UBC Library has online tools like SpringShare's LibInsight platform to help with data collection, but that information is entered by library employees.

---
<!-- .slide: data-background="cornsilk" -->
### Think of examples
_data generated automatically_  <!-- .element: class="fragment semi-fade-out" data-fragment-index="1" -->

_data compiled by employees_ <!-- .element: class="fragment" data-fragment-index="1" -->

notes: _Prompt for responses from the group for each channel. Put columns on board, then fill gaps if necessary_ 

---
<!-- .slide: data-background="lightblue" -->
## The value of operational data

notes: _section title slide, transition from 'types' to 'value' of data_. So we've listed many kinds of data. What is it actually good for? Why should anyone care about it?

---

- external reporting
- internal planning, workflows, assessment

notes: _read bullets, after each describe in a few sentences. In this new section emphasis on why this work is important, who it benefits, etc._ 

To help illustrate we'll share two scenarios that involve operational data reporting. In each scenario, emphasize value of data for time-saving, reducing errors, better decision making, etc. _Each example could include images to illustrate how we supported them: e.g. screenshot of a Tableau report, illustration of a data workflow._

---
<!-- .slide: data-background="cornsilk" -->
### Scenario 1
Placeholder for descriptive title or phrase 

notes: _Meghan to present scenario related to collections budget or spending_
a scenario where a library employee (GAA?) is faced with a large manual transcribing job, with data that's already available. We can provide a spreadsheet, they'd have to web scrape.

---
<!-- .slide: data-background="cornsilk" -->
### Scenario 2
Placeholder for descriptive title or phrase 

notes: _Jeremy to present scenario where a manual transcribing job could be eliminated or simplified_ 

---
<!-- .slide: data-background="lightblue" -->
## Guiding principles for handling data

notes: _Proposed new section to highlight values that inform our work (section also added to outline slide at beginning). This is a good place to talk about our training and documentation efforts, the work it takes to present data responsibly, being available to all library employees, the importance of normalization, the preference for direct access to disagregated data (because out-of-the-box eventually comes up short), etc._

At least some slides in this section could have prompts for student engagement, possibly references to the way that would also apply in RDM (e.g. describing data). I suggest we use our Tableau setup as a recurring thread through this section.

---

### Library Data Team's role as interpreter

- Consultations like reference interviews
- Need to understand library context
- Familiar with technology and tools
- Help others understand what's possible

notes: The Library data team acts as a bridge between library operations/employees and the data.

---

### Available to all library employees

notes: _stress this isn't an admin unit, it's meant to be integrated into work at all levels, wherever it is helpful._

Could we use this as a bridge to introduce our Tableau setup? E.g. everyone has accounts, unless reports are confidential anyone can browse them, etc. If so, the subsequent slides in this section could, where applicable, show a Tableau report that expresses that value. For example: dashboard tabs with instructions; data that's normalized before being presented; ability to export underlying data; 

---

### Data integrity, cleanup, providing context

notes: Meghan

---

### Data literacy/education

notes:

---

### Preference for disaggregated data

notes:

---

<!-- .slide: data-background="lightblue" -->
## Operational data workflows

notes: _describe two operational data workflows to help students understand the range of tools involved, and the effort involved in presenting an accessible report or dashboard. The workflows should also include examples of how the data gets used._

---
<!-- .slide: data-background="cornsilk" -->
### Workflow 1
Improving access to Google Analytics data about website use

notes: highlight the API -> TSV -> Tableau (Google Analytics)

---
<!-- .slide: data-transition="slide-in none-out" -->
![GA data flow](media/ga_data_flow_1.png)

notes: 

---

<!-- .slide: data-transition="none-in zoom-out" -->
![GA data flow](media/ga_data_flow_2.png)

notes: at the end of every month the Library Data Team takes snapshots of the month's website activity and stores them in TSV files on the T: drive. This happens automatically with Python scripts that harvest selected dimensions and metrics using the Google Analytics API. We don't harvest all the data, but enough to answer many website activity questions.  

---

<!-- .slide: data-transition="zoom-in fade-out" data-background-image="media/tsv_view.png" -->

notes: These TSV files are stored in a T: drive directory that's visible to everyone. Some of the files are large (the pages file has more than 3M rows) and won't open in software like Excel, but they're available to anyone who wants to analyze the data themselves. 


---

<!-- .slide: data-transition="fade-in zoom-out" -->
![GA data flow](media/ga_data_flow_3.png)

notes: Most of us will prefer to move along to step three in the diagram, where these TSV files are turned into Tableau reports that are updated every month.

---

<!-- .slide: data-background-image="media/overview_report.png" data-transition="zoom-in none-out" -->

notes: here's an example of one of the Tableau dashboards. This one shows an overview of activity for the entire Library website from July 2023 to May 2024. Across the top you can filter by dimensions including the date, session source, device category, and medium. Even at a glance you can see that the overview graphs reflect the academic schedule, with a decrease in activity during the summer months and over the winter break.

---

<!-- .slide: data-background="cornsilk" -->
### Workflow 2
Compiling gate counts

notes: _Meghan to present this. Workflow emphasizes long history, various collection formats, library closures, inconsistencies in reporting. How to give context and use responsible. Importance of normalization. Data integrity._

---


