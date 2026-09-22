<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $x\in X$, let $e_x$ be the [indicator function](../../../../indicator-function.md) of $\{x\}$. In the [ring of functions](../../../../ring-of-functions.md) $R=\mathbb R^X$, multiplication is pointwise, so

$$
e_xf=f(x)e_x.
$$

Suppose first that $X$ is finite, and let $J$ be an [ideal](../../../../ideal.md) of $R$. Define $S=\{x\in X:f(x)\ne0\text{ for some }f\in J\}$. If $x\in S$, choose such an $f$; multiplying it by $e_x/f(x)$ shows that $e_x\in J$. Every $f\in J$ satisfies

$$
f=\sum_{x\in S}f(x)e_x,
$$

where the real scalars are constant [functions](../../../../function-split.md). Thus $J=(e_x:x\in S)$ has a finite [generating set of an ideal](../../../../generating-set-of-an-ideal.md), so $R$ is a [Noetherian ring](../../../../noetherian-ring.md). If $X$ is empty, $R$ is the [zero ring](../../../../zero-ring.md), and the conclusion still holds.

If $X$ is infinite, consider the [ideal](../../../../ideal.md)

$$
F=\{f\in\mathbb R^X:\{x:f(x)\ne0\}\text{ is finite}\}.
$$

It is an [ideal](../../../../ideal.md) because a sum has [support](../../../../support.md) contained in the union of the two [supports](../../../../support.md), and multiplication by any [function](../../../../function-split.md) cannot enlarge [support](../../../../support.md). If $f_1,\ldots,f_r$ generated $F$, their [supports](../../../../support.md) would have a finite union $T$. Every element of $(f_1,\ldots,f_r)$ would vanish outside $T$, whereas $e_x\in F$ for any $x\in X\setminus T$. This contradiction proves

$$
\boxed{\mathbb R^X\text{ is Noetherian}\iff X\text{ is finite}.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the commutative algebra course of the University of Oxford](../../../split.md)
5. [Commutative algebra course of the University of Oxford](../../../../commutative-algebra-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
