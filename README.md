This is the web application like Quora and StackOverflow for users to Ask question and get Answer
---

####[Ask&Answer System URL](http://tobetaoblog.appspot.com/)
This web application is built by with Google App Engine Cloud Platform ([ref](https://cloud.google.com/appengine/docs)) and deployed on Google App Engine. 
Jinjia is the template used ([ref](https://cloud.google.com/appengine/docs/python/gettingstartedpython27/templates)).

Highlight features includes:

* **default page with login** - Users could see all questions and answers without login.
* **multiple users** - The system handles multiple users and each user is able to create/edit one or more question/answer owned by the user once login .
* **tags** - Users could define tags. Each post might has a number of tags and click a tag can view all posts marked by that tag. 
* **Designed feature** - Each page shows up to 10 post with next page or previous page button available. JavaScript and page features could be referenced to Bootstrap ([ref](http://bootstrapzero.com/)) and StackOverflow ([ref](http://bootstrapzero.com/)
* **uploads** - user can upload images locally both in add question page or add answer page. Answer could also be added in view question page without upload iamge feature.
* **RSS** - each question has RSS link, that dumps a entire blog in XML format.
* **votes** - A logged in user could vote up or down on any question/answer. 
* **timestamp** - Questions and answers are stored along with a timestamp created or modified. 
* **contents limits** - each question will display content capped at 500 characters. Upload image could not exceed limit size. 
* **Branch** - program is develped using GIT and branch with RSS function turned down is open source in GitHub https://github.com/liangxiang/OST_Project.

Additional features with search and sort are under development.

Design
---
Classes
	
* Mainpage: `Show the contents of main page`

* ViewQuestion: `Show the contents of question page`

* Question: `The database taht stores all the question.`
			`It also provides render functions that can render the htmls.`
			`The render function also replace the white spaces to <br>`
			`handles the links and image links. `

* QuestionEdit: `This handles the edit page letting user to edit an exiting question.`

* NewQuestion: `add new question`

* QeustionEntry: `Handles the post action that an user submits a edited post.`

* Answer: `The database taht stores all the answers.`
			`It also provides render functions that can render the htmls.`
			`The render function also replace the white spaces to <br>`
			`handles the links and image links. `

* QuestionVote: `database related to vote of question`

* AnswerVote: `database related to vote of answer`

* AnswerEdit: `This handles the edit page letting user to edit an exiting answer.`

* NewAnswer: `add new answer`

* AnswerEntry: `Handles the post action that an user submits a edited answer.`

* VoteQuestion: `support the function to vote question`

* VoteAnswer: `support the function to vote answer`

* EST: `support the time recording`

* Image: `show image`

* AnswerImage: `iamge added in answer post`

* RSS: `The main page has RSS function`

* questionRSS: `Each question has RSS function`


Further posibly improvement:
---
* Delete function is missing, you cannot delete a post or a blog.
* Uploaded images should be managed. You canot delete any uploaded things.