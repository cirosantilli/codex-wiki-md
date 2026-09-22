<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Normalize the ring modes as $\varphi_j(x)=L^{-1/2}e^{ik_jx}$, with distinct $k_j=2\pi\ell_j/L$ and integers $\ell_j$. Inserting $\hat\psi(x)=\varphi_1(x)a_1+\varphi_2(x)a_2$ into the [contact interaction](../../../../contact-interaction-quantum-mechanics.md) gives

$$
H_{\rm int}=\frac g2\sum_{i,j,k,l=1}^2 I_{ijkl}a_i^\dagger a_j^\dagger a_k a_l,
\qquad I_{ijkl}=\int_0^L\varphi_i^*\varphi_j^*\varphi_k\varphi_l\,dx.
$$

[Orthogonality](../../../../orthogonal-vectors.md) makes $I_{ijkl}=1/L$ when $k_i+k_j=k_k+k_l$, and zero otherwise: this is [momentum conservation](../../../../momentum-conservation.md) in the projected [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md). There is one all-mode-1 term, one all-mode-2 term, and four mixed terms with one particle in each mode. A pair conversion between distinct ring modes would require $2k_1=2k_2$ and therefore vanishes.

Using $a_j^{\dagger2}a_j^2=n_j(n_j-1)$ and $a_1^\dagger a_2^\dagger a_1a_2=n_1n_2$ yields the [contact interaction between two ring modes](../../../../contact-interaction-between-two-ring-modes.md),

$$
\boxed{H_{\rm int}=\frac{g}{2L}\left[n_1(n_1-1)+n_2(n_2-1)+4n_1n_2\right],\qquad
\alpha=\beta=\frac g{2L},\quad\gamma=\frac{2g}{L}.}
$$

The factor four comes from two independent choices of ordering for the [creation operators](../../../../creation-operator.md) and [annihilation operators](../../../../annihilation-operator.md). This is the two-mode projected model; a full ring [contact interaction](../../../../contact-interaction-quantum-mechanics.md) can also scatter particles into other modes while conserving total [momentum](../../../../momentum-split.md).

## ↑ Ancestors (14)

1. [B](../b.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the theoretical physics II course of the University of Cambridge](../../../split.md)
5. [Theoretical Physics II course of the University of Cambridge](../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
6. [Theoretical Physics course of the University of Cambridge](../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
