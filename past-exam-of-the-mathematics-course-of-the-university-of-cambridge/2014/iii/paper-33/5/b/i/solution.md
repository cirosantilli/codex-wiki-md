<h1 id="5/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For woman $i$, write $m_i$ for the number of births, $Y_i$ for the number with defects, $a_i$ for baseline age, and $e_i$ for exposure. Let $p_i$ be the common marginal defect probability for her births. The first fit is a grouped [grouped-binomial logistic regression](../../../../../../../grouped-binomial-logistic-regression.md):

$$
Y_i\mid a_i,e_i,m_i\sim\operatorname{Bin}(m_i,p_i),\qquad
\log\frac{p_i}{1-p_i}=\beta_0+\beta_a a_i+\beta_e e_i.
$$

It assumes independent women and, conditionally on their covariates, independent births with the same probability within each woman. The supplied birth totals are the binomial denominators; fitting the proportions with weights $m_i$ is equivalent to this grouped-binomial specification. The fitted linear predictor is $-1.74272+0.02030a_i+2.33028e_i$.

The second fit is a [generalized additive model](../../../../../../../generalized-additive-model.md) with the same logit [link function](../../../../../../../link-function.md) and the mean specification

$$
\log\frac{p_i}{1-p_i}=\beta_0+f_a(a_i)+f_e(e_i),\qquad E(Y_i)=m_ip_i.
$$

The functions $f_a,f_e$ are penalized [cubic regression splines](../../../../../../../cubic-regression-spline.md) with natural boundary conditions. Centering constraints such as $\sum_i f_a(a_i)=\sum_i f_e(e_i)=0$ separate them from the intercept; the fitted centered intercept is $-0.2031$. Their [second derivative roughness penalties](../../../../../../../second-derivative-roughness-penalty.md) control complexity.

The call estimates a common scale rather than fixing it at one. Its working [variance](../../../../../../../variance-split.md) specification for the counts is

$$
\boxed{\operatorname{Var}(Y_i)=\phi m_ip_i(1-p_i),\qquad\widehat\phi=3.3506.}
$$

Equivalently the variance of $Y_i/m_i$ is $\phi p_i(1-p_i)/m_i$. This is the working moment interpretation of an overdispersed binomial [generalized additive model](../../../../../../../generalized-additive-model.md): the code uses binomial deviance for fitting and estimated scale for inference. With $\phi\ne1$, it is not an exact independent-binomial sampling model. Women are still treated as independent groups, but within-woman dependence or unobserved heterogeneity can motivate the extra dispersion. The [quasibinomial regression](../../../../../../../quasibinomial-regression.md) interpretation states what the scaled analysis assumes without inventing a full probability distribution for its counts.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 33](../../../../paper-33-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
