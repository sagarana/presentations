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
### Collections budget & data

notes: This is a simplified hypothetical example of managing collection budget spending, based on a real scenario in a top Canadian academic library, not naming any names. Imagine you are in a librarian role which includes the responsibility for selecting and purchasing collection materials: ebooks, print books, journal subscriptions, etc. 

---
### Collections budget & data
![Suballocations](media/scenario1-1-bg.png)

notes: A specific amount of money is allocated for these purchases. Seems simple enough?

---

### Collections budget & data
![Suballocations](media/scenario1-2-bg.png)

notes: Data lives within multiple systems: vendor and publisher platforms, the ILS or LMP (library management platform), and the university's financial systems. The fund allocation for your purchases is actually shared by everyone on your team, each purchasing for multiple subject areas or languages or formats. The fund balances live in the ILS; with other expenditure data in the financial systems; but you create and view your selections and orders in the vendor system, where the fund names and codes are mapped to but not the same as the ILS. You can't tell how much your colleagues have spent already, or on what. How do you manage this spending? ... Some people might keep their own spreadsheets in which they manually transcribe orders and costs and keep track of the math, perhaps collaborating with the rest of their team. It's not ideal: invoiced costs sometimes differ from order prices, there's currency exchange, other charges. It's a lot of manual accounting and trust in a uniform process across many individuals.

---
### Collections budget & data
![Suballocations](media/scenario1-3-bg.png)

notes: I can help. Luckily, we have direct access to the ILS and financial databases. Working with the selectors (and their head/manager) we create a spreadsheet dividing up the allocated money into buckets managed by each member of the team, called sub-allocations. I pull all of that data together in a single Tableau report, which updates auotmatically on a daily schedule, so that each sub-allocation can be tracked by you, the selectors. Tableau reporting also allows managers, branch heads, AULs, and finance staff to monitor spending in other ways: print or e, government or endowment funded, tax brackets, shipping, currency of purchase, and so on.

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

### Managing data

- Data integrity and cleanup
- Storage and access
- Methods and systems change over time
- Description, communication

notes: Data can be quantitative, qualitative, structured or unstructured. Data integrity: is data good, complete, accurate, consistent? Who created it, how has it managed over time, how well does it represent the real world? Can we improve it by correcting errors, standardizing and normalizing, filling in gaps? The context of longitudinal data is of note - libraries do a lot of year-over-year analysis, and we have datasets that go back decades. Data collection methods, analysis and management vary considerably when comparing data from 2005,to 2015, to 2025. Documentation is very important, and often challenging.

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
### Gate Counts

notes: _Meghan to present this. Workflow emphasizes long history, various collection formats, library closures, inconsistencies in reporting. How to give context and use responsible. Importance of normalization. Data integrity._ "Gate count" is a standardized definition set by ARL: "the number of persons who physically enter the library in a year." This statistic is included in the annual Report to the Senate, as well as many annual statistical surveys administered by academic library organizations such as ARL, CARL, CPSLD, and others. 

---

### Gate Counts
![Gate count workflow](media/workflow2-1-bg.png)

notes: At UBC Library, we collect daily counts of patrons entering the branches as recorded by electronic gates at entrances. This usually requires noting the number on the electronic counter before the library opens and at the end of the day after closing, at a minimum. The actual gates have different manufacturers depending on when they were installed; some count entrances and exits, some exits only. Their counters have digit limits and reset after a certain number, e.g. 100,000. The data can be used to inform decisions on desk staffing, open hours, and other public services. Seems simple enough? Of course not...


---

### Gate Counts
![Gate count workflow](media/workflow2-2-bg.png)

notes: Surprise: this is _still_ an oversimplified representation of managing gate count data. Multiple library branches, some of which have no gates, some one, some multiple; some count twice per day, some multiple times per day, and there can be gaps; open hours are different for each branch, term, year. All of the variables change over each year, each term, and even day-to-day depending on staffing practices or any interruptions to regular routines. The timeline represents a small selection of factors that help provide context to the data: methods varying from recording and calculating by hand to automatic collection. Even with LibInsight, our online platform, most people probably jot down numbers on paper and/or use a calculator to get the count from the physical gate counter screen to the digital record. You might think having the gates automatically load data into a database would be preferable; there are pros and cons: it's more expensive, a separate system/vendor/software, and the database exports canned reports in one format that can't be edited.

---

### Gate Counts
![Gate count workflow](media/workflow2-3-bg.png)

notes: When we migrated to LibInsight, we worked on big project to clean, merge, reshape and analyze the gate count data from the past ten or so years, most of which came from spreadsheets manually maintained by staff. This historical data is then unioned with current data we extract out of LibInsight via API (which also gets archived annually). I've also brought in Open Hours data, which lives in a database managed by Library IT and updated by staff. The Tableau report is accessible to all staff online and updates automatically. We use this for the core purpose of getting the single ARL stat of "how many people visit the library in a year" as well as vizualizations, access to raw data, and detailed, granular analysis of all fields: e.g. average gate count on weekdays vs. weekends, or visits per hour in a year.

---

### Gate Counts
![Gate count workflow](media/tableau-gate-count-by-year.png)

notes: Here's one of the dashboards from the Tableau report. This shows gate count, hours open, and visits per open hour in 2023 and 2024. Think about meaning and context: what does it mean for a branch to be busy? Can you say one branch is busier than another, or that visits have increased from one year to the next? If you have a similar number of visitors in 2023 and 2024, but in 2024 the open hours were reduced signficantly, we would see a significant increase in "visits per open hour" (though little to no change to the total number of visitors in the year). This is an example of normalizing to a common denominator to allow meaningful comparisons and analysis, and help inform planning and decision-making like "should we stay open until 6pm or 9pm"?
