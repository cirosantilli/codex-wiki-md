<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use on $\widetilde H_m$ the inner product $(w,z)_1=(\nabla w,\nabla z)$. The map $F_m$ in the hint is continuous because it is a finite-dimensional polynomial map. Since the velocity $v=\nabla^\perp\Phi$ is divergence-free,

$$
\begin{aligned}
\nu(F_m(w),w)_1
&=-\nu\|\nabla w\|_2^2-\gamma\|w\|_2^2
-((v\mathbin\cdot\nabla)w,w)+(g,w)\\
&=-\nu\|\nabla w\|_2^2-\gamma\|w\|_2^2+(g,w).
\end{aligned}
$$

The [Poincaré inequality](../../../../../../../poincare-inequality.md) bounds $\|w\|_2\leq\mu_1^{-1/2}\|\nabla w\|_2$. Thus $(F_m(w),w)_1<0$ on every $H^1$ sphere whose radius is larger than $\|g\|_2/(\nu\sqrt{\mu_1})$. The [Brouwer inward-pointing zero lemma](../../../../../../../brouwer-inward-pointing-zero-lemma.md) supplies $w_\ast$ inside that sphere with $F_m(w_\ast)=0$.

Set $\omega_m=w_\ast$, solve $-\Delta\Psi_m=\omega_m$ in $\widetilde H_m$, and put $u_m=\nabla^\perp\Psi_m$. Expanding $F_m(w_\ast)=0$ gives exactly the first equation of the Galerkin system, so $(\omega_m,\Psi_m,u_m)$ is a solution.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Paper 359](../../../../paper-359-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
