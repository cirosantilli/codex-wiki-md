<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $\sigma>1$, the [three-four-one zero-free-region argument](../../../../../../three-four-one-zero-free-region-argument.md) starts from

$$
3+4\cos\theta+\cos2\theta=2(1+\cos\theta)^2\geq0.
$$

Applying this termwise to

$$
-\frac{\zeta'(s)}{\zeta(s)}
=\sum_{n\geq1}\frac{\Lambda(n)}{n^s}
$$

gives

$$
-3\frac{\zeta'(\sigma)}{\zeta(\sigma)}
-4\Re\frac{\zeta'(\sigma+it)}{\zeta(\sigma+it)}
-\Re\frac{\zeta'(\sigma+2it)}{\zeta(\sigma+2it)}
\geq0.
$$

Suppose $\rho=\beta+i\gamma$ is a zero with $|\gamma|\geq4$. In the supplied [Local partial-fraction expansion of the Riemann zeta logarithmic derivative](../../../../../../local-partial-fraction-expansion-of-the-riemann-zeta-logarithmic-derivative.md), every nearby zero contributes a nonnegative real part at $\sigma+i\gamma$ when $\sigma>1$. Keeping the term from $\rho$ gives

$$
\Re\frac{\zeta'(\sigma+i\gamma)}{\zeta(\sigma+i\gamma)}
\geq\frac1{\sigma-\beta}-O(\log|\gamma|).
$$

At height zero the pole at one gives

$$
-\frac{\zeta'(\sigma)}{\zeta(\sigma)}
=\frac1{\sigma-1}+O(1),
$$

and the same local expansion at height $2\gamma$ gives

$$
-\Re\frac{\zeta'(\sigma+2i\gamma)}{\zeta(\sigma+2i\gamma)}
\ll\log|\gamma|.
$$

Substitution yields

$$
\frac4{\sigma-\beta}
\leq\frac3{\sigma-1}+O(\log|\gamma|).
$$

Set $\sigma=1+\eta/\log|\gamma|$, first choosing a sufficiently small absolute $\eta>0$. If $\beta>1-c/\log|\gamma|$, the left side is at least $4\log|\gamma|/(\eta+c)$. Choosing $c>0$ sufficiently small contradicts the last inequality. Therefore

$$
\boxed{\zeta(s)\ne0
\quad\text{for}\quad
\sigma>1-\frac c{\log|t|},\quad |t|\geq4.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
