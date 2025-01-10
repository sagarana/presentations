<!-- .slide: data-background="darkseagreen" data-transition="none" -->

## Website activity data 
### Google Analytics overview 
\
\
Library Data Team, UBC Library\
<https://confluence.it.ubc.ca/display/ASMNT/Library+Data+Home><!-- .element: class="small" --> 


notes: Thanks for joining us today! My name is Jeremy Buhler, I'm the Data Librarian at UBC Library and a member of the Library Data Team, a group that compiles, manages, and provides access to data about UBC Library activities. 

Today's session is about website activity data collected by Google Analytics and - more importantly - how you can access that data to learn how UBC Library users interact with our website.

The session is being recorded and we intend to post an edited version on Confluence as a resource for others who want to learn about Google Analytics. Please don't let that stop you from engaging! I'll stop at several points for questions, and you're welcome to raise your hand or put questions in the chat at any time. Do take advantage of the fact that we're here in real time, and make the most of the session by engaging. 

---

<!-- .slide: data-background="seashell" data-transition="none-in slide-out" -->
### Library Data Team

- Jeremy Buhler, _Data Librarian_
- Brett Dimond, _Data Analyst and Curator_
- Meghan Waitt, _Library Data Analyst_

With help from TDUX and Library IT partners <!-- .element: class="fragment" style="color:darkgreen; font-style:italic" -->

notes: Much of the work we'll discuss today was done by the Library Data Team. I've already introduced myself, and Brett Dimond is also on the call today to help with the chat and Q&A. The work we did wouldn't have been possible with Brett, who set up the pipeline between Google Analytics and Tableau. Meghan's work is also prominent in today's presentation. She's currently away but deserves credit for all the Tableau reports you'll see today.

|| I also want to acknowledge the support of colleagues in TDUX and Library IT, especially Salma Lalji, Schuyler Lindberg, Mark Goodwin, and Rebecca Dickson.

---

<!-- .slide: data-background="seashell"  -->

### Session content

- What is Google Analytics?
- Google Analytics at UBC Library 
- Find and use website activity data


notes: So here's an outline of what we'll cover. Many of you are familiar with Google Analytics, but it will be new to some of you, so we'll start with an introduction to how it works. In the second part I'll provide an overview of How Google Analytics is set up at UBC Library, and then we'll show you how to find and use website activity data. 

---

<!-- .slide: data-background="seashell"  -->
### Additional resources in Confluence
<https://confluence.it.ubc.ca/display/ASMNT/Google+Analytics>

notes: nearly everything in this presentation is also documented in Confluence. The pages at this link are an excellent resource and can be used to orient new employees to website activity data at UBC Library.

---

<!-- .slide: data-transition="slide-in zoom-out" -->

### 2022/2023 Senate Report

![2022/23 Senate Report figures](media/senate_report_orange.png)

<https://about.library.ubc.ca/news/publications/senate-report-2022-2023/> <!-- .element: class="small" -->

notes: So, on to an example - here's _one_ place where UBC Library routinely uses website activity data. This is a screenshot of the most recent Senate Report. Underlined in orange is the total number of "visits" - or sessions - on the Library website that year. And now I want to hear from you: please write in the chat or put up your hand if you prefer to speak: 

- if you've used website activity data, what did you use if for? 
- if you haven't used website activity data before, what do you want to know about how users interact with our website?
- and for everyone, are there projects where you expect to need this kind of data?

We have time... please do provide examples and I'll do my best to incorporate them into the session. 

Thank you for those examples! My goal for this session is to inspire you to use website activity data in more creative and meaningful ways - your examples suggest you're already on the way. 

There _is_ a place for reporting a single statistic like this total in the Senate Report...

---

<!-- .slide: data-background-image="media/overview_report.png" -->

notes: ...but I want us to engage with the more detailed data beneath this statistic, such as the breakdowns available in the Tableau report shown here. You can see at a glance that we can explore other dimensions of the data, including levels of engagement, where users come from, and what kind of devices they use. Let's build our way to this more sophisticated report by starting at the beginning...

---

<!-- .slide: data-background="steelblue" data-transition="none-in fade-out" -->

## What is Google Analytics?

notes: What is Google Analytics?

---

<!-- .slide: data-background="seashell" data-transition="fade-in slide-out" -->

Google Analytics (GA) is a web-based service that collects data about website activity 


notes: Google Analytics, also referred to by the acronym GA, is a web-based service that collects data about website activity. 

You don't need to know a lot about Google Analytics to use the data it collects, but it's helpful to understand what's happening when we say that GA "collects data about website activity"

