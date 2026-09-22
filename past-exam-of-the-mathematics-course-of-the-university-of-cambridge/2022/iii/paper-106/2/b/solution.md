<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $p\geq2$, integrate the stated scalar inequality to obtain the [Clarkson inequality](../../../../../../clarkson-s-inequalities.md)

$$
\left\lVert\frac{f+g}{2}\right\rVert_p^p
+\left\lVert\frac{f-g}{2}\right\rVert_p^p
\leq\frac{\lVert f\rVert_p^p+\lVert g\rVert_p^p}{2}.
$$

If $f,g$ belong to the unit ball and $\lVert f-g\rVert_p\geq\varepsilon$, then

$$
\left\lVert\frac{f+g}{2}\right\rVert_p
\leq\left(1-(\varepsilon/2)^p\right)^{1/p}<1.
$$

Thus $L^p[0,1]$ is [uniformly convex](../../../../../../uniformly-convex-banach-space.md).

Now let $X$ be uniformly convex. It is enough to show that every $\Phi\in S_{X^{**}}$ lies in the canonical image of $X$. Given $\varepsilon>0$, choose the corresponding uniform-convexity constant $\delta$, and choose $f\in B_{X^*}$ with $\Phi(f)>1-\delta$. If $x,y\in B_X$ both satisfy $f(x),f(y)>1-\delta$, then

$$
\left\lVert\frac{x+y}{2}\right\rVert>1-\delta,
$$

so $\lVert x-y\rVert<\varepsilon$. By [Goldstine theorem](../../../../../../goldstine-theorem.md), every weak-star neighbourhood of $\Phi$ contains some $Jx$ with $x\in B_X$. Directing these neighbourhoods produces a norm-Cauchy net $(x_\alpha)$; completeness gives $x_\alpha\to x\in B_X$, and weak-star convergence then gives $Jx=\Phi$. Scaling handles the whole bidual ball, so $X$ is [reflexive](../../../../../../reflexive-banach-space.md).

For $p\geq2$, uniform convexity therefore makes $L^p$ reflexive. If $1<p<2$, its conjugate exponent $q$ is greater than two, so $L^q$ is reflexive. Since $(L^p)^*=L^q$ and a Banach space whose dual is reflexive is itself reflexive, $L^p$ is reflexive for every $1<p<\infty$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
