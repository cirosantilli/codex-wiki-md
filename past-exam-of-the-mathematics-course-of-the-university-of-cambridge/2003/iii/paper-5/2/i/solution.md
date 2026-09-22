<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [quasi-isometry](../../../../../../quasi-isometry.md) $f:X\to Y$ has constants $\lambda\ge1$, $\epsilon\ge0$ such that

$$
\lambda^{-1}d_X(x,x')-\epsilon\le d_Y(f(x),f(x'))\le\lambda d_X(x,x')+\epsilon
$$

for all $x,x'$, and every $y\in Y$ is within $\epsilon$ of some point of $f(X)$. One may use a separate coarse-surjectivity constant and enlarge $\epsilon$ to include it. No continuity is required.

Choose $f'(y)\in X$ with $d_Y(f(f'(y)),y)\le\epsilon$. The triangle inequality gives

$$
d_Y(y,y')-2\epsilon\le d_Y(f(f'(y)),f(f'(y')))\le d_Y(y,y')+2\epsilon.
$$

Combining this with the distortion inequalities for $f$ yields

$$
\lambda^{-1}d_Y(y,y')-\frac{3\epsilon}{\lambda}\le d_X(f'(y),f'(y'))\le\lambda d_Y(y,y')+3\lambda\epsilon.
$$

Also $d_Y(f(f'(f(x))),f(x))\le\epsilon$, so the lower distortion inequality gives $d_X(f'(f(x)),x)\le2\lambda\epsilon$. Hence every point of $X$ is within $2\lambda\epsilon$ of the image of $f'$. Taking the larger common error constant shows that **$f'$ is a $(\lambda,3\lambda\epsilon)$ [quasi-isometry](../../../../../../quasi-isometry.md)**. It is a [quasi-inverse of a quasi-isometry](../../../../../../quasi-inverse-of-a-quasi-isometry.md); both composites are uniformly close to their respective identities.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
