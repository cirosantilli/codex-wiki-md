<h1 id="4h/solution">Solution</h1>

↑ **Parent:** [4H](../4h.md)

The [identity theorem](../../../../../identity-theorem.md) can be expressed as the principle of isolated zeros: a [holomorphic function](../../../../../holomorphic-function.md) on a connected open set is either identically zero or has isolated zeros. Locally this follows from its [Taylor series](../../../../../taylor-series.md): at a zero of a function which is not locally zero, factor the first nonzero power, $f(z)=(z-z_0)^m h(z)$ with $h(z_0)\ne0$. Connectedness then rules out a nonempty open region of zeros unless the whole function vanishes.

Set $g(z)=\overline{f(\bar z)}$. This is [holomorphic](../../../../../complex-differentiability-at-a-point.md) on the punctured plane: reflecting and conjugating a local power series produces another power series. The absence of an [essential singularity](../../../../../essential-singularity.md) means that the singularity at zero is removable or a pole. Thus for some integer $m\geq0$, $z^m f(z)$ extends holomorphically across zero; the same is true of $z^m g(z)$. Their difference

$$
H(z)=z^m(f(z)-g(z))
$$

therefore extends to a [holomorphic function](../../../../../holomorphic-function.md) on all of $\mathbb C$. At every $1/n$, real-valuedness gives $H(1/n)=0$. These zeros accumulate at zero, which is now an interior point of the domain of $H$. The [identity theorem](../../../../../identity-theorem.md) forces $H\equiv0$. For $z\ne0$ we may divide by $z^m$, yielding

$$
\boxed{f(z)=\overline{f(\bar z)}.}
$$

The conjugation outside $f$ is essential. Also, applying the [identity theorem](../../../../../identity-theorem.md) directly on the punctured plane would be invalid: the accumulation point zero does not belong to that domain.

## ↑ Ancestors (10)

1. [4H](../4h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
