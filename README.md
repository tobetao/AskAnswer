This is the final project of OST 2014 implemented in Python
---

####[blog System URL](http://lx350-final.appspot.com/)
This blog system is built by Jinjia, Google App Engine and Bootstrap, and is deployed on Google App Engine. 

All required features are implemented. Plus, I implement "smarter" sorting of questions, that users could use to sort by "create time", "modified time", "votes" and "answers".

* **multiple users** - The system handles multiple users and each user is able to create one or more question/answer. A user can select and edit the question/answer posted by the user.
* **tags** - Users could define tags. Each post might has a number of tags and click a tag can view all posts marked by that tag. 
* **pagenation** - every page has 'next' and 'previous' links to other pages, and each page has no more than 10 posts. 
* **uploads** - user can upload images locally and image with an URL could be shown inline.
* **RSS** - each question has RSS link, that dumps a entire blog in XML format.
* **votes** - A logged in user could vote up or down. User without login could just view question/answer but not vote. 
* **timestamp** - Questions and answers are stored along with a timestamp hen created or modified. 
* **default view** - each question will display content capped at 500 characters. 
* **RSS** - each question will display a RSS link.
* **Branch** - program is develped using GIT and branch with RSS function turned down is open source in GitHub https://github.com/liangxiang/OST_Project.


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