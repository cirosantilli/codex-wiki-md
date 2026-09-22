<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [Lévy measure](../../../../../levy-measure.md) $K$ on the real line is a nonnegative [Borel measure](../../../../../borel-measure.md) satisfying

$$
K(\{0\})=0,\qquad \int_{\mathbb R}(1\wedge y^2)\,K(dy)<\infty.
$$

It records the intensity per unit time of jumps of a [Lévy process](../../../../../levy-process.md). Under the additional small-jump first-moment condition, the [uncompensated Lévy–Khintchine formula](../../../../../uncompensated-levy-khintchine-formula.md) is

$$
\mathbb E e^{iuX_t}=\exp\{t\psi(u)\},\qquad \psi(u)=ibu-\frac12\sigma^2u^2+\int_{\mathbb R\setminus\{0\}}(e^{iuy}-1)\,K(dy),
$$

where $b\in\mathbb R$ and $\sigma^2\ge0$. The integral is absolutely convergent: near zero its integrand has absolute value at most $|u||y|$, while outside a neighborhood of zero it is at most $2$ and $K$ has finite mass. If the usual compensated [Lévy–Khintchine formula](../../../../../levy-khintchine-formula.md) uses drift $\gamma$, this convention has $b=\gamma-\int_{|y|\le1}yK(dy)$.

A [Lévy process](../../../../../levy-process.md) starts at zero and has stationary [independent increments](../../../../../independent-increments.md) and stochastic continuity. Its [characteristic function](../../../../../characteristic-function.md) at time $t$ is $e^{t\psi(u)}$, with $\psi(0)=0$ and $\psi$ continuous. The given time-one [characteristic function](../../../../../characteristic-function.md) is strictly positive. It therefore has the unique continuous logarithm vanishing at zero,

$$
\psi(u)=-\log(1+u^2/2).
$$

Any other continuous exponent would differ by an integer multiple of $2\pi i$; continuity on the real line and the value at zero make that integer identically zero. This determines all increment laws. More explicitly, for $0=t_0<t_1<\cdots<t_m$,

$$
\mathbb E\exp\!\left(i\sum_{j=1}^m u_jX_{t_j}\right)=\exp\!\left\{\sum_{j=1}^m(t_j-t_{j-1})\psi\!\left(\sum_{k=j}^m u_k\right)\right\}.
$$

Thus it determines every [finite-dimensional distribution](../../../../../finite-dimensional-distribution.md). For the standard [càdlàg](../../../../../cadlag.md) version of a [Lévy process](../../../../../levy-process.md), coordinates at rational times determine the path, so these laws determine the entire process law on its canonical path space as well.

To find the [Lévy measure](../../../../../levy-measure.md), try the symmetric density $e^{-\alpha|y|}/|y|$. Its jump exponent is

$$
J_\alpha(u)=2\int_0^\infty\frac{\cos(uy)-1}{y}e^{-\alpha y}\,dy.
$$

Differentiation under the integral is justified by the integrable bound $2e^{-\alpha y}$. The elementary [Fourier sine transform](../../../../../fourier-sine-transform.md) gives

$$
J_\alpha'(u)=-2\int_0^\infty e^{-\alpha y}\sin(uy)\,dy=-\frac{2u}{\alpha^2+u^2}.
$$

Since $J_\alpha(0)=0$, integration in $u$ yields $J_\alpha(u)=-\log(1+u^2/\alpha^2)$. Choosing $\alpha=\sqrt2$ matches the prescribed exponent exactly. This is the [Lévy measure of a symmetric Laplace time-one law](../../../../../levy-measure-of-a-symmetric-laplace-time-one-law.md):

$$
\boxed{K(dy)=\frac{e^{-\sqrt2|y|}}{|y|}\mathbf1_{\{y\ne0\}}\,dy,\qquad b=0,\quad\sigma^2=0.}
$$

The candidate satisfies the [Lévy measure](../../../../../levy-measure.md) condition because its density is of order $1/|y|$ near zero and decays exponentially at infinity; moreover $\int_{|y|\le1}|y|K(dy)=2\int_0^1e^{-\sqrt2y}dy<\infty$. Uniqueness of the triplet in the [Lévy–Khintchine formula](../../../../../levy-khintchine-formula.md) proves that these are the required coefficients. The infinite mass near zero means infinitely many small jumps, not a Gaussian component; their total variation is finite on bounded time intervals because $\int(1\wedge|y|)K(dy)<\infty$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
