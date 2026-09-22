<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Work with the stipulated approximate [conditional likelihood](../../../../../../conditional-likelihood.md). Let $Z_0=\{i:y_i=0\}$ and $Z_+=\{i:y_i>0\}$, and put

$$
a_i(p)=(1-p)^{t_i},\qquad A_i(\theta,p)=\theta+(1-\theta)a_i(p).
$$

Terms independent of the parameters, including the positive-count [binomial coefficients](../../../../../../binomial-coefficient.md), can be omitted. The [log-likelihood](../../../../../../log-likelihood.md) is

$$
\ell(\theta,p)=\sum_{i\in Z_0}\log A_i
+|Z_+|\log(1-\theta)
+\sum_{i\in Z_+}\{y_i\log p+(t_i-y_i)\log(1-p)\}.
$$

For an interior [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md), set its two [score functions](../../../../../../informant-function.md) to zero. Differentiating with respect to $\theta$ gives

$$
\boxed{\sum_{i\in Z_0}\frac{1-(1-p)^{t_i}}
{\theta+(1-\theta)(1-p)^{t_i}}
-\frac{|Z_+|}{1-\theta}=0.}
$$

Differentiating with respect to $p$ gives

$$
\boxed{-\sum_{i\in Z_0}\frac{(1-\theta)t_i(1-p)^{t_i-1}}
{\theta+(1-\theta)(1-p)^{t_i}}
+\sum_{i\in Z_+}\left\{\frac{y_i}{p}-\frac{t_i-y_i}{1-p}\right\}=0.}
$$

Here there are seven zero-count patients and five positive-count patients, with $\sum_{Z_+}y_i=23$ and $\sum_{Z_+}(t_i-y_i)=36$. Thus the positive-count contribution to the second equation is $23/p-36/(1-p)$.

An interpretable way to solve the equations uses a posterior cure weight for each observed patient:

$$
q_i(\theta,p)=\begin{cases}
\displaystyle\frac{\theta}{\theta+(1-\theta)(1-p)^{t_i}},&y_i=0,\\
0,&y_i>0.
\end{cases}
$$

For a zero count, $1-q_i=(1-\theta)(1-p)^{t_i}/A_i$ is the posterior probability of belonging to the non-cured component under this approximate conditional model. The two [score functions](../../../../../../informant-function.md) can then be rewritten as

$$
\frac{\sum_i q_i}{\theta}-\frac{\sum_i(1-q_i)}{1-\theta},\qquad
\frac{\sum_i y_i}{p}-\frac{\sum_i(1-q_i)(t_i-y_i)}{1-p}.
$$

Therefore the [conditional cure-weight equations for paired Poisson counts](../../../../../../conditional-cure-weight-equations-for-paired-poisson-counts.md) are

$$
\boxed{\widehat\theta=\frac1n\sum_iq_i(\widehat\theta,\widehat p),\qquad
\widehat p=\frac{\sum_i y_i}{\sum_i[1-q_i(\widehat\theta,\widehat p)]t_i}.}
$$

They can be solved by an [expectation-maximization algorithm](../../../../../../expectation-maximization-algorithm.md): calculate the weights at the current parameters, update $\theta$ to their mean and $p$ to the weighted event fraction, and iterate. A solution of the equations must be checked as a maximum; the equations alone do not guarantee a global maximum. In particular the boundary $\theta=0$ gives the no-cure estimate $p=1/8$ and should be compared. Boundaries $p=0$, $p=1$ or $\theta=1$ have zero likelihood for these positive counts with positive pre-treatment counts. Numerical maximization gives an interior fit about $(0.57549,0.38614)$, with larger [log-likelihood](../../../../../../log-likelihood.md) than the no-cure boundary, consistent with the PDF's rounded estimates.

The word “approximate” is important. If cure is specified before conditioning in the original [Poisson distributions](../../../../../../poisson-distribution.md), the conditional cure probability given $T_i=t_i$ would actually be

$$
\Pr(\text{cured}\mid T_i=t_i)
=\frac{\theta}{\theta+(1-\theta)e^{-\beta\lambda_i}(1+\beta)^{t_i}},
$$

which still depends on $\lambda_i$. This follows because a cured total has mean $\lambda_i$ and a non-cured total has mean $(1+\beta)\lambda_i$. The likelihood supplied in the question instead treats $\theta$ as the mixture probability after conditioning; the score and weight equations above maximize exactly that stipulated approximation, without claiming nuisance-rate elimination for the full cure model.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
