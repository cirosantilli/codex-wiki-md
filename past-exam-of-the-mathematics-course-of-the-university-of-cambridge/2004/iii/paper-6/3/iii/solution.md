<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**The first algebra exists.** Let $A=L^1(0,1)$ with truncated [convolution](../../../../../../convolution.md)

$$
(f*g)(t)=\int_0^t f(s)g(t-s)\,ds.
$$

The [Tonelli theorem](../../../../../../tonelli-theorem.md) gives

$$
\|f*g\|_1\leq\int_{s,u\geq0,\ s+u\leq1}|f(s)||g(u)|\,ds\,du
\leq\|f\|_1\|g\|_1.
$$

[Commutativity](../../../../../../commutativity.md) follows by replacing $s$ with $t-s$; [associativity](../../../../../../associative-property.md) follows from the [Fubini theorem](../../../../../../fubini-s-theorem.md) applied to the simplex $s,u\geq0$, $s+u\leq t$. Together with completeness of $L^1$, this makes $A$ a commutative [Banach algebra](../../../../../../banach-algebra-split.md), not necessarily unital. Adjoin an identity using [unitization](../../../../../../unitization-of-an-algebra.md):

$$
B=\mathbb C\oplus A,\quad
(\alpha,f)(\beta,g)=(\alpha\beta,\alpha g+\beta f+f*g),\quad
\|(\alpha,f)\|=|\alpha|+\|f\|_1.
$$

This [norm](../../../../../../norm.md) is complete and submultiplicative by the preceding bound, and $e=(1,0)$ is the identity. This is the [Volterra convolution algebra on a finite interval](../../../../../../volterra-convolution-algebra-on-a-finite-interval.md) with an identity adjoined.

Take $x=(0,\mathbf1)$, where $\mathbf1(t)=1$. Direct induction under [convolution](../../../../../../convolution.md) gives

$$
x^n=(0,t^{n-1}/(n-1)!),\qquad
\|x^n\|=\frac1{n!}>0.
$$

Thus no power vanishes. For every $\lambda\ne0$ the series

$$
\frac e\lambda+\sum_{n=1}^{\infty}\frac{x^n}{\lambda^{n+1}}
$$

converges absolutely, since its [norms](../../../../../../norm.md) have factorial denominators. Multiplication by $\lambda e-x$ telescopes to $e$, so it is an inverse. On the other hand $x$ cannot be invertible: its scalar coordinate is zero, and scalar coordinates multiply, so $xy$ can never equal $e$. Hence

$$
\boxed{\sigma_B(x)=\{0\},\qquad \rho(x)=0,\qquad x^n\ne0\text{ for every }n\geq1.}
$$

This explicitly exhibits a nonnilpotent [quasinilpotent element](../../../../../../quasinilpotent-element.md) without assuming a spectral-radius formula.

**The second algebra does not exist.** Suppose it did, and choose a nonscalar $y$. Nonemptiness of its [spectrum of an element](../../../../../../spectrum-of-an-element.md), together with $\rho(y)=0$, gives $\sigma_B(y)=\{0\}$. But $y+e$ is still nonscalar: if $y+e=\alpha e$, then $y=(\alpha-1)e$. By [translation of the spectrum by a scalar](../../../../../../translation-of-the-spectrum-by-a-scalar.md),

$$
\sigma_B(y+e)=1+\sigma_B(y)=\{1\},\qquad\rho(y+e)=1.
$$

This contradicts the required zero [spectral radius](../../../../../../spectral-radius.md) for every nonscalar element. The contradiction already uses the spectral condition alone; the nonvanishing-power condition cannot remedy it.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
