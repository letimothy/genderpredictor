# genderpredictor
Predicts male or female based on height, weight, and shoe size

Python

#Begin:

from sklearn import tree

# [height, weight, shoe size]
X = [[181,80,44], [177,70,43], [160,60,38], [166,56,40]]

Y = ['male', 'female', 'female', 'male']

clf = tree.DecisionTreeClassifier()

clf = clf.fit(X,Y)

prediction = clf.predict([[190,70,43]])
print(prediction)
