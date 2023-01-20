# Statistical Analysis Reports <img align="right" width="75" height="75" src="https://cdn.pixabay.com/photo/2018/01/12/16/16/growth-3078543_960_720.png">

Here are two summaries of reports I did as part of my comprehensive exam in my master's program. The full reports are also uploaded to this repository.

## Multivariate Analysis using SAS 

#### Data

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

## Regression Analysis using R

#### Data 

The yacht data set gives six variables that could potentially be used to predict residuary resistant (ResidResis) of sailing yachts. Knowledge of a ship’s residuary resistance can be useful to determine the ship’s performance and to estimate the required propulsive power. The six variables are longitudinal position of the center of buoyancy (LongiPos), prismatic coefficient (PrisCoef), length-displacement ratio (LDRatio), beam-draughtratio (BDRatio), length-bean ratio (LBRatio), and Froude number (Froude), all adimensional. 

#### Summary 
I first re-code LongiPos as a categorical variable with five levels, calculate sample means for the remaining four, and note one missing observation. Next, I start with a first-order regression model that includes all predictors. A residuals vs fitted plot shows curvature and nonconstancy of error variance while a normal q-q plot shows that the errors are not normally distributed. From this initial model, I transform the data both in Y and X using Box-Cox and Box-Tidwell trans-formations. A best subsets algorithm determines that a model with PrisCoef, BDRatioT, FroudeT, and LongiPos2 predictors is the best. I further improve on the model and determine that the transformedFroude numbers is the best variable to predict residuary resistance. I also conclude that the association between residuary resistance and Froude number was not the same across levels of LongiPos 
