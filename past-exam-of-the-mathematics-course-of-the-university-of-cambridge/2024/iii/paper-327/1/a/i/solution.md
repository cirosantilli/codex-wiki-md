<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Schwartz space](../../../../../../../schwartz-space.md) on the [real line](../../../../../../../real-line.md) is

$$
\mathcal S(\mathbb R)
=\left\{\varphi\in C^\infty(\mathbb R):
p_{m,n}(\varphi)<\infty\text{ for every }m,n\in\mathbb N_0\right\},
\qquad
p_{m,n}(\varphi)=\sup_{x\in\mathbb R}|x^m\varphi^{(n)}(x)|.
$$

These [seminorms](../../../../../../../seminorm.md) define its [Fréchet space](../../../../../../../frechet-space.md) topology. The space of [tempered distributions](../../../../../../../tempered-distribution.md) is its [continuous dual space](../../../../../../../continuous-dual-space-split.md),

$$
\mathcal S'(\mathbb R)=\mathcal S(\mathbb R)^*.
$$

With the angular-frequency convention, the [Fourier transform](../../../../../../../fourier-transform.md) of a [Schwartz function](../../../../../../../schwartz-function.md) is

$$
\widehat\varphi(\lambda)
=\int_{\mathbb R}e^{-i\lambda x}\varphi(x)\,dx.
$$

It maps $\mathcal S$ continuously to itself. The transform of $u\in\mathcal S'$ is defined through the [dual pairing](../../../../../../../dual-pairing.md):

$$
\boxed{\langle\widehat u,\varphi\rangle
=\langle u,\widehat\varphi\rangle},
$$

up to the fixed reflection and $2\pi$ factor if the inverse-transform convention is used for the test function.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 327](../../../../paper-327-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
