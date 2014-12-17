This is the web application like Quora and StackOverflow for users to Ask question and get Answer
---

####[Ask&Answer System URL](http://tobetaoblog.appspot.com/)
This web application is built by with Google App Engine Cloud Platform ([ref](https://cloud.google.com/appengine/docs)) and deployed on Google App Engine. 
Jinjia is the template used ([ref](https://cloud.google.com/appengine/docs/python/gettingstartedpython27/templates)).

The program is designed to include following highlight features:

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
* **User friendly page style** - The whole page is desinged to be user friendly which includes soft color, natural button and comfortable webframe. 

Additional features with search and sort are under development.

Design
---
Files Description
	
* AccessDB.py: `undergoing features to store NLP database`

* helpers.py: `draft`

* settings.py: `Jinjia draft`

* main.py: `python file that contains all functional classes to implement Ask&Answer features`

* addquestion.html: `Define the show page when user click to add a question`

* ansewr_template.html: `Define the framework of answer.`

* app.yaml: `Necessary file with Google App Engine.`

* bootstrap_base.html: `Outer frame or the website`

* creaetanswer_image.html: `the page when user click to add answer.`

* questionpage.html: `the page when user in the view question page`

* sideRss: `RSS for each question`

Code Description

* class Question: `main handler for ask question`

* class QuestionPage: `function to support view question`

* class QuestionSave: `Question database`

* class editQuestion: `Support edit function to question`

* class QuestionVote: `database of question votes`

* class VoteQuestion: `support vote function to question`

* class Answer: `main handler for answer`

* class AnswerVote: `database of answer votes`

* class VoteAnswer: `support vote function to answer`

* class editAnswer: `Support edit function to answer`

* class AnswerSave: `answer database`

* class Image: `handler of image`

* class AnswerImage: `handler of image in answer page`

* class NewAnwer_iamge: `handler of image in add answer page`

* class RelativeTime: `show current time`

* class questionRSS: `RSS for each question`

Compile instruction:
---
* This web application is build with Google App Engine, the installation instruction is as following
	- Install Google App Engine ([ref](https://cloud.google.com/appengine/downloads))
	- Download my whole project from Github ([ref](https://github.com/tobetao/AskAnswer))
	- Run and Deploy using Google App Engine Launcher
	- Free Google App Engine account could be registered here ([ref](https://appengine.google.com/))

Undergoing development:
---
* Support a superuser that can remove question or answer.
* Keep track of views and give viewers access to these stats.
* Integration with a web service to translate pages to other languages, post to facebook/twitter/G+, display ads, etc.
* Support emailing updates, where any answer posted will get sent to the person asking the question (see ([Document](https://cloud.google.com/appengine/docs/python/mail/receivingmail))
* Allow viewers to search for questions or answers by text in the contents.
* Allow users the ability to follow a question, and create a view page that shows all of the followed questions.
* Allow "smarter" sorting of questions, that uses a combination of activity (number of answers or votes) and time to better rank the questions.
