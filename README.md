# Amazon's Cloud Based Multi Criteria Recommender Application


Recommender systems are software applications that attempt to reduce information overload.
Their goal is to recommend items of interest to the end users based on their preferences. To
achieve that, most Recommender Systems exploit the Collaborative Filtering approach. This
report aims to provide an overview of the class of multi-criteria recommender systems. It
defines the recommendation problem as a multi criteria decision making (MCDM) problem.
This project uses Trip Advisor dataset and leverages cloud based Amazon MapReduce
services to parallel process 400,000+ reviews from 1840 hotels to extract multi criteria
information. This processed information is then split into training and testing sets and fed to
Random Forest Classifier for prediction. Finally, it compares the predicted ratings with actual
ratings to assess overall accuracy of the model.
