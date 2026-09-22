<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $a$ prime to $p$, put

$$
b_a(X)=\frac{X^{-a}-X^a}{X^{-1}-X}
=X^{1-a}\frac{1-X^{2a}}{1-X^2},\qquad f_a(T)=b_a(1+T)^{p-1}.
$$

For positive $a$, $b_a(X)=X^{1-a}\sum_{j=0}^{a-1}X^{2j}$ is a [Laurent polynomial](../../../../../../laurent-polynomial.md). For negative $a$, use $b_a=-b_{-a}$. Hence it is regular at $X=1$ with value $a$, and $f_a\in\mathbb Z_p[[T]]^\times$ has constant coefficient $a^{p-1}\equiv1\pmod p$. Evaluation at $\zeta_n$ shows that $c_n(a)$ is a [unit](../../../../../../unit-in-a-ring.md) and reduces to one in the [residue field](../../../../../../residue-field.md), so $c_n(a)\in U_n$.

Because $p$ is odd, $\prod_{\xi\in\mu_p}\xi=1$. Both maps $\xi\mapsto\xi^2$ and $\xi\mapsto\xi^{2a}$ permute $\mu_p$, and therefore

$$
\begin{aligned}
\prod_{\xi^p=1}b_a(\xi X)
&=X^{p(1-a)}\frac{\prod_{\xi^p=1}(1-\xi^{2a}X^{2a})}
{\prod_{\xi^p=1}(1-\xi^2X^2)}\\
&=X^{p(1-a)}\frac{1-X^{2ap}}{1-X^{2p}}=b_a(X^p).
\end{aligned}
$$

This rational-function identity also holds for negative $a$ and extends across the removable point $X=1$. It implies $Nf_a=f_a$. Part 1(b) now proves all the required norm compatibilities, and **$c(a)\in U_\infty$**, with Coleman series $f_a$.

Use the additive formal coordinate $z=\log(1+T)$, in which $D=d/dz$. Then

$$
f_a(e^z-1)=\left(\frac{\sinh(az)}{\sinh z}\right)^{p-1}.
$$

Its logarithm after normalization by $a^{p-1}$ is even, so all odd derivatives at zero vanish. For the even derivatives, the [hyperbolic cotangent generating function for Bernoulli numbers](../../../../../../hyperbolic-cotangent-generating-function-for-bernoulli-numbers.md) gives

$$
\begin{aligned}
\frac{d}{dz}\log f_a(e^z-1)
&=(p-1)\bigl(a\coth(az)-\coth z\bigr)\\
&=(p-1)\sum_{j\geq1}\frac{2^{2j}B_{2j}(a^{2j}-1)}{(2j)!}z^{2j-1}.
\end{aligned}
$$

Here the [Bernoulli numbers](../../../../../../bernoulli-number.md) use $B_1=-1/2$. Differentiating $k-1$ more times yields the answer for every index:

$$
\boxed{\delta_k(c(a))=\begin{cases}
0,&k\text{ odd},\\
(p-1)2^k(a^k-1)\dfrac{B_k}{k},&k\geq2\text{ even}.
\end{cases}}
$$

These rational expressions lie in $\mathbb Z_p$ because they equal the integral logarithmic-derivative definition in part (a). In particular $\delta_1=0$; substituting $B_1$ into the even-index formula would give an incorrect answer. For $a=\pm1$ the sequence is one and every derivative vanishes, as the formula also shows.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
