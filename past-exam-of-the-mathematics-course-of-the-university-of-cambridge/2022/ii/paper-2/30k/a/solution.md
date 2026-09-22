<h1 id="30k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put

$$
q=\mu-(1+r)S_0,\qquad h=m-(1+r)x.
$$

For a risky holding vector $\theta$ and the remaining wealth in the bank,

$$
X_1=(1+r)x+\theta^T(S_1-(1+r)S_0),
$$

so

$$
\mathbb E X_1=(1+r)x+\theta^Tq,\qquad
\operatorname{Var}(X_1)=\theta^TV\theta.
$$

When $V$ is nonsingular it is positive definite. Cauchy--Schwarz in the  
$V$ inner product gives

$$
(\theta^Tq)^2
\leq(\theta^TV\theta)(q^TV^{-1}q),
$$

with equality exactly when $\theta=\lambda V^{-1}q$. Under  
$\theta^Tq=h$,

$$
\boxed{\theta^*=
\frac{h}{q^TV^{-1}q}V^{-1}q,\qquad
\min\operatorname{Var}(X_1)
=\frac{h^2}{q^TV^{-1}q}}.
$$

For the constraint $\mathbb E X_1\geq m$, if $h\leq0$ the zero risky portfolio is feasible and the minimum variance is zero. If $h>0$, the inequality binds and the preceding optimizer and minimum apply.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [30K](../../30k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
