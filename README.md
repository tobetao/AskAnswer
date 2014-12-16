This is the web application like Quora and StackOverflow for users to Ask question and get Answer
---

####[Ask&Answer System URL](http://tobetaoblog.appspot.com/)
This web application is built by with Google App Engine Cloud Platform ([ref](https://cloud.google.com/appengine/docs)) and deployed on Google App Engine. 
Jinjia is the template used ([ref](https://cloud.google.com/appengine/docs/python/gettingstartedpython27/templates)).

Highlight features includes:

* **default page with login** - Users could see all questions and answers without login.
* **multiple users** - The system handles multiple users and each user is able to create/edit one or more question/answer owned by the user once login .
* **tags** - Users could define tags. Each post might has a number of tags and click a tag can view all posts marked by that tag. 
* **Designed feature** - Each page shows up to 10 post with next page or previous page button available. JavaScript and page features could be referenced to Bootstrap ([ref](http://bootstrapzero.com/)) and StackOverflow ([ref](http://bootstrapzero.com/))
* **uploads** - user can upload images locally both in add question page or add answer page. Answer could also be added in view question page without upload iamge feature.
* **RSS** - each question has RSS link, that dumps a entire blog in XML format.
* **votes** - A logged in user could vote up or down on any question/answer. 
* **timestamp** - Questions and answers are stored along with a timestamp created or modified. 
* **contents limits** - each question will display content capped at 500 characters. Upload image could not exceed limit size. 
* **Branch** - program is develped using GIT and branch with RSS function turned down is open source in GitHub https://github.com/tobetao/AskAnswer/branches.

Additional features with search and sort are under development.

Design
---
Files Description
	
* main.py: `python file that contains all functional classes to implement Ask&Answer features`

* addquestion.html: `Define the show page when user click to add a question`

* ansewr_template.html: `Define the framework of answer.`

* app.yaml: `Necessary file with Google App Engine.`

* bootstrap_base.html: `Outer frame or the website`

* creaetanswer_image.html: `the page when user click to add answer.`

* questionpage.html: `the page when user in the view question page`

* sideRss: `RSS for each question`


Undergoing development:
---
* Support a superuser that can remove question or answer.
* Keep track of views and give viewers access to these stats.
* Integration with a web service to translate pages to other languages, post to facebook/twitter/G+, display ads, etc.
* Support emailing updates, where any answer posted will get sent to the person asking the question (see ([Document](https://cloud.google.com/appengine/docs/python/mail/receivingmail))
* Allow viewers to search for questions or answers by text in the contents.
* Allow users the ability to follow a question, and create a view page that shows all of the followed questions.
* Allow "smarter" sorting of questions, that uses a combination of activity (number of answers or votes) and time to better rank the questions.
