# PCA_Multicollinearity and Intrinsic Low Dimension
#PCA #Multicollinearity #Intrinsic Low Dimension

### Why is Multicollinearity a Potential Problem?
- Multicollinearity refers to a condition in which the independent variables are correlated to each other
- Multicollinearity can also affect the interpretation of the model, as it undermines the statistical significance of independent variables.
- Getting very high standard errors for regression coefficients
- The overall model is significant, but none of the coefficients are significant

### How do you apply PCA to remove Multicollinearity?
- PCA (Principal Component Analysis) takes advantage of multicollinearity and combines the highly correlated variables into a set of uncorrelated variables.
- Therefore, PCA can effectively eliminate multicollinearity between features.
<img width="706" alt="Screenshot 2023-12-21 at 3 45 45 PM" src="https://github.com/ColleenJung/PCA_Multicollinearity-andIntrinsic-Low-Dimension/assets/119357849/158e2f39-45f3-4857-8cc5-13fb2f7f6f8a">


### PCA Model
- The goal of PCA is to identify patterns in a data set, and then distill the variables down to their most important features so that the data is simplified without losing important traits.

### Intrinisic dimension
- Intrinsic dimension is the number of PCA features needed to approximate a dataset.
- If we need to reduce the dimension we should know which features we should select and which to neglect.
- Usually, PCA in Sklearn will automatically find the number of Intrinsic Dimensions itself.
- It will consider PCA features with significant variance.

### How?
- Discards low variance PCA features
- Assumes the high variance features are informative
