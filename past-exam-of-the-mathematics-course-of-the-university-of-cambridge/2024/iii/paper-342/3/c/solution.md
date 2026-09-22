<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [group velocity](../../../../../../group-velocity.md) is $v_g=\hbar^{-1}\partial_k\varepsilon_k$. Since it is positive everywhere on the branch, every wave packet travels in the same direction: this is a [Chiral Majorana edge mode](../../../../../../chiral-majorana-edge-mode.md).

Near $k=0$, particle-hole symmetry gives $\varepsilon_k=\hbar vk+O(k^3)$. Let $c_k$ annihilate the positive-$k$ part of this branch. Particle-hole symmetry identifies $c_k^\dagger=c_{-k}$. Hence

$$
c(x)=\int\frac{dk}{2\pi}e^{ikx}c_k
$$

satisfies $c(x)^\dagger=c(x)$ and is a Majorana field. Fourier transforming the linear dispersion gives

$$
H^{(\rm lw)}=-i\hbar v\int dx\,c(x)\partial_xc(x).
$$

The continuum analogue of the real antisymmetric matrix $A$ is the real anti-self-adjoint differential kernel

$$
A(x,y)=-\hbar v\,\partial_x\delta(x-y),
$$

up to the normalization convention for the Majorana anticommutator.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 342](../../../paper-342-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