---

<!-- .slide: data-background="lightblue" --> 

## What does GA collect?

notes: First of all, what does GA actually collect? As you visit a website, scroll down a page, click on a link, your activity is tracked and saved as a series of "dimensions" and "metrics" linked to that website visit. 

---

<!-- .slide: data-background="seashell" data-transition="slide-in zoom-out" -->

**Dimensions** provide context <span style="color:darkgreen; font-style:italic"><br/>which web pages? what browser?<br/><br/></span> <!-- ..element: class="fragment" -->
**Metrics** are quantitative measurements <span style="color:darkgreen; font-style:italic"><br/>how many pageviews? how many sessions?</span> <!-- .element: class="fragment" -->


notes: **Dimensions** provide context for the activity that's tracked. What web pages did you viewed? What browser or operating system did you use? Did you get to the site by following a link? If so, from where? 

**Metrics** are quantitative measurements - or to put it another way, things you can count or calculate. For example, how many times was a particular page viewed? How many sessions were there? And what _percentage_ of those sessions was actually engaged. 


---

<!-- .slide: style="font-size:0.6em; color:dimgray" data-transition="zoom-in fade-out" -->


| Dimension | Description |
| --- | --- | 
| Browser | _The browser used to view your website_    |
| Country | _The country from which the user activity originated_ | 
| Device category | _The type of device: desktop, tablet, or mobile_ |   
| Page location | _The full URL of web pages visited_ | 
| Session source | _The source from which traffic originated for a new session (e.g. google)_ | 
| Year month | _The year and month of the website activity_ | 

<https://confluence.it.ubc.ca/display/ASMNT/About+Google+Analytics+data> 

notes: Google Analytics collects literally hundreds of dimensions and metrics. This table shows just a few dimensions that are commonly used, all of which are readily available in Tableau. You might already see how combining these dimensions can provide a more nuanced picture of our users. It's possible, for example, to identify the subset of users who visited the website using mobile devices during a particular month...  

---

<!-- .slide: style="font-size:0.6em; color:dimgray" data-transition="fade" -->


| Metric | Description |
| --- | --- | 
| Session  | _Period of time during which a user interacts with the website or app_ | 
| Engaged sessions | _The number of sessions that lasted longer than 10 seconds, or had 2 or more screen views_ |
| Engagement rate | _The percentage of engaged sessions (engaged sessions divided by sessions)_ | 
| Event count | _The number of times an event is triggered on a website or app_ |
| Views | _Total number of app screens and/or web pages user saw_ | 

<https://confluence.it.ubc.ca/display/ASMNT/About+Google+Analytics+data> 

notes: ...and then check the metrics associated with that population. Was their engagement rate different than other groups? What pages or parts of the website receive the greatest number of views? Again, this table is only a small sample of the _metrics_ available in Google Analytics. 

---

<!-- .slide: data-background="seashell" data-transition="none-in slide-out" -->

Combine dimensions and metrics with insight and curiosity... 

...for a more meaningful representation of website activity <!-- .element class="fragment" -->


notes: My challenge to you is this: to combine dimensions with insight and curiosity... 

|| to produce a more meaningful representation of UBC Library's website activity.  

---

<!-- .slide: data-background="lightblue"  -->

## How does GA collect the data?

notes: In Confluence and on the Google Analytics help pages there are definitions of dimensions and metrics, but it's easier to interpret them if we understand **how** they're gathered. How **does** Google Analytics collect the data?

---

<!-- .slide: data-background="seashell" data-transition="slide-in zoom-out" -->
 
<span>A <b>property</b> is a website, group of web pages, or app</span>

<span>Every property has a unique <b>tracking ID</b></span> <!-- .element: class="fragment" -->

<span>The tracking ID is added to <b>all pages in the property</b></span> <!-- .element: class="fragment" --> 

<span style="font-size:smaller;color:dimgray;font-style:italic"><br/>A web page can be in more than one property</span> <!-- .element: class="fragment" --> 

notes: An important concept is what GA calls a **property**, which is a website, group of pages, or even an app for which data is tracked.

|| Every property is given a unique tracking ID...

|| ...and this tracking ID is added to all the pages in the property - more precisely, it's added to the HTML of each of the pages. There's one more important thing to understand here: 

|| Just as I live in BC and Vancouver at the same time, the same web page can be in more than one property. Let's look at an example. 

---

<!-- .slide: data-background-image="media/oc_homepage.png" style="font-size:0.7em" data-transition="zoom-in none-out" -->


