<h1 id="9e/solution">Solution</h1>

↑ **Parent:** [9E](../9e.md)

The [Bolzano-Weierstrass theorem](../../../../../bolzano-weierstrass-theorem.md) states that every [bounded sequence](../../../../../bounded-sequence.md) of real numbers has a [convergent subsequence](../../../../../convergent-subsequence.md). We first use it to show that a [continuous function](../../../../../continuous-function.md) on $[a,b]$ is bounded above. Otherwise, choose $x_n\in[a,b]$ with $f(x_n)>n$. A convergent subsequence $x_{n_k}\to c$ exists, with $c\in[a,b]$ because the interval is closed. [Continuity](../../../../../continuous-function.md) would give $f(x_{n_k})\to f(c)$, contradicting $f(x_{n_k})>n_k\to\infty$.

Let $L=\sup\{f(x):x\in[a,b]\}$, which is finite. By the definition of [supremum](../../../../../supremum.md), there are $y_n\in[a,b]$ with $L-1/n<f(y_n)\le L$. Another application of the [Bolzano-Weierstrass theorem](../../../../../bolzano-weierstrass-theorem.md) gives a subsequence $y_{n_k}\to c\in[a,b]$. By [continuity](../../../../../continuous-function.md),

$$
f(c)=\lim_{k\to\infty}f(y_{n_k})=L.
$$

Thus **the supremum is actually attained**:

$$
\boxed{\exists c\in[a,b]\ \forall x\in[a,b]:\ f(x)\le f(c).}
$$

This proves the maximum part of the [extreme value theorem](../../../../../extreme-value-theorem.md) from sequential compactness rather than assuming it.

Now suppose $f''<0$ on $\mathbb R$. Applying the [mean value theorem](../../../../../mean-value-theorem.md) to $f'$ shows that $f'$ is strictly decreasing. At a [local maximum](../../../../../local-maximum.md) of a [differentiable function](../../../../../differentiable-function.md), the left difference quotients are nonnegative and the right difference quotients are nonpositive; existence of the derivative forces $f'=0$. A strictly decreasing function has at most one zero. Therefore

$$
\boxed{f''<0\ \Longrightarrow\ \text{at most one local maximum}.}
$$

If that zero exists, $f'$ is positive to its left and negative to its right, so the local maximum is also a [global maximum](../../../../../global-maximum.md).

For the uniform bound by $K<0$, define

$$
h(x)=f'(x)-Kx.
$$

Its derivative is $h'(x)=f''(x)-K<0$, so $h$ is strictly decreasing by the [mean value theorem](../../../../../mean-value-theorem.md). Comparing with $h(0)=f'(0)$ gives

$$
\begin{cases}
f'(x)<f'(0)+Kx,&x>0,\\
f'(x)>f'(0)+Kx,&x<0.
\end{cases}
$$

Because $K<0$, this makes $f'$ negative at sufficiently large positive $x$ and positive at sufficiently large negative $x$. The function $f'$ is continuous, since it is differentiable; the [intermediate value theorem](../../../../../intermediate-value-theorem.md) supplies a zero $c$ between such points. Its strict decrease makes this zero unique. Again using the [mean value theorem](../../../../../mean-value-theorem.md) for $f$, the derivative signs imply that $f$ increases up to $c$ and decreases after $c$:

$$
\boxed{f''(x)<K<0\ \text{for all }x
\ \Longrightarrow\ f\text{ has a unique global maximum}.}
$$

This illustrates [uniform negative curvature and global maximization](../../../../../uniform-negative-curvature-and-global-maximization.md).

Merely requiring $f''<0$ does not force existence. Take

$$
f(x)=-e^{-x}.
$$

Then $f'(x)=e^{-x}>0$ and $f''(x)=-e^{-x}<0$, but $f$ is strictly increasing, approaches $0$ as $x\to+\infty$, and never equals $0$. **The answer to the final question is no**, even for a function bounded above:

$$
\boxed{\sup_{\mathbb R}(-e^{-x})=0\quad\text{and the supremum is not attained}.}
$$

The stronger uniform curvature assumption prevents this behaviour. Here $f''(x)\to0$ at the end where the supremum is approached, so no uniform negative bound of that kind is available.

## ↑ Ancestors (10)

1. [9E](../9e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
