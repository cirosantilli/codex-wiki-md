<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the uniform [probability measure](../../../../../../probability-measure.md) on the [symmetric group](../../../../../../symmetric-group.md) $S_n$ and the unnormalized [Hamming distance](../../../../../../hamming-distance.md)

$$
d_H(\sigma,\tau)=|\{j:\sigma(j)\ne\tau(j)\}|.
$$

Let $f:S_n\to\mathbb R$ have [Lipschitz constant](../../../../../../lipschitz-constant.md) $K>0$ for this distance. We will prove the one-sided [concentration inequalities](../../../../../../concentration-inequality.md)

$$
\boxed{\mathbb P(f-\mathbb Ef\geq t),\ \mathbb P(f-\mathbb Ef\leq-t)
\leq\exp\!\left(-\frac{t^2}{2nK^2}\right),\qquad t\geq0.}
$$

Consequently $\mathbb P(|f-\mathbb Ef|\geq t)\leq2e^{-t^2/(2nK^2)}$ for $t>0$. A zero [Lipschitz constant](../../../../../../lipschitz-constant.md) makes $f$ constant, so that case is immediate.

Let $\sigma$ be a uniform [permutation](../../../../../../permutation.md), reveal $\sigma(1),\ldots,\sigma(k)$ successively, and define the [Doob exposure martingale](../../../../../../doob-exposure-martingale.md)

$$
M_k=\mathbb E[f(\sigma)\mid\sigma(1),\ldots,\sigma(k)],\qquad
M_0=\mathbb Ef,\quad M_n=f(\sigma).
$$

Fix the first $k-1$ images. For an available value $a$, let $h(a)$ be the conditional mean when $\sigma(k)=a$. Given two available values $a,b$, left-composition with the [transposition](../../../../../../transposition-permutation.md) exchanging $a,b$ is a [bijection](../../../../../../bijection.md) from completions with next image $a$ to completions with next image $b$. It fixes the previously exposed images and changes exactly two coordinates of each complete [permutation](../../../../../../permutation.md). Since conditional completions are uniform, averaging the [Lipschitz condition](../../../../../../lipschitz-continuity.md) over this pairing gives $|h(a)-h(b)|\leq2K$.

Thus, conditionally on the first $k-1$ images, $M_k-M_{k-1}$ has mean zero and takes values in an interval of length at most $2K$. We need the range-length version of the [Hoeffding lemma](../../../../../../hoeffding-lemma.md): if a real [random variable](../../../../../../random-variable-split.md) $Z$ has mean zero and lies in an interval of length $\ell$, then

$$
\mathbb E e^{\lambda Z}\leq e^{\lambda^2\ell^2/8}\qquad(\lambda\in\mathbb R).
$$

Here is a proof. For $\psi(\lambda)=\log\mathbb E e^{\lambda Z}$, differentiation gives $\psi''(\lambda)=\operatorname{Var}_\lambda(Z)$ under the exponentially tilted [probability distribution](../../../../../../probability-distribution.md). Any distribution on an interval of length $\ell$ has [variance](../../../../../../variance-split.md) at most $\ell^2/4$, because its squared distance from the interval midpoint is at most $\ell^2/4$. Since $\psi(0)=\psi'(0)=0$, integrating this second-derivative bound gives the lemma for both signs of $\lambda$. The same argument holds for every conditional distribution.

Apply it conditionally to each [martingale difference](../../../../../../martingale-difference.md) and use the tower property of [conditional expectation](../../../../../../conditional-expectation.md) repeatedly:

$$
\mathbb E e^{\lambda(M_n-M_0)}\leq e^{n\lambda^2K^2/2}.
$$

The [exponential Markov bound](../../../../../../exponential-markov-bound.md) now gives, for $\lambda>0$,

$$
\mathbb P(M_n-M_0\geq t)\leq\exp(-\lambda t+n\lambda^2K^2/2).
$$

Choose $\lambda=t/(nK^2)$ to obtain the upper tail in the box, and apply the argument to $-f$ for the lower tail. This proves [concentration of Lipschitz functions on the symmetric group](../../../../../../concentration-of-lipschitz-functions-on-the-symmetric-group.md). Using only the bound $|M_k-M_{k-1}|\leq2K$ in the absolute-increment [Azuma-Hoeffding inequality](../../../../../../azuma-s-inequality.md) would lose a factor four in the exponent; the conditional range length is what yields the constant needed in part (ii).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
