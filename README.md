# Regression

methods on regressing Y onto X. regression is useful for:

* modelling relationships
* predicting the future
* testing relationships

remember: **all models are wrong, but some are useful** - g. box

## Generalized Linear Models

GLMs are normally covered in later portions of regression courses, but I think it makes sense to understand them first. take a look at the table below:


| Distribution | Link Function | Regression Function |
| ------------ :| ------------- :| -------------------: |
| Normal | $g(\mu) = \mu$ | $\mu = x^T\beta$ |
| Binomial | $g(\mu) = log(frac{\mu}{1-\mu})$ | $\mu = \frac{e^x^T\beta}{1+e^x^T\beta}$ |
| Poisson | $g(\mu) = log(\mu)$ | $ m = e^x^T\beta |
| Gamma | $g(\mu) = \frac{1}{\mu}$ | $ \mu = \frac{1}{x^T\beta}$ |

Generalizing a linear model simply means allowing us to regress Y onto X across different distributions that Y may follow. The typical linear regression assumes Y is sampled from a simple normal distribution.
