<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Expand around the $+z$ polarized [ground state](../../../../ground-state.md). With $n_j=a_j^\dagger a_j$ fixed as $S\to\infty$, the [Holstein–Primakoff transformation](../../../../holstein-primakoff-transformation.md) gives $S_j^+=\sqrt{2S}a_j+O(S^{-1/2})$, $S_j^-=\sqrt{2S}a_j^\dagger+O(S^{-1/2})$ and $S_j^z=S-n_j$. The longitudinal exchange contributes

$$
-J(1+u)\sum_j(S-n_j)(S-n_{j+1})=-LJ(1+u)S^2+2JS(1+u)\sum_jn_j+O(S^0).
$$

Use

$$
\begin{aligned}
S_j^xS_{j+1}^x+S_j^yS_{j+1}^y&=\tfrac12(S_j^+S_{j+1}^-+S_j^-S_{j+1}^+),\\
(\mathbf S_j\times\mathbf S_{j+1})_z&=\tfrac{i}{2}(S_j^+S_{j+1}^--S_j^-S_{j+1}^+).
\end{aligned}
$$

The transverse exchange then gives $-JS(a_{j+1}^\dagger a_j+a_j^\dagger a_{j+1})$, and the [Dzyaloshinskii-Moriya interaction](../../../../antisymmetric-exchange.md) gives $-iDS(a_{j+1}^\dagger a_j-a_j^\dagger a_{j+1})$. Discarding the constant $-LJ(1+u)S^2$ and all $O(S^0)$ interactions yields

$$
\boxed{H_{\rm LSW}=\sum_j\left[Aa_{j+1}^\dagger a_j+A^*a_j^\dagger a_{j+1}+Bn_j\right],\quad A=-S(J+iD),\quad B=2JS(1+u).}
$$

Here [periodic boundary conditions](../../../../periodic-boundary-conditions.md) make each $n_j$ occur twice in the longitudinal sum. The approximation is the [linear spin-wave approximation](../../../../linear-spin-wave-approximation.md), controlled by small local [magnon](../../../../magnon.md) occupation compared with $S$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../d/solution.md)
