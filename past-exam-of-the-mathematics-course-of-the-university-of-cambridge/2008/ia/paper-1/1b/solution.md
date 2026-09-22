<h1 id="1b/solution">Solution</h1>

↑ **Parent:** [1B](../1b.md)

[De Moivre's theorem](../../../../../de-moivre-s-theorem.md) says that, for a real angle $\theta$ and an integer $m$,

$$
(\cos\theta+i\sin\theta)^m=\cos(m\theta)+i\sin(m\theta).
$$

For a [complex number](../../../../../complex-number.md) $z=\rho(\cos\theta+i\sin\theta)$, the corresponding formula is $z^m=\rho^m[\cos(m\theta)+i\sin(m\theta)]$, with $z\ne0$ required for negative powers.

Put $q=e^{i\theta}$. If $\theta\notin2\pi\mathbb Z$, the [finite geometric series](../../../../../finite-geometric-series.md) gives

$$
S=\sum_{r=1}^nq^r=\frac{q-q^{n+1}}{1-q}.
$$

To extract the real part, multiply numerator and denominator by $1-q^{-1}$. The denominator becomes $2(1-\cos\theta)$, and the numerator is $q-1-q^{n+1}+q^n$. Thus this [finite trigonometric sum](../../../../../finite-trigonometric-sum.md) is

$$
\boxed{\sum_{r=1}^n\cos(r\theta)
=\frac{\cos(n\theta)-\cos((n+1)\theta)}{2(1-\cos\theta)}-\frac12.}
$$

At $\theta\in2\pi\mathbb Z$, the sum equals $n$; the printed quotient is undefined there, though its continuous limiting value is $n$.

Now take $\theta=2p\pi/(n+1)$ with $1\leq p\leq n$. This is not a multiple of $2\pi$, while $(n+1)\theta=2p\pi$ and $\cos(n\theta)=\cos(2p\pi-\theta)=\cos\theta$. Substitution gives

$$
\boxed{\sum_{r=1}^n\cos\left(\frac{2p\pi r}{n+1}\right)
=\frac{\cos\theta-1}{2(1-\cos\theta)}-\frac12=-1.}
$$

## ↑ Ancestors (10)

1. [1B](../1b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
