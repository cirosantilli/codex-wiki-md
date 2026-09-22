<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A real [random variable](../../../../../random-variable-split.md) is a [sub-Gaussian random variable](../../../../../sub-gaussian-distribution.md) with exponent $b\geq0$ when its [moment-generating function](../../../../../moment-generating-function.md) satisfies

$$
\mathbb E e^{tX}\leq e^{b^2t^2/2}\qquad(t\in\mathbb R).
$$

Differentiating at $t=0$ from both sides gives $\mathbb EX=0$. Exponential integrability near zero justifies this differentiation. Conversely, if $|X|\leq M$ and $\mathbb EX=0$, [convexity](../../../../../convex-function.md) gives

$$
e^{tX}\leq\frac{M+X}{2M}e^{tM}+\frac{M-X}{2M}e^{-tM},\qquad
\mathbb Ee^{tX}\leq\cosh(tM)\leq e^{t^2M^2/2}.
$$

The last inequality follows by comparing power series using $(2j)!\geq2^j j!$. The case $M=0$ is immediate. Thus **a bounded [random variable](../../../../../random-variable-split.md) is sub-Gaussian exactly when it is centered**; the bound $M$ is one possible exponent.

For $b>0$, the [Markov inequality](../../../../../markov-inequality.md) applied to $e^{tX}$ gives $\mathbb P(X>R)\leq\exp(b^2t^2/2-tR)$. Choose $t=R/b^2$ and repeat with $-X$. The [union bound](../../../../../boole-s-inequality.md) yields

$$
\boxed{\mathbb P(|X|>R)\leq2e^{-R^2/(2b^2)}}\qquad(R>0).
$$

If $b=0$, the same exponential estimate with arbitrarily large $t$ shows $X=0$ almost surely, so all subsequent inequalities are trivial.

Integrating this [tail probability](../../../../../tail-probability.md) estimate gives, for every real $k\geq2$,

$$
\mathbb E|X|^{2k}=2k\int_0^\infty r^{2k-1}\mathbb P(|X|>r)\,dr
\leq2(2b^2)^k\Gamma(k+1).
$$

We need $2\Gamma(k+1)\leq k^k$. For integer $k$ this follows inductively from $2\cdot2!=2^2$ and $(k+1)k^k\leq(k+1)^{k+1}$. To cover real $k$ as well, set $H(k)=k\log k-\log\Gamma(k+1)-\log2$. Differentiating the [Gamma function](../../../../../gamma-function.md) integral gives $(\log\Gamma)'(k+1)=\mathbb E\log Y$ for a [Gamma distribution](../../../../../gamma-distribution.md) with shape $k+1$ and rate $1$. The [Jensen inequality](../../../../../jensen-s-inequality.md) bounds this by $\log(k+1)$. Hence $H'(k)\geq1-\log(1+1/k)>0$ and $H(2)=0$. Taking the $2k$th root now proves

$$
\boxed{\|X\|_{2k}\leq b\sqrt{2k}\quad(k\geq2)}.
$$

Here $\|X\|_p=(\mathbb E|X|^p)^{1/p}$ is the [Lp norm](../../../../../lp-norm.md).

For the final assertion we prove the required [Littlewood interpolation inequality](../../../../../littlewood-interpolation-inequality.md), rather than assuming it. Apply [Holder inequality](../../../../../holder-inequality.md) with conjugate exponents $3/2$ and $3$:

$$
\mathbb E|X|^2=\mathbb E\bigl(|X|^{2/3}|X|^{4/3}\bigr)
\leq(\mathbb E|X|)^{2/3}(\mathbb E|X|^4)^{1/3}.
$$

Raising to the power $3/2$ gives $\|X\|_2^3\leq\|X\|_1\|X\|_4^2$. The preceding [Lp norm](../../../../../lp-norm.md) estimate with $k=2$ says $\|X\|_4\leq2b$. Therefore

$$
\boxed{\|X\|_2^3\leq4b^2\|X\|_1}.
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