<div style="background-color:white; height:20%;padding:7%">
<h4>Tracking ID for UBC Library website</h4>
<h3>G-CH28RE4DNT</h3>
</div> <!-- .element: class="fragment"  -->


```html [2,8] 
<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-CH28RE4DNT"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'G-CH28RE4DNT');
</script>
```
<!-- .element: class="fragment" -->


<div style="background-color:white;color:dimgray;height:10%;padding:3%">
Plus a separate tracking ID for the <em>Open Collections</em> property</div> <!-- .element: class="fragment"  -->

notes: Here's a screenshot of the Open Collections home page. 

|| It's part of the UBC Library website, which has the tracking ID shown. In order for Google Analytics to track website activity, all pages in the UBC Library website need to have...

...a chunk of code like this. Notice the UBC Library tracking ID in the highlighted lines of code. 

|| There is also a separate property just for Open Collections...
and this has its own tracking ID. If you were too look closely at the HTML of Open Collections pages you'd find both of these tracking IDs.

---

<!-- .slide: data-background="seashell" data-transition="none" -->

When users load a page, the tracking code sends website activity data to Google Analytics and links it to the relevant properties

notes: when users load a page, the tracking code sends website activity to Google Analtyics. This activity gets linked to the properties that correspond to the tracking IDs, and it gets stored as dimensions and metrics that reflect the user's activity.

Take a beat to close section.

I'd like to pause for a moment - does anyone have questions or comments?


---

<!-- .slide: data-background="steelblue" data-transition="none-in slide-out" -->

## Google Analytics at UBC Library 


notes: How is Google Analytics set up at UBC Library? In the next slides I'll answer three questions about UBC Library's implementation of Google Analytics:

- Who is involved?
- What websites are covered? and
- How do we handle the data?


---

<!-- .slide: data-background="lightblue" -->

## Who is involved?

notes: first, who's involved in setting up Google Anaytics, making sure it's configured appropriately, and making the data accessible? 

---

<!-- .slide: data-background="seashell" -->

### Shared responsibilities

- Library Data Team <span style="color:darkgreen;font-style:italic">data access</span> <!-- .element: class="fragment" -->
- TDUX <span style="color:darkgreen;font-style:italic">service owner, strategy</span> <!-- .element: class="fragment" -->
- Library IT <span style="color:darkgreen;font-style:italic">implement/configure</span> <!-- .element: class="fragment" --> 


notes: it's a team effort with most of the responsibility split between the Library Data Team, TDUX, and Library IT. 

|| The Library Data Team connects library employees with the website activity data they need for planning, decisions, and reports. It's role is to make Google Analytics data accessible.
TDUX

|| TDUX is the service owner for website activity data. It articulates the Library's data collection strategy, which includes deciding what website activity data should be collected to meet our needs.

|| Library IT implements and configures Google Analytics, and it uses analytics data to inform its own projects and decision-making.

It's usually Library IT that makes sure the right Google Analytics tracking codes are added to the right page.


---

<!-- .slide: data-background="lightblue" -->
## What websites are covered?

notes:  what websites are covered? Our Google Analtyics implementation strives to collect data for all public facing web pages.   

---

<!-- .slide: data-background="seashell" data-transition="slide-in zoom-out" -->

A **property** is a website, group of web pages, or app

UBC Library collects data for dozens of properties <!-- .element: class="fragment" -->


notes: These are grouped into Google Analytics properties, where a **property** is a website, group of web pages, or app for which website activity data is collected. 

|| Thanks to Library IT's work we have data for dozens of properties - one that provides an overview of _nearly the entire site_ (excluding UBC Okanagan), and many others for subsets of the website, like a branch website. Let's use one of the branch websites as an example. 

---

<!-- .slide: data-background-image="media/woodward.png" -->

<div style="background-color:white; height:20%;padding:7%; color:dimgray">
<h4>Part of broader <em>UBC Library</em> property</h4>
<em>and</em>
<h4>has its own <em>Woodward Library</em> property</h4>
</div> <!-- .element: class="fragment"  -->

notes: Here's the Woodward Library branch page. It's part of the UBC Library property...

|| ...but in some contexts it can be treated as its own website. When a user visits this Woodward home page their activity is recorded in both properties. 


The full list of GA properties that the Library Data Team provides access to appears in drop-down filters in the Tableau reports. 

A note about UBC Okanagan data: Because Google Analtyics was handled differently at each UBC campus, UBCO Okanagan website activity is not currently included in the main UBC Library website property. However, it _is_ available as a separate property.  If you have quesitons or if you can't find the website or pages you're interested in, please contact the Library Data Team.

