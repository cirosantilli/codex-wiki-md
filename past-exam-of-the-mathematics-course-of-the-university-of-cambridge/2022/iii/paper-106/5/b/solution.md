<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Identify $X$ with its canonical image in $X^{**}$ and put

$$
d=d(\Phi,X)>0,
\qquad
c=\frac d{d+1}.
$$

For $x\in S_X$ and $\lambda\in\mathbb R$, if $|\lambda|\leq1/(d+1)$ then

$$
\lVert x-\lambda\Phi\rVert
\geq1-|\lambda|\lVert\Phi\rVert
\geq\frac d{d+1}=c.
$$

If $|\lambda|\geq1/(d+1)$, then

$$
\lVert x-\lambda\Phi\rVert
\geq d(\lambda\Phi,X)=|\lambda|d\geq c.
$$

Therefore $d(x,\operatorname{span}\{\Phi\})\geq c$.

The restriction of $x\in X^{**}$ to $\ker\Phi\subseteq X^*$ has norm

$$
\sup_{g\in B_{\ker\Phi}}|g(x)|
=d(x,(\ker\Phi)^\perp)
=d(x,\operatorname{span}\{\Phi\})
\geq c,
$$

where the first equality is the [Hahn-Banach distance formula](../../../../../../hahn-banach-distance-formula.md) and $(\ker\Phi)^\perp=\operatorname{span}\{\Phi\}$. Scaling from $S_X$ gives

$$
c\lVert x\rVert\leq\sup_{g\in B_{\ker\Phi}}|g(x)|
$$

for every $x\in X$. Hence $\ker\Phi$ is $c$-norming for $X$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
