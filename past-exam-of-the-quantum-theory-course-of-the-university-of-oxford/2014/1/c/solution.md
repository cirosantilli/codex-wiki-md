<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The initial [quantum state](../../../../quantum-state.md) is the [equal superposition of the first two box states](../../../../equal-superposition-of-the-first-two-box-states.md), $(\psi_1+\psi_2)/\sqrt2$. The [orthonormality](../../../../orthonormal-set.md) of the two [energy eigenstates](../../../../energy-eigenstate.md) makes its squared [norm](../../../../norm.md) equal to one. Their separate [stationary state](../../../../stationary-state.md) phases give

$$
\boxed{\Psi(x,t)=\frac1{\sqrt a}\left[\sin\frac{\pi x}{a}e^{-iE_1t/\hbar}+\sin\frac{2\pi x}{a}e^{-iE_2t/\hbar}\right].}
$$

Write $\Omega=(E_2-E_1)/\hbar=3\pi^2\hbar/(2ma^2)$. The [probability density](../../../../probability-density.md) is

$$
\rho(x,t)=\frac1a\left[\sin^2\frac{\pi x}a+\sin^2\frac{2\pi x}a+2\sin\frac{\pi x}a\sin\frac{2\pi x}a\cos\Omega t\right].
$$

Each squared sine integrates to $a/4$ on the left half. For the [quantum interference](../../../../quantum-interference.md) term, the product-to-sum identity gives

$$
\int_0^{a/2}\sin\frac{\pi x}a\sin\frac{2\pi x}a\,dx=\frac12\int_0^{a/2}\left(\cos\frac{\pi x}a-\cos\frac{3\pi x}a\right)dx=\frac{2a}{3\pi}.
$$

Hence the [Born rule](../../../../born-rule.md) gives

$$
\boxed{P_{\mathrm L}(t)=\int_0^{a/2}\rho(x,t)\,dx=\frac12+\frac4{3\pi}\cos\Omega t.}
$$

The [quantum interference](../../../../quantum-interference.md) moves probability between the halves even though each component separately is a [stationary state](../../../../stationary-state.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the quantum theory course of the University of Oxford](../../../split.md)
5. [Quantum theory course of the University of Oxford](../../../../quantum-theory-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
