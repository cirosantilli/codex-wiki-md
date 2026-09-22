<h1 id="29k/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The risk of $\overline X_n$ is constantly $1/n$. Suppose an estimator $\delta$ dominates it, and put  
$m(\theta)=\mathbb E_\theta\delta$ and $b(\theta)=m(\theta)-\theta$. The biased [Cramér-Rao bound](../../../../../../cramer-rao-bound.md), using total information $n$, gives

$$
R(\theta,\delta)\geq
\frac{m'(\theta)^2}{n}+b(\theta)^2.
$$

Domination would imply

$$
(1+b'(\theta))^2+n b(\theta)^2\leq1
$$

for every real $\theta$. The standard differential-inequality argument shows that the only globally defined differentiable solution is $b\equiv0$: a nonzero value forces $b'$ to retain a sign and magnitude that makes $b$ leave the permitted bounded interval in one time direction.

Thus $m(\theta)=\theta$. The Cramer--Rao inequality now gives  
$\operatorname{Var}_\theta\delta\geq1/n$, so domination forces equality everywhere. Equality in Cramer--Rao makes the centred estimator proportional to the Gaussian score:

$$
\delta-\theta=\frac1n\sum_i(X_i-\theta),
$$

and hence $\delta=\overline X_n$ almost surely. No strict improvement exists, so $\overline X_n$ is admissible.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [29K](../../29k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
