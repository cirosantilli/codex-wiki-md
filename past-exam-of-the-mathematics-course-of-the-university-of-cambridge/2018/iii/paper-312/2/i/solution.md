<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The background [Einstein-de Sitter universe](../../../../../../einstein-de-sitter-universe.md) satisfies $a'=\mathcal H a$ and $\mathcal H'=-\mathcal H^2/2$. Introduce $\mathcal F_n$ and $\mathcal G_n$ for the spatial [convolutions](../../../../../../convolution.md) in the [Fourier transform](../../../../../../fourier-transform.md) representation with kernels $F_n$ and $G_n$, respectively, so $\delta^{(n)}=a^n\mathcal F_n$ and $\theta^{(n)}=-\mathcal H a^n\mathcal G_n$. Differentiation gives

$$
(\delta^{(n)})'=n\mathcal H a^n\mathcal F_n,\qquad
(\theta^{(n)})'=-\left(n-\frac12\right)\mathcal H^2a^n\mathcal G_n.
$$

At first order the [cosmological continuity equation](../../../../../../cosmological-continuity-equation.md) yields $F_1-G_1=0$, while the [cosmological Euler equation](../../../../../../cosmological-euler-equation.md) gives $3F_1/2-3G_1/2=0$. The growing-mode normalization therefore gives $\boxed{G_1=F_1=1}$.

At second order, take the unsymmetrized order of the inputs printed in the paper. Matching the [alpha mode-coupling kernel](../../../../../../alpha-mode-coupling-kernel.md) and [beta mode-coupling kernel](../../../../../../beta-mode-coupling-kernel.md) terms gives

$$
2F_2-G_2=\alpha(q_1,q_2),\qquad
\frac52G_2-\frac32F_2=\beta(q_1,q_2).
$$

Hence

$$
F_2=\frac57\alpha+\frac27\beta,\qquad
G_2=\frac37\alpha+\frac47\beta.
$$

With the paper's unsymmetrized convention $\alpha=\beta=(q_1+q_2)/q_1$, one possible unsymmetrized representation is

$$
\boxed{F_2(q_1,q_2)=G_2(q_1,q_2)=\frac{q_1+q_2}{q_1}}.
$$

Only the symmetric part enters a [convolution](../../../../../../convolution.md) of two identical linear fields. Symmetrizing gives

$$
F_{2,s}=G_{2,s}=\frac12\left[\frac{q_1+q_2}{q_1}+\frac{q_1+q_2}{q_2}\right]
=\boxed{\frac{(q_1+q_2)^2}{2q_1q_2}}.
$$

This is the [one-dimensional cosmological density kernel](../../../../../../one-dimensional-cosmological-density-kernel.md). The physical symmetric one-dimensional Euler kernel is also $(q_1+q_2)^2/(2q_1q_2)$: symmetrizing the printed $\beta$ reproduces it, so its apparently different unsymmetrized form is not a contradiction. Unsymmetrized kernels themselves are not unique, since antisymmetric parts integrate to zero. Zero input momenta require the usual separate treatment of the homogeneous background.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
