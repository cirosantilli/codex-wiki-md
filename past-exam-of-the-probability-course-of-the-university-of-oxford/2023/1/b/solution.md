<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [Borel set](../../../../borel-set.md) $A\subseteq\mathbb R$, the [joint probability density](../../../../joint-probability-density.md) gives

$$
\mathbb P(XY\in A)=\int_{\mathbb R}\int_{\mathbb R}\mathbf1_A(xy)f(x,y)\,dy\,dx.
$$

For each $x\ne0$, substitute $z=xy$. The [change of variables for probability densities](../../../../change-of-variables-for-probability-densities.md) contributes $dy=dz/|x|$, with the absolute value accounting for the reversed orientation when $x<0$. The line $x=0$ has two-dimensional [Lebesgue measure](../../../../lebesgue-measure.md) zero, so omitting it changes no [probability](../../../../probability.md). By the [Tonelli theorem](../../../../tonelli-theorem.md),

$$
\mathbb P(XY\in A)=\int_A\left[\int_{\mathbb R\setminus\{0\}}\frac1{|x|}f\left(x,\frac zx\right)\,dx\right]dz.
$$

The bracket is nonnegative and its [integral](../../../../integral-split.md) over $\mathbb R$ is one. This proves the [probability density of a product of random variables](../../../../probability-density-of-a-product-of-random-variables.md) formula:

$$
\boxed{f_Z(z)=\int_{\mathbb R\setminus\{0\}}\frac1{|x|}f\left(x,\frac zx\right)\,dx.}
$$

As usual, a [probability density function](../../../../probability-density-function.md) is determined only almost everywhere; exceptional infinite values are harmless.

For the [independent random variables](../../../../independent-random-variables.md) with the specified [uniform distribution](../../../../continuous-uniform-distribution.md), $f(x,y)=b^{-2}$ on $(0,b)^2$ and zero elsewhere. When $0<z<b^2$, the conditions $0<x<b$ and $0<z/x<b$ are equivalent to $z/b<x<b$. Therefore

$$
f_Z(z)=\frac1{b^2}\int_{z/b}^{b}\frac{dx}{x}=\frac1{b^2}\log\frac{b^2}{z},
\qquad
\boxed{f_Z(z)=\begin{cases}b^{-2}\log(b^2/z),&0<z<b^2,\\0,&\text{otherwise}.\end{cases}}
$$

The value assigned at zero is arbitrary. Substitution $s=z/b^2$ checks [normalization of a probability distribution](../../../../normalization-of-a-probability-distribution.md): $\int_0^1-\log s\,ds=1$. This is the [product of independent uniform random variables](../../../../product-of-independent-uniform-random-variables.md) law.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the probability course of the University of Oxford](../../../split.md)
5. [Probability course of the University of Oxford](../../../../probability-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
