# End-to-end distance of a worm-like chain

↑ **Parent:** [Worm-like chain](worm-like-chain.md)

For a free three-dimensional [worm-like chain](worm-like-chain.md) with contour length $L$ and [persistence length](persistence-length.md) $\ell_p$, the unit-tangent correlation is $\langle\mathbf t(s)\cdot\mathbf t(s')\rangle=e^{-|s-s'|/\ell_p}$. Since $\mathbf R=\int_0^L\mathbf t(s)\,ds$, integrating this correlation gives

$$
\langle R^2\rangle=2\int_0^L(L-u)e^{-u/\ell_p}\,du
=2\ell_pL-2\ell_p^2(1-e^{-L/\ell_p}).
$$

For $L\gg\ell_p$, the leading term is $2\ell_pL$, the [ideal chain](ideal-chain.md) law with [Kuhn length](kuhn-length.md) $2\ell_p$. For $L\ll\ell_p$, a [Taylor series](taylor-series.md) gives $\langle R^2\rangle=L^2-L^3/(3\ell_p)+O(L^4/\ell_p^2)$, approaching a rigid rod. This ideal semiflexible-chain model omits long-range [excluded volume](excluded-volume.md); sufficiently long dilute chains in a [good solvent](good-solvent.md) can cross over to swollen-chain statistics.

## ↑ Ancestors (6)

1. [Worm-like chain](worm-like-chain.md)
2. [Biopolymer mechanics](biopolymer-mechanics.md)
3. [Mathematical biology](mathematical-biology-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2012/paper-1/1/b/solution.md)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2016/paper-1/4/solution.md)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2018/section-b/b4/solution.md)
