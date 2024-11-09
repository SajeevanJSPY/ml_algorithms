#### Simple Linear Model

simple linear model relationship,
$$y \approx \beta 0 + \beta 1 x$$
estimator function for linear models, 
$$\hat y \approx \hat{\beta 0}  + \hat{\beta 1} x$$

Let $\hat{y_i} = \hat{\beta 0} \hat{\beta 1} x_i$ be the prediction for Y based on the $\large i$th value of X, 
Then $e_i = y_i - \hat{y_i}$ represents the $\large i$th residual
we define the *residual sum of squares* (**RSS**) as
$$ RSS = e_1^2 + e_2^2 + ... + e_n^2 $$
$$ 
\hat{\beta 1} = \frac
	{\sum_{i=1}^n{(x_i - \overline x)(y_i - \overline y)}}
	{\sum_{i=1}^n{(x_i - \overline x)^2}} 
$$
$$\hat{\beta 0} = \overline y - \hat{\beta 1}\overline x$$
where $\large \overline y \equiv \frac{1}{n}\sum_{i=1}^n{y_i}$ and $\overline x \equiv \frac{1}{n}\sum_{i=1}^n{x_i}$ are the sample means

###### Assessing the Accuracy of the Coefficient Estimates

we assume that the *true* relationship between X and Y takes the form
				$Y = f(X) + \large \epsilon$
for some unknown function $\large f$, where $\large \epsilon$ is a mean-zero random error term
$$Y = \beta 0 + \beta 1 X + \large \epsilon$$
*standard error* of $\hat{\large \mu}$ , written as SE($\hat{\large \mu}$)
$$Var(\hat{\large \mu}) = SE(\hat{\large \mu})^2  = \large \frac{\sigma^2}{n}$$
To compute the standard errors associated with $\hat{\beta 0}$ and $\hat{\beta 1}$, we use the following formulas:
$$
SE(\hat{\beta 0})^2 = \large \sigma ^ 2 \left [\frac{1}{n} + \frac{ \overline x^2}{\sum_{i=1}^n{(x_i - \overline{x})^2}} \right]
$$
$$
SE(\hat{\beta 1})^2 = \frac{ \sigma^2}{\sum_{i=1}^n{(x_i - \overline{x})^2}}
$$

*residual standard error* and is given by the formula
			$RSE = \large \sqrt \frac{RSS}{n-2}$

Standard errors can be used to compute *confidence intervals*
For linear regression, the 95% confidence interval for $\large \beta_1$ approximately takes the form
			$\large \hat{\beta 1}^2 \pm \; 2 \cdot SE(\hat{\beta 1})$ 

