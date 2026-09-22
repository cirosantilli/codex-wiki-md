<h1 id="9f/solution">Solution</h1>

↑ **Parent:** [9F](../9f.md)

The [expectation](../../../../../expected-value.md) of a complex random quantity is defined through its real and imaginary parts. Both $\cos X$ and $\sin X$ are bounded, so all expectations below exist. Expand the addition formulae and apply the [expectation of a product of independent random variables](../../../../../expectation-of-a-product-of-independent-random-variables.md) identity:

$$
\begin{aligned}
E\cos(X+Y)&=E\cos X\,E\cos Y-E\sin X\,E\sin Y,\\
E\sin(X+Y)&=E\sin X\,E\cos Y+E\cos X\,E\sin Y.
\end{aligned}
$$

Combining real and imaginary parts proves

$$
\boxed{E e^{i(X+Y)}=(E e^{iX})(E e^{iY}).}
$$

For the [simple symmetric random walk](../../../../../simple-symmetric-random-walk.md), write $W_n=\sum_{j=1}^n\xi_j$, with independent increments satisfying $P(\xi_j=1)=P(\xi_j=-1)=1/2$. The usual casino model uses these independent, or conditionally fair, increments. Their [characteristic function](../../../../../characteristic-function.md) is $(e^{iu}+e^{-iu})/2=\cos u$, so repeated factorization gives

$$
\boxed{\phi(u)=E e^{iuW_n}=(\cos u)^n.}
$$

This is real for real $u$. Equivalently, the [distribution](../../../../../distribution-mathematical-analysis.md) of $W_n$ is symmetric, making $E\sin(uW_n)=0$.

For any integer $k$, [Fourier orthogonality](../../../../../fourier-orthogonality.md) gives

$$
\frac1{2\pi}\int_{-\pi}^{\pi}e^{iuk}\,du=\mathbf1_{\{k=0\}}.
$$

The [random walk](../../../../../random-walk.md) has finite support, so we may interchange its finite [expectation](../../../../../expected-value.md) with this integral. Therefore

$$
P(W_n=0)=\frac1{2\pi}\int_{-\pi}^{\pi}(\cos u)^n\,du.
$$

For even $n$, evenness and reflection symmetry about $\pi/2$ reduce this to

$$
\boxed{P(W_n=0)=\frac2\pi\int_0^{\pi/2}(\cos u)^n\,du,\qquad \gamma=\frac2\pi.}
$$

For odd $n$, $W_n$ has odd parity and cannot be zero, so **$P(W_n=0)=0$**. As a separate combinatorial check, for $n=2m$ the return [probability](../../../../../probability.md) is $\binom{2m}{m}/2^{2m}$, since exactly $m$ positive increments are required.

## ↑ Ancestors (10)

1. [9F](../9f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
