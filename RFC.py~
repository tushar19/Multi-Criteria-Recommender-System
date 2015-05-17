#!/usr/bin/env python

from sklearn.ensemble import RandomForestClassifier
from sklearn import neighbors, datasets
import math
from numpy import genfromtxt
import re

data_features_file = 'Features.txt'
data_features_train_file = 'features_data_train.txt'
data_features_test_file = 'features_data_test.txt'
X_train = []
Y_train= []
X_test= []
Y_test= []
Xtrain= []
Xtest = []

def main():
        get_data()

        rf = RandomForestClassifier(n_estimators=100)
    	rf.fit(X_train, Y_train)
    	predicted_probs =  rf.predict_proba(X_test)
    	predicted_probs = ["%f" % x[1] for x in predicted_probs]
    	print predicted_probs
    	#csv_io.write_delimited_file("rf_benchmark.csv", predicted_probs)
   

def get_features():
	features = []
	
	f = open(data_features_file, 'r+')
	for line in f:
		features.append(line.strip())
	f.close()
	return features

def get_data():
	
	f = open(data_features_train_file, 'r+')
	for line in f:

		Y_train, X1 = line.strip().split('\t')
		X_train = re.split(' ', X1)
		
	f.close()

	f = open(data_features_test_file, 'r+')
	for line in f:
		Y_test, X2 = line.strip().split('\t')
		X_test = re.split(' ', X2)
		
		
		
	f.close()

	return


if __name__=="__main__":

    main()
