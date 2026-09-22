<h1 id="22g/solution">Solution</h1>

↑ **Parent:** [22G](../22g.md)

Use the convention

$$
\widehat f(\xi)=\int_{\mathbb R^n}f(x)e^{-ix\cdot\xi}\,dx.
$$

The [Riemann-Lebesgue lemma](../../../../../riemann-lebesgue-lemma.md) states that if $f\in L^1(\mathbb R^n)$, then $\widehat f$ is continuous and

$$
\widehat f(\xi)\longrightarrow0
\qquad\text{as }|\xi|\to\infty.
$$

Continuity follows from the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md), since $e^{-ix\cdot\xi_j}\to e^{-ix\cdot\xi}$ and the integrands are dominated by $|f(x)|$.

For the decay, first take $g\in C_c^1(\mathbb R^n)$. Choose a coordinate $j$ for which $|\xi_j|\geq|\xi|/\sqrt n$. Integration by parts gives

$$
\widehat g(\xi)
=\frac1{i\xi_j}
\int_{\mathbb R^n}\partial_jg(x)e^{-ix\cdot\xi}\,dx,
$$

and hence

$$
|\widehat g(\xi)|
\leq\frac{\sqrt n}{|\xi|}\|\partial_jg\|_1
\longrightarrow0.
$$

Since $C_c^1(\mathbb R^n)$ is dense in $L^1(\mathbb R^n)$, choose $g$ with $\|f-g\|_1<\varepsilon$. The elementary Fourier bound gives

$$
|\widehat f(\xi)-\widehat g(\xi)|\leq\|f-g\|_1<\varepsilon,
$$

so the decay for $g$ implies the decay for $f$.

The [Parseval identity](../../../../../parseval-identity.md) says that for $f,g\in L^2(\mathbb R^n)$, with their Fourier transforms defined by the [Plancherel theorem](../../../../../plancherel-theorem.md),

$$
\boxed{
\int_{\mathbb R^n}f(x)\overline{g(x)}\,dx
=\frac1{(2\pi)^n}
\int_{\mathbb R^n}\widehat f(\xi)\overline{\widehat g(\xi)}\,d\xi
}.
$$

In particular,

$$
\|\widehat f\|_2=(2\pi)^{n/2}\|f\|_2.
$$

For the given radial function, as $|x|\to0$,

$$
|f(x)|\sim |x|^a,
$$

while as $|x|\to\infty$,

$$
|f(x)|\sim |x|^{-b}.
$$

Using [polar coordinates](../../../../../polar-coordinates.md), local integrability of $|f|^q$ is therefore determined by

$$
\int_0^1r^{aq+n-1}\,dr<\infty
\quad\Longleftrightarrow\quad aq>-n,
$$

and integrability at infinity by

$$
\int_1^\infty r^{-bq+n-1}\,dr<\infty
\quad\Longleftrightarrow\quad bq>n.
$$

The assumptions $2a>-n$ and $b>n$ imply both $f\in L^2(\mathbb R^n)$ and $f\in L^1(\mathbb R^n)$. The Riemann--Lebesgue lemma and the direct estimate $|\widehat f|\leq\|f\|_1$ give $\widehat f\in L^\infty$, while Parseval gives $\widehat f\in L^2$. Finally, for every $2\leq p<\infty$,

$$
\int_{\mathbb R^n}|\widehat f|^p
\leq
\|\widehat f\|_\infty^{p-2}
\|\widehat f\|_2^2<\infty.
$$

Thus

$$
\boxed{\widehat f\in L^p(\mathbb R^n)\quad\text{for every }2\leq p\leq\infty}.
$$

## ↑ Ancestors (10)

1. [22G](../22g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
