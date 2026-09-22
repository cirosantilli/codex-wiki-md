<h1 id="28l/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $\delta(X)=X$ and $X\sim\operatorname{Pois}(\theta)$,

$$
R(\theta,\delta)
=\frac1\theta\mathbb E_\theta[(X-\theta)^2]
=\frac{\operatorname{Var}_\theta(X)}{\theta}
=1.
$$

Thus this rule has constant risk one.

To show that no rule has smaller worst-case risk, fix any $\alpha>1$ and let

$$
\pi_j=\operatorname{Gamma}(\alpha,\lambda_j),
\qquad \lambda_j\downarrow0.
$$

Part (a) gives

$$
\theta\mid X=x\sim
\operatorname{Gamma}(\alpha+x,\lambda_j+1).
$$

Since the reciprocal moment of a gamma variable with shape $k>1$ and rate $s$ is $s/(k-1)$, part (b)(iii) gives the Bayes rule

$$
\delta_j(x)=\frac{\alpha+x-1}{\lambda_j+1}.
$$

Its minimum posterior expected loss is

$$
\mathbb E(\theta\mid X=x)
-\big(\mathbb E(\theta^{-1}\mid X=x)\big)^{-1}
=\frac{\alpha+x}{\lambda_j+1}
-\frac{\alpha+x-1}{\lambda_j+1}
=\frac1{\lambda_j+1}.
$$

Hence the Bayes risk is

$$
r_j=\frac1{\lambda_j+1}\longrightarrow1.
$$

The criterion from part (b)(ii) now proves

$$
\boxed{\delta(X)=X\text{ is minimax}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [28L](../../28l.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
