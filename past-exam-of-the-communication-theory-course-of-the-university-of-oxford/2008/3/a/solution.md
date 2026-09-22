<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Unique decipherability makes the map from $(X_1,\ldots,X_m)$ to the concatenated binary string $M$ [injective](../../../../injective-function.md). [Entropy](../../../../information-entropy-split.md) is unchanged by an [injective](../../../../injective-function.md) relabelling, and [memorylessness](../../../../memoryless-classical-information-source.md) gives [independence](../../../../independent-random-variables.md), hence

$$
H(M)=H(X_1,\ldots,X_m)=mH(X).
$$

Given $L=\ell$, the string has at most $2^\ell$ possibilities. The [entropy](../../../../information-entropy-split.md) bound for finite alphabets therefore gives $H(M\mid L=\ell)\le\ell$. Averaging,

$$
H(M\mid L)\le\mathbb EL=m\mathbb E|c(X)|.
$$

The random length cannot simply be discarded: it can also carry information. Let $\ell_{\max}$ be the maximum [codeword length](../../../../codeword-length.md), finite since the alphabet is finite. Since $L$ is a [function](../../../../function-split.md) of $M$ and takes at most $m\ell_{\max}+1$ values,

$$
mH(X)=H(L)+H(M\mid L)\le\log_2(m\ell_{\max}+1)+m\mathbb E|c(X)|.
$$

Divide by $m$ and let $m\to\infty$. This proves $\boxed{\mathbb E|c(X)|\ge H(X)}$. The conclusion also covers a deterministic source; the source's lowercase $x$ in its final [expectation](../../../../expected-value-split.md) denotes the random source letter.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the communication Theory course of the University of Oxford](../../../split.md)
5. [Communication Theory course of the University of Oxford](../../../../communication-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