---

<!-- .slide: data-background="lightblue" data-transition="slide-in none-out" -->

## How do we manage the data? 

notes: Google collects the data, but there's some work involved to get it to you in a format that's easy to access and up to date. How _do_ we manage the data?

---

<!-- .slide: data-transition="none" -->
![GA data flow](media/data_flow_1.png)

notes: This is a simplified representation of how the data gets from Google to you. The starting point is the Google Analytics Server where all the data is first collected.

---

<!-- .slide: data-transition="none-in zoom-out" -->
![GA data flow](media/data_flow_2.png)

notes: at the end of every month the Library Data Team takes snapshots of the month's website activity and stores them in TSV files on the T: drive. This happens automatically with Python scripts that harvest selected dimensions and metrics using the Google Analytics API. We don't harvest all the data, but enough to answer many website activity questions.  

---

<!-- .slide: data-transition="zoom-in fade-out" data-background-image="media/tsv_view.png" -->

![GA data flow](media/file_hierarchy.png)

notes: These TSV files are stored in a T: drive directory that's visible to everyone. Some of the files are large (the pages file has more than 3M rows) and won't open in software like Excel, but they're available to anyone who wants to analyze the data themselves. 


---

<!-- .slide: data-transition="fade-in zoom-out" -->
![GA data flow](media/data_flow_3.png)

notes: Most of us will prefer to move along to step three in the diagram, where these TSV files are turned into Tableau reports that are updated every month.

---

<!-- .slide: data-background-image="media/overview_report.png" data-transition="zoom-in none-out" -->

notes: here's an example of one of the Tableau dashboards. This one shows an overview of activity for the entire Library website from July 2023 to May 2024. Across the top you can filter by dimensions including the date, session source, device category, and medium. Even at a glance you can see that the overview graphs reflect the academic schedule, with a decrease in activity during the summer months and over the winter break.

|| Pause for end of section.

|| I'd like to pause again for questions before we move to the final section. Are there any questions about UBC Library's implementation of Google Analytics?

Now we'll move on to the last section...

---

<!-- .slide: data-background="steelblue" data-transition="none"-->

## Find and use website activity data 

notes: Where can you find website activity data to use in reports, for planning, or for decision making? 

---

<!-- .slide: data-background="seashell" data-transition="none-in slide-out" -->

There are several paths

1. Use Google Analytics reports on Tableau <!-- .element: class="fragment" style="color:darkgreen" -->
2. Request a custom report <!-- .element: class="fragment" style="color:darkgreen" -->
3. Access the Google Analytics interface <!-- .element: class="fragment" style="color:darkgreen" -->


notes: There are several paths and you might need more than one depending on your project. You can:

|| Use Google Analyics reports on Tableau...
|| Request a custom report...
|| or Access data directly using the Google Analytics interface.

---

<!-- .slide: data-background="lightblue" -->

## Use Google Analytics reports on Tableau

notes: the most appropriate path will depend on your project, but if you're not sure: start with the Google Analytics reports on Tableau.

---

<!-- .slide: data-background="seashell" -->

Designed to answer frequently asked questions


<ul style="color:darkgreen; font-style:italic">
<ul>
<li>where are visitors coming from?</li>
<li>what pages were viewed, and how often?</li> 
<li>what do people search for?</li>
</ul> <!-- .element: class="fragment" -->

notes: These reports are designed to answer frequently asked questions... 

|| ...like where visitors come from, what pages they view, and what search terms they use

---

<!-- .slide: data-background="seashell" data-transition="slide-in fade-out -->
### Links to reports on Tableau

