# NumPY-Mini-Project-Udacity
# Mean Normalization
In machine learning we use large amounts of data to train our models. Some machine learning algorithms may require that the data is *normalized* in order to work correctly. The idea of normalization, also known as *feature scaling*, is to ensure that all the data is on a similar scale, *i.e.* that all the data takes on a similar range of values. For example, we might have a dataset that has values between 0 and 5,000. By normalizing the data we can make the range of values be between 0 and 1.

In this lab, you will be performing a different kind of feature scaling known as *mean normalization*. Mean normalization will scale the data, but instead of making the values be between 0 and 1, it will distribute the values evenly in some small interval around zero. For example, if we have a dataset that has values between 0 and 5,000, after mean normalization the range of values will be distributed in some small range around 0, for example between -3 to 3. Because the range of values are distributed evenly around zero, this guarantees that the average (mean) of all elements will be zero. Therefore, when you perform *mean normalization* your data will not only be scaled but it will also have an average of zero. 


# Data Separation
After the data has been mean normalized, it is customary in machine learnig to split our dataset into three sets:

A Training Set
A Cross Validation Set
A Test Set
The dataset is usually divided such that the Training Set contains 60% of the data, the Cross Validation Set contains 20% of the data, and the Test Set contains 20% of the data.

In this part of the lab you will separate X_norm into a Training Set, Cross Validation Set, and a Test Set. Each data set will contain rows of X_norm chosen at random, making sure that we don't pick the same row twice. This will guarantee that all the rows of X_norm are chosen and randomly distributed among the three new sets.

