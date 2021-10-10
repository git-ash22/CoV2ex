# Cov2ex

The ongoing pandemic had a lot of impacts on human life. Due to the lockdown in the entire country, people are having more time these days and hence are into social media. Social media has become a platform wherein people share all their thoughts and emotions. Due to the social distancing norms and other preventive measures, people are connecting each other through this platform. This gives us the opportunity to analyse the overall mental reaction of the people to this pandemic. In this paper, we collected data from twitter having state wise tweets related to COVID-19 pandemic and have manually set the emotion conveyed by each tweet in it. This is then used for training the model and we output the average emotion conveyed by each state. This can be useful in understanding the psychological impact the COVID-19 had on the people, state-wise; helping the governments to take necessary actions accordingly. The output as well as COVID-19 guidelines and data are then represented in a website.

#Objective
1. To create a website that gives details about the COVID-19 pandemic in India, such as its data, norms, regulatory actions, psychological support, etc.
2. To collect data from twitter and shown live sentiments in a geographical map representation. Also we displayed the current trending keywords about COVID-19 on the website to give people an idea of the current situation of the pandemic.
3. To create a helpline for people suffering from mental illness owing to the lockdown and COVID related crisis using question analysis.

#Dataset
The Project uses two different datasets. Both datasets serve different functionalities to the CoV2eX Website. 
First dataset is a global twitter dataset that has the tweet as text corresponding to its sentiments. 
 a. This is used in training the model in order to predict the sentiment of a given tweet. 
 b. The dataset consists of 23,242 tweets. 
The second dataset is the one that consists of the regional tweets from India. 
a. This dataset just has the date and time, tweet ID, sentiment score and place; and does not contain the text as such for the evaluation. 
b. The dataset gives the sentiment scores of 12,705 tweets with tweets from around 1,115 unique cities across India. Mumbai and New Delhi top the count with 1,473 and 1,309 tweets respectively.

#Methodology
1. The global data has been analysed and a world cloud has been plotted from it. The 23,242 tweets were converted into a list and were joined into a single sentence.
2. After this, we preprocess the dataset. In order to train the model well, we removed punctuations and stopwords from the dataset.
3. Then, we convert the sentences into a matrix of token count.
4. Then we applied the train test split. The split occurs in the ratio of 80:20 for the train and test respectively.
5. Naive Bayes classifier is implemented to train the model.
6. After training the model, a basic confusion matrix was plotted in order to obtain the complete representation of the classification.
7. After this, the accuracy was noted.
8. The web development part of the project included basic tools such as HTML and CSS.
9. Another phase of the project was the helpline provided by the website. 
    a. This was done using the calculation of a score. 
    b. This score is taken using some questions. 
    c. There were 8 questions asked, this is then scored on a scale of 0 to 10.
    d. The calculated score is then used for classification of the user’s mental state. 
    e. This is then used for displaying relevant contents for each individual. 
    f. This consists of many videos, podcasts, articles related to improving health conditions through meditations and other well-being practices.
    
#Results
1. A website was designed in order to display the primary details of the pandemic and the guidelines that are needed to be followed by the public
2. This website displays the information about the day to day cases of COVID-19 along with other relevant details
3. The website also consists of the state-wise cases represented in a graph
4. The test accuracy of our MultinomialNB model came out to be 81%.
5. Label 2’s classification was most accurate compared to other labels. 
    a. The F1-Score for label 2 was 87% 
    b. It had a precision score of 89% 
    c. It had a recall score of 32%. 
    
#Conclusion
We implemented sentiment analysis using Naive Bayes machine learning algorithm suitable for problems with text classification and multi classifications and also because a Naive Bayes classifier runs fast, since the computations required are simple sums and logarithms. We did sentiment analysis only on tweets amounting below 25,000. Thus, it need not necessarily illustrate the sentiments of the world as a whole. Most of the tweets are more or less neutral while there are more positive tweets than negative tweets. Which means that in general, the people are trying not to be negative despite the difficult times.