- [Library website activity](https://reports.im.it.ubc.ca/#/site/Library/workbooks/6294/views) for current data
- [Library website activity - historical](https://reports.im.it.ubc.ca/#/site/Library/workbooks/6137/views) before 2023-07

notes: The two repors shown here are a good starting point. They have similar content but cover different time periods.

In 2023 Google Analytics underwent a major change, upgrading from a platform called _Universal Analytics_ to _Google Analytics 4_. This included changes to many dimensions and metrics, so it's important to use caution when comparing website activity from before and after July 2023. We've documented some of the differences on the Google Analytics pages in Confluence. If you have questions about comparing data over the long term, please consult these pages or contact the Library Data Team.

For many applications it's enough to use data from July 2023 onward, so in this presentation we'll focus on the current report.      

---

_Live demonstration of current website activity report_

notes: Load the report, step through each of the sheets in order, find a question for each

- About this report
- Overview
	- For the main UBC Library property, this is the only place to get the big picture for the entire UBCV Library website (but excludes UBCO).
	- Filter to 2024, exclude may (Winter term 2)
	- Show summary
	- Change to sessions
	- Notice that engagement rate is 56%, and that 5% of sessions are from US visitors
	- Limit to non-UBC LigGuides source
	- This subset of the activity is different. Engagement rate is higher (62% instead of 56) and the percentage and US visitors account for 21% of views, not 5%. We'd have to investigate more closely to know for sure, but this is likely because of LibGuides at US institutions linked UBC Library web pages.
- Searches
	- When a URL includes a search term - like what you see in the URL of search results pages - Google Analtyics records the term and counts the 'search' event. 
	- We can limit to searches run on just part of the Library site, identified by a hostname. The top line here represents searches at resources.library.ubc.ca. Filter to resource page searches.
	- expand the list of search terms to show grouping
	- search for 'date' to show 'uptodate', an indication that users are looking for a point-of-care medicine platform we don't have. It doesn't mean we should buy it, but perhaps there's a way to redirect these users to DynaMed, a similar platform that we _do_ subscribe to.
	- Remove 'date' search term
- Search terms
	- switch to cloud
	- this is another view of the research guides search terms
	- note that there's a filter for average searches per month to prevent the display from getting too cluttered with lesser-run searches. You might need to adjust this depending on other filter settings.
- Sessions
	- switch to Sessions tab. This dashboard (and many of the others) provides a more detailed look at other smaller properties. 
	- the date filter applies to the entire report, so this is pre-filtered to show Jan-April 2024. 
	- show the property name filter. Here you can choose the website you want to view. Change it to Asian Library. Again not surprisingly, the Asian Library has a higher percentage of international visits. On the UBC Library website overall, 82% of sessions are from users in Canada, but that's only 70% for the Asian Library website. 
	- Other graphs on this website are familiar from the overview tab 
- Page views
	- when branches are reviewing their websites they sometimes want to know which pages get the most traffic, or how much activity is associated with certain pages. The Page views tab can answer these questions.
	- Switch to techserv.library.ubc.ca
- 404 Page
	- Not a web crawler, but can help spot when users are repeatedly pointed to page that appears to be on a UBC site, but doesn't exist - or doesn't exist anymore.
- Properties and Pages
	- An administrative page that lists all the properties in the report along with counts of visited pages in each domain


---

<!-- .slide: data-background="lightblue" -->

## Request a custom report 

Notes: there are many things we can learn from the Tableau report, but it won't always answer our questions about website activity data. 

---

Needs not met by Tableau reports? Submit a request using the [Library Data Team contact form](https://helpdesk.library.ubc.ca/request-for-library-datareporting-services/)

<https://helpdesk.library.ubc.ca/request-for-library-datareporting-services/> <!-- .element: class="small" -->

Notes: If you need metrics or dimensions that aren't in the report, or combinations of dimensions that the report doesn't provide, submit a request to the Library Data Team. We can't guarantee that we can provide the data you're looking for, but we'll do our best to idenify what's available and package it for your needs.


---

<!-- .slide: data-background="lightblue" -->

## Access the Google Analytics interface


notes: A third way to get Google Analytics data is to access the GA interface directly.

---

<!-- .slide: data-background="seashell" -->

**Advantage:** access all the data collected by Google Analytics (not just the subset in Tableau)

**Disadvantage:** must learn to use and interpret the Google Analytics web interface

notes: This involves more setup and is probably most suitable for people whose job requires them to work directly with Google Analytics. It can be helpful because it provides access to all the data collected by Google Analytics, not just the subset that is included in Tableau reports. 

The main disadvantage is that you need to learn to use and interpret the Google Analtyics web interface - this level of engagement involves more commitment.


---

<!-- .slide: data-background="seashell" -->
### To request direct access to GA

1. Create a Google account linked to your _ubc.ca_ email
2. Request GA access using the [TDUX contact form](https://helpdesk.library.ubc.ca/litmu/request-form/)

notes: if you would like to request direct access to GA, you'll need to have a Google account that's linked to your ubc.ca email address. The next step is to request access using the TDUX contact form.

---

<!-- .slide: data-background="lightblue"  -->

### Additional resources in Confluence
<https://confluence.it.ubc.ca/display/ASMNT/Google+Analytics>

notes: For further help accessing and using Google Analytics data, please consult the Google Analytics pages in Confluence or contact the Library Data Team.

Pause for recording end

Ask Questions about third part

---

<!-- .slide: data-background="darkseagreen" data-transition="none" -->

# Thank you
