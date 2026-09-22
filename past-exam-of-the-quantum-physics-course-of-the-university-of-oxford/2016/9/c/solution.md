<h1 id="9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [linear confinement correction to Coulomb bound states](../../../../linear-confinement-correction-to-coulomb-bound-states.md) uses $H'=br$, and its [first-order energy correction](../../../../first-order-energy-correction.md) in a normalized Coulomb [eigenstate](../../../../eigenstate.md) is $b\langle r\rangle$. Replace $a_0$ by $a_q$ in the [hydrogen](../../../../hydrogen.md) [wavefunctions](../../../../wave-function-split.md). The normalized [spherical harmonics](../../../../spherical-harmonic.md) remove the angular [integral](../../../../integral-split.md), leaving

$$
\langle r\rangle_{nl}=\int_0^\infty r^3|R_{nl}(r)|^2\,dr.
$$

For $1s$, the [integral](../../../../integral-split.md) of $r^3e^{-2r/a_q}$ yields

$$
\langle r\rangle_{1s}=\frac4{a_q^3}\frac{3!}{(2/a_q)^4}=\frac32a_q.
$$

For $2s$, put $u=r/a_q$ and square the full radial [polynomial](../../../../polynomial-split.md), including its cross term:

$$
\langle r\rangle_{2s}=\frac{a_q}{2}\int_0^\infty u^3\left(1-u+\frac{u^2}4\right)e^{-u}du
=\frac{a_q}{2}\left(3!-4!+\frac{5!}4\right)=6a_q.
$$

For $2p$, the same calculation gives

$$
\langle r\rangle_{2p}=\frac{a_q}{24}\int_0^\infty u^5e^{-u}du=5a_q.
$$

Consequently the first two Coulomb levels become, to first order,

$$
\boxed{\begin{aligned}
E_{1s}&=-\frac{m_qa^2}{4\hbar^2}+\frac32ba_q+O(b^2),\\
E_{2s}&=-\frac{m_qa^2}{16\hbar^2}+6ba_q+O(b^2),\\
E_{2p,m}&=-\frac{m_qa^2}{16\hbar^2}+5ba_q+O(b^2),\qquad m=-1,0,1.
\end{aligned}}
$$

Thus the second level splits into a singlet orbital level and a triply degenerate orbital level, with $E_{2s}-E_{2p}=ba_q+O(b^2)$. For the confining sign $b>0$, $2p$ lies lower than $2s$: its smaller mean radius gives the smaller positive correction. The expansion assumes these corrections and the induced couplings to other principal shells are small compared with the relevant Coulomb [energy](../../../../energy-split.md) gaps; $ba_q^2/a\ll1$ is the governing small parameter for fixed low $n$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [9](../../9.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the quantum physics course of the University of Oxford](../../../split.md)
5. [Quantum physics course of the University of Oxford](../../../../quantum-physics-course-of-the-university-of-oxford.md)
6. [Year 2 of the physics course of the University of Oxford](../../../../year-2-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
