
Community Pages - Structure 
===========================


Motivation
----------

We need a new set of community pages to replace the [Pentaho community
pages](http://community.pentaho.com). It has to be the main go-to point for
community people.


It's made of a generic _"umbrella"_ for the community pages, but each
individual project needs to have it's own identity, it's own independence. 


We need to make this somehow hierarquical. We can have subprojects inside
projects (eg: some kettle plugin that wants to have it's own project page)


Communication Style
-------------------

The goal is to have something that is aimed for the technical people. Something
that complements the main [Pentaho website](http://www.pentaho.com) image, but
for a different audience. The ultimate goal is to get the buy-in from CTO's on
this community side, and redirect CEO's / CFO's to the _pentaho.com_ website.



Website / Professional documentation
-------------------------------------

We need a strategy for differentiating between this community websites and
Pentaho's professional documentation strategy, led by Paula Toth. 

The proposal here is that most sections of the _sitemap_ stays outside the
documentation group. Only the specific _documentation_ sections (as simple or
complex as they can be) will live in the same platform as the rest of the
professional documentation.

Pentaho's currently evaluating what platform to choose for the professional
documentation part. In order for that not to be a blocker to this project, I
propose 2 stages.

An added bonus would be to be able to design the architecture of the site with
complementary titles and taxonomy to support both the Community and the
InfoCenter. We can change either the InfoCenter or the Community as needed.  


### Phase 1: Extract

We should have documentation available on the website since day one. We should
look into where the documentation lives and either import it or just create it
in the same way as the rest of the platform. Whatever works.


### Phase 2: Embed

Once the documentation group moves forward with the project, we'd insert all
existing documentation into the chosen platform and link / embed the pages from
that documentaion platform into the websites



Main Community Page
-------------------


Here are the relevant sections for the main community site

* About
* Engage
	* Forums
	* IRC
	* Mailing lists
	* Bug Tracking
	* Get the source
	* CI
	* Blogs
* List of projects
* News
* Blog posts (blend with _News_?)
* Events
* Training
* Support
* Contact us
* Upgrade to EE (blend with _Support_?)


News and blogs can simply be a feed of all the subprojects' news and blogs.
Events and training can also be gathered from the subprojects' events (but not
only, eg: the Pentaho European Meeting is something that is not related with a
single project only but to the whole community page)


Projects
--------


Each project page will contain detailed and contained information about the
project. Can be a major project like kettle or mondrian or simply a small
project like _CST_


Here's a possible project hierarchy:

* Community Pages
	* BI Server
	* Mondrian
	* Kettle
		* Kettle CMIS input plugin page
		* Other kettle plugins that may have it's own page
	* Reporting
	* Weka
	* Ctools
		* CDE
		* CDA
		* CDF
	* Sparkl
	* Community Webpages (this)
	* _etc_



Project structure
-----------------


Here's the project structure. We probably can / should group with in a better
navigation structure

* About
* Examples / Screenshots
* Documentation (Link with Paula Toth's work)
* FAQ (Under documentation?)
* Get the source
* Getting started
	* How to use the binaries
	* How to compile the project
	* How to debug the code
* Download
* News
* Changelog
* Blog (Blend this 3?)
* Engage
	* Forums
	* IRC
	* Mailing List
	* Bug tracking
	* CI
	* Community Blogs
* API / jsdocs
* Credits / Contributors
* Events
* Support (people may want to have it's individual support pages)



General considerations
----------------------

This entire structure will be hosted on a single jekyll structure on github. We
could think about separating this into individual submodules, but it's probably
overkill and we could easily go into dependency hell. This is an open issue
though, as I'm not absolutely convinced about it. 


Implementation steps
--------------------

1. Pedro to come up with general sitemap structure
2. Nuno / UX team to come up with UI proposal
3. Pedro / Miguel / Gonçalo to implement the structure in Jekyll
4. Implement community page
5. Implement individual projects
6. Get existing documentation inserted here somehow
7. Implement some deploy mechanism
8. As soon as Paula's ready, integrate/ embed the documentation source
9. Contact project owners (Matt / Thomas / Mark / Julian) and get their
   involvement for the updates
10. Contact external entities to see if they want to have their own pages


Timeframe
---------

The usual: *ASAP*
