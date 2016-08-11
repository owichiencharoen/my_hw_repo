# Project Design Writeup and Approval Template

Follow this as a guide to completing the project design writeup. The questions for each section are merely there to suggest what the baseline should cover; be sure to use detail as it will make the project much easier to approach as the class moves on.

### Project Problem and Hypothesis

* What's the project about? What problem are you solving?

I am trying to predict mobile users' demographic characteristics, which is provided as a depedent variable named "group" (presumably it's an encoded variable mappable to age, gender), so that the company can serve better, more targeted, more relevant advertisements to them.

* Where does this seem to reside as a machine learning problem? Are you predicting some continuous number, or predicting a binary value?

It's a classification problem. My model will be trained on various inputs including categorical features (such as phone brand), and continuous numerical features (such as duration of engagement). There will also be time series (datetime).

* What kind of impact do you think it could have?

I think the impact will be significant to any business that wants to serve relevant advertisements.

* What do you think will have the most impact in predicting the value you are interested in solving for?




### Datasets

* Description of data set available, at the field level (see table)

Data comes in six relational tables, star schema, in csv format. Each branch table is linked to the main table by unique keys. This data is provided by kaggle.
 

* If from an API, include a sample return (this is usually included in API documentation!) (if doing this in markdown, use the javacription code tag)




### Domain knowledge
* What experience do you already have around this area?

I work in media, so I understand the importance of serving advertisements that are relevant to the target audience.

* Does it relate or help inform the project in any way?

Not really, because machine learning model only focuses on predicting/classifying the data. It doesn't care about the business or the industry.

* What other research efforts exist?

There is a very active community on kaggle that discusses, shares info, and tries to solve this problem.


### Project Concerns

* What questions do you have about your project? What are you not sure you quite yet understand? (The more honest you are about this, the easier your instructors can help).

I want to know how to deal with time series. I want sklearn to handle string categorical features, but it doesn't. I will have to do get-dummies and end up with a very large, very sparse matrix.

* What are the assumptions and caveats to the problem?
    * What data do you not have access to but wish you had?

It would be nice to have more predictors than the ones given in this kaggle competition. For example, if we could know a bit more about the users, such as income, profession, etc.
    
    * What is already implied about the observations in your data set? For example, if your primary data set is twitter data, it may not be representative of the whole sample (say, predicting who would win an election)

This data may not be representative of the whole country of China.  We won't know if this sample was fairly selected to represent the entire population.
    
* What are the risks to the project?
    * What's the cost of your model being wrong? (What's the benefit of your model being right?)
    
The cost of the model being wrong is that we serve a poor advertisement with no effect on the target user.  So the cost is the opportunity cost.
    
    * Is any of the data incorrect? Could it be incorrect?

the demographic characteristics (dependent variable 'group') in the training set could be incorrect.  It probably came from a market research firm.


### Outcomes
* What do you expect the output to look like?

I expect the output to be a classification results for each row.

* What does your target audience expect the output to look like?

It's a kaggle competition, so the expectation is quite clear and it's aligned with mine.

* What gain do you expect from your most important feature on its own?

Not sure.

* How complicated does your model have to be?

I have no preference, as long as it isn't overfitted to the training set and it does a good prediction job on the unseen (test) data.  It doesn't need to be interpretable, so if it's very complicated but it performs better I will use it.

* How successful does your project have to be in order to be considered a "success"?

I want my accuracy to be within 3% of the kaggle winner.  If I can get that close, I'll be very happy and consider it a success.

* What will you do if the project is a bust (this happens! but it shouldn't here)?

There is no contigency plan! I must not fail!

