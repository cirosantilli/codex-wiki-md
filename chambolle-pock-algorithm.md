<h1 id="chambolle-pock-algorithm">Chambolle–Pock algorithm</h1>

↑ **Parent:** [Convex optimization](convex-optimization-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chambolle–Pock_algorithm)

For a [saddle point](saddle-point.md) problem $\min_u\max_v\{F(u)+\langle Du,v\rangle-G(v)\}$, one update ordering is

$$
u^{k+1}=\operatorname{prox}_{\tau F}(u^k-\tau D^*v^k),\qquad v^{k+1}=\operatorname{prox}_{\sigma G}(v^k+\sigma D(2u^{k+1}-u^k)).
$$

The [proximal operators](proximal-operator.md) treat both nonsmooth convex terms, while the extrapolation $2u^{k+1}-u^k$ couples the primal and dual variables. The primal objective is $F(u)+G^*(Du)$, with $G^*$ the [convex conjugate](convex-conjugate.md). A dual-first ordering is obtained by exchanging roles; consistent indexing is needed when comparing the formulas.

**Table of contents**

- [Convergence of primal-dual hybrid gradient](convergence-of-primal-dual-hybrid-gradient.md)

## ↑ Ancestors (5)

1. [Convex optimization](convex-optimization-split.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-65/3/c/solution.md)
- [TGV divergence splitting](tgv-divergence-splitting.md)
