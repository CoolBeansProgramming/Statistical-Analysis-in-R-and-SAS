# Statistical Analysis Reports <img align="right" width="75" height="75" src="https://cdn.pixabay.com/photo/2018/01/12/16/16/growth-3078543_960_720.png">



## Multivariate Analysis using SAS 

#### Background of Data Set

The skull data set gives four measurements on male Egyptian skulls: maximum breadth,
basilbregmatic height, basialvelar length, and nasal height, all measured in millimeters. The
data are taken from five different time periods.

#### Summary 

To analyze the skull data set, I first determined that there were no multivariate outliers.
Using one-way MANOVA, I concluded that at least one mean vector of the four
measurements from the five different time periods is different. To determine if one or all
vectors differ, I would do multiple comparisons to determine which pairs of groups have
different mean vectors and which components of these mean vectors differ. Using principal
component analysis, I determined that three components are appropriate to effectively
summarize the sample variability and, based on the first and second principal components, it
would be difficult to distinguish between the five time periods. For classification analysis, I
determined that linear discriminant analysis is appropriate using Estimated Minimum TPM Rule
for Equal-Covariance Normal Populations. Further analysis may include interpretation of the
principal components and exploration into the high apparent error rate and estimated
expected actual error rate.

