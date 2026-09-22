<h1 id="23i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $f\in L^\infty(\mathbb R^n)$ and $g\in L^1(\mathbb R^n)$, define their [convolution](../../../../../../convolution.md) by

$$
(f*g)(x)=\int_{\mathbb R^n}f(y)g(x-y)\,dy.
$$

It is bounded because

$$
|(f*g)(x)|\le\|f\|_\infty\|g\|_1.
$$

If $\tau_hg(z)=g(z+h)$, then

$$
|(f*g)(x+h)-(f*g)(x)|
\le\|f\|_\infty\|\tau_hg-g\|_1.
$$

Continuity of translation in $L^1$ makes the right-hand side tend to zero with $h$, uniformly in $x$. Thus the [convolution of L infinity and L1 functions](../../../../../../convolution-of-l-infinity-and-l1-functions.md) is bounded and continuous.

Now let $f=\mathbf1_A$ and $g(x)=\mathbf1_A(-x)$. Then

$$
(f*g)(z)=\int_{\mathbb R^n}\mathbf1_A(y)\mathbf1_A(y-z)\,dy.
$$

At zero this equals $|A|>0$. By continuity it remains positive throughout some open neighbourhood $U$ of zero. Positivity at $z$ means that some $y$ satisfies $y\in A$ and $y-z\in A$, so $z\in A-A$. Hence

$$
\boxed{U\subseteq A-A}.
$$

This is the [Steinhaus theorem](../../../../../../steinhaus-theorem.md).

The conclusion also holds when $|A|=\infty$. Since $\mathbb R^n$ is the union of bounded balls, some measurable subset $A\cap B(0,R)$ has finite positive measure. Its difference set lies inside $A-A$ and already contains a neighbourhood of zero.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [23I](../../23i.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
