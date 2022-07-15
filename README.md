# wine-quality
this is solution for wine quality prediction by using basic ML Model and LazyPredict
the general data prescription has the different chemical compositions of wine , which effect the wine qualiy
I came up with an approach which can help us understand data by forming our own class label by giving constraints to pH attribute
we are using pH attribute because as manu know pH scale is standardized scale to determine the nature of any chemical compound/mixture or element 
The constraints of the pH are as follows:
if pH is in the range 3.4 to 3.6 --> it is considered to be good wine
if the pH value is less than 3.4 --> it is considered to be moderate wine because of its good color and bitter taste
if the pH is greater than 3.6 --> it is considered to be bad wine 
we label encode the above attribute and obtain the class label 
for proving that this can model is accurate I have also done lazypredict for confirmation.
the datasets we have used are winequality-red.csv,winequality-white.csv


# naive bayesian classification
It is one of the most used ML classification used for probabilistic classification  of the data
One of its demerits are , for naive we shall assume all the features of the data are independent but it is not possible in the case of real world data
we use the accuracy and confusion matrix to present the performance of the bayesian model 
the dataset I have used is playtennis.csv
# Sentimental Analysis using NLP 
In this project our goal is to predict the emotion of the input (text , image or any other form ) 
my database is named as AllProductReviews which basically consists 5 main labels which represent the level of customer satisfaction  about n different products for better presentation I have sliced down the dataset for one of such products, but the tricky point here it doesn't contain any fixed sentiment , so in the code blocks below I have tried to determine the main sentiments through using the column named ReviewStar which is of int data type by using this label I have generated 5 unique sentiments(very bad , bad , average , good ,excellent) and perfomed onehotencoding for the binary transmission of the  sentiments. this is when the nltk and wordcloud packages come to picture, wordcloud helped me to present the top reviews of entire boat headphone reviews later on I have ntlk for processing the reviews and performed the GridSeearch using the random forest classifier. I have extracted the features using the countVectorizer and obtain the output score , accuracy score using the GridSearch with LogisticRegression and also visualize the top 100 words which resultesd in getting each of three sentiments i.e. average , excellent and bad.
