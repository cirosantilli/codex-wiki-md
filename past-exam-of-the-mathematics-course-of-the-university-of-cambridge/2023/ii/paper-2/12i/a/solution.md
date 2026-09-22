<h1 id="12i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [one-time pad](../../../../../../one-time-pad.md) over the [finite additive group](../../../../../../finite-additive-group.md) $\mathbb Z_n$ uses a key $K$ that is [uniform](../../../../../../continuous-uniform-distribution.md) on $\mathbb Z_n$, [independent](../../../../../../independent-random-variables.md) of the plaintext $X$, as long as the plaintext, and never reused. Encryption and decryption are

$$
C=X+K\pmod n,
\qquad
X=C-K\pmod n.
$$

For [independent random variables](../../../../../../independent-random-variables.md) $X,Y$, [conditioning reduces entropy](../../../../../../conditioning-reduces-entropy.md) and translation by a known element of the [finite additive group](../../../../../../finite-additive-group.md) preserves entropy, so

$$
H(X+Y)\geq H(X+Y\mid Y)=H(X\mid Y)=H(X).
$$

Interchanging $X$ and $Y$ gives $H(X+Y)\geq H(Y)$, hence

$$
\boxed{H(X+Y)\geq\max\{H(X),H(Y)\}}.
$$

This is the [entropy of a sum of independent finite-group variables](../../../../../../entropy-of-a-sum-of-independent-finite-group-variables.md).

The result explains why adding [independent pad symbols](../../../../../../independent-random-variables.md) cannot reduce uncertainty. For a [uniform](../../../../../../continuous-uniform-distribution.md) pad, $X+K$ is itself uniform and is [independent](../../../../../../independent-random-variables.md) of $X$, which is the [perfect-secrecy property](../../../../../../perfect-secrecy.md). Independence is necessary: if $X$ is nonconstant and $Y=-X\pmod n$, then $X+Y=0$ is constant, so

$$
\boxed{H(X+Y)=0<H(X)=H(Y).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12I](../../12i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
