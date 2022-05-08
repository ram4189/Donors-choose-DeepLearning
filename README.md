# Donors choose application screening

DonorsChoose.org is a platform where public school teachers can request necessary materials and experiences for their students. At any given time, there are thousands of classroom requests that can be brought to life with a gift of any amount.

Every year DonorsChoose.org receives hundreds of thousands of project proposals for classroom projects in need of funding. For manually screening such large amounts of data, right now, a large number of volunteers is required before it’s approved to be posted on the DonorsChoose.org website.

DATASET : https://www.kaggle.com/c/donorschoose-application-screening 


# MEDIUM BLOG: https://medium.com/@smartrambit/deep-learning-project-donors-choose-application-screening-2b1d049a916



![plot](C:\Users\rap\Documents\ML\AAIC_new\Masters\Assignments\donors_choose_NB\donors_choose_new\donors_choose\score_comparison.PNG)


# Conclusions

Here we have tried 3 types of models:

Model1: For Essay feature embedding features has been created using Glove model. All the words are considered while creating features. Since there are more features so model is converging very fast and hence within less number of epochs we are able to get the maximum roc_auc_score. Also here we have used label encoding for categorical features(Thanks for suggesting AAIC team)


Model2: It is similar to Model 2 except that instead of taking all the words as features we are choosing most important features. This we are doing through idf vectorizer. we are not choosing top 25% (These are words like The, a which are most frequent but actually don't contain any meaning. Also bottom idf features are rare features which also do not add any importance. With only 50% important and meaningful features we are able to get good score although in more number of epochs than Model 1 and Model 2. If we use more epochs probably we can get better results.


Model3: Here we are making use of convolution layer to learn any spatial feature in the categorical features. Both Model 1 and Model 3 are performing well, however Model 1 appears to converge faster. Instead of using label encoding here, We have used one hot encoding for categorical variables.



## ðŸš€ About Me
I love to deal with data ...

## Color Reference

| Color             | Hex                                                                |
| ----------------- | ------------------------------------------------------------------ |
| Example Color | ![#0a192f](https://via.placeholder.com/10/0a192f?text=+) #0a192f |
| Example Color | ![#f8f8f8](https://via.placeholder.com/10/f8f8f8?text=+) #f8f8f8 |
| Example Color | ![#00b48a](https://via.placeholder.com/10/00b48a?text=+) #00b48a |
| Example Color | ![#00d1a0](https://via.placeholder.com/10/00b48a?text=+) #00d1a0 |


## Contributing

Contributions are always welcome!

See `contributing.md` for ways to get started.

Please adhere to this project's `code of conduct`.

