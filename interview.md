# Basic interview questions

* Describe a data-related project you completed, and what you learned from the project.
	* Be ready to talk about a couple of projects that you think really show off your contributions, engineering and modeling skills, and teamwork.
	* What was the goal of the project?
	* What were your specific duties and responsibilities? Who else was involved? Were you happy with the outcome of the project?
	* How did you keep track of progress? How did you estimate milestones and deadlines? How did review status against them?
	* You should be able to give a  high-level explanation of your work in the form of a “story”. You should explain why you worked on a project, what you were trying to accomplish, what your contributions were, what were some of the challenges and how you solved them (these should also include “soft” challenges — e.g. the team didn’t have a process for coordinating and sharing results, and you instituted one). The goal is to help the interviewer immediately understand, as an outsider, that your skills will generalize to a different field and environment. 
	* You can deep-dive into the more technical details later if the interviewer is interested.
	* What would you have done differently? Be prepared to describe a difficult/unsuccessful situation.
* Do you see yourself as a data scientist, and why?
	* Yes! Use examples from your past work, making sure to translate the astronomy jargon into high-level terms.
* You are given a spreadsheet that includes data about an internet company (e.g. number of users, time spent on the platform, and sharing activity) and their monthly revenue. This dataset fits into memory. What is your process for analyzing this data?
	* Most people will jump into talking about regression methods, importing the data into scikit-learn, etc. _Don't do that right away._
	* As a mature data scientist, the correct way to answer this is to detail what process you would follow in real life. You would not jump straight into analysis, but you would /you would ask more questions before jumping into the analysis/, including:
		* Who is the audience? 
		* What business problem are they interested in solving? What business metrics are we optimizing for?
		* How do you ensure correct communication and translation of jargon between stakeholders? What is considered a "user" (all users, including inactive? only active users? only paying users?). What is considered "time spent on the platform"? etc. Nailing down and defining these is one of the most difficult parts of the process in practice.
		* What is the /current process/ that's already in place? How are we trying to improve it?
		* Are they trying to explain what drives sales, or forecast future sales? Does the model need to be explainable to stakeholders?
		* What data is included? Where is the data coming from?
		* etc
	* 	Once you transition into talking about the analysis, you should be able to:
		* identify if this is a classification, regression, or outlier/anomaly detection problem
		* identify immediately what is the response variable based on your earlier questions (e.g., sales in this case) and what the relevant predictors are.
		* start the discussion with the simplest possible modeling techniques. Simple, explainable, understandable models should be preferred over more complex models, unless there are performance goals that cannot be achieved by the simpler model. Linear and logistic regression can go a long way, and in practice, it is the production model for a lot of problems. 
		* describe your analysis workflow — typically asking stakeholders and domain experts about goals, requirements and constraints for the model; running an EDA (exploratory data analysis) to help you understand the data and correlations between the different variables; thinking about a choice of model family; coming up with a few simple features (predictors); separating the dataset into train / validation / test sets; training models;  computing test metrics and understand model outputs (what are regions of the feature space where the model works well or not so well?), then translation into business metrics.
		* describe how you would explain the output of your model to your audience
* How much machine learning work have you done?
	* You probably have done ML-adjacent work in astronomy, you just called it something different.
	* If you really, really haven’t done an ML project in astronomy, be prepared to describe previous projects that could have been concretely improved with machine learning
* What is in your current data science toolbox?
	* Start from the prototyping basics (say, Python / Jupyter / Pandas / Sklearn, or R), then move on to other tools you are proficient with.
* How is data used in Astronomy?
	* Again, think at a high level. Examples: where is the data you used in your research coming from? How did you reduce it? What models did you use? What was your analysis process? How did you ensure reproducibility? How did you share your results with the rest of your team?
* What is something you would like to learn (e.g. algorithm, technique, stack, etc.) while at X?
* Why are you interested in Y? (where Y is the core business of the company/the mission of the data science team you’re applying for)
	* A lot of people are surprisingly unprepared to answer this
* Some soft questions include:
	* Tell me about a challenge or conflict you have experienced at work
	* What makes you uncomfortable?
	* What are some of your leadership experiences?
	* Why are you leaving your field?
	* Tell me about a time you made a mistake at work.
	* For a past project, how did you decide what would make that project successful?
* Be prepared to answer very simple stats problems.
	* Usually, those include questions that are slightly tricky on the surface but can be answered easily by invoking some form of Bayes’ theorem. 
* Simple questions about basic ML algorithms and techniques, for example:
	* Can you give a *basic* explanation of how (linear regression, logistic regression, classification trees, random forests, K-means clustering, neural networks) work?
		* Think about an example problem where that algorithm is applicable
		* What are some of the strengths of the algorithm? What are some of its limitations? (being able to answer this question is _much more important_ than knowing all the implementation details of the algorithm. Neural networks are not the magic answer to everything.)
	* What is the gradient descent method?
	* What is regularization? When is it useful?
	* What is multicollinearity? How can we solve it?
	* What is the curse of dimensionality? When would you suffer its effects? How can you compensate for it?
* Simple questions about data:
	* What are ways you could deal with missing data?
	* How can you determine if a data set is “clean”?
	* What are some ways you can deal with messy data?
	* What is big data? Would you consider the projects you worked on “big data”? How do you deal with it?
* Be prepared to describe or whiteboard some simple setups that involve writing SQL queries on data
	* For a data science interview, these are typically very basic SQL queries that include aggregations and joins
