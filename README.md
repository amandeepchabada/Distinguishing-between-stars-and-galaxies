# Distinguishing between stars and galaxies

Comparing different methods to deal with missing values and to determine which one was the most effective in helping us distinguish between stars and galaxies

# Table of results

|     Method                         |     Average Test Accuracy    |     Avg test accuracy with missing values only    |
|------------------------------------|------------------------------|---------------------------------------------------|
|     No   Processing                |     0.72                     |     0.56                                          |
|     A.   Omit missing Samples      |     0.37                     |     0.00                                          |
|     B.   Predict Majority Class    |     0.66                     |     0.41                                          |
|     C.   Omit Missing Features     |     0.79                     |     0.71                                          |
|     D.   Impute Average Values     |     0.73                     |     0.56                                          |
|     E.   Winsorize                 |     0.75                     |     0.59                                          |

I would recommend Method C. Omit Missing Features for this particular dataset as it has the best accuracy. However, this may not be completely appropriate for other datasets as Omitting missing features may lead to overfitting and poor generalization. 
The classifier might latch on to some feature and give it a very high weightage which may lead to us losing out on some of the more intricate trends in the data. 
Winsorizing is another method which I would recommend as it performed similarly and succeeded in keeping the crux of the data relations intact.
