# Polynomial module from a linear operator

↑ **Parent:** [Module (mathematics)](module-mathematics.md)

A [linear operator](linear-operator.md) $T:V\to V$ on a [vector space](vector-space-split.md) over a [field](field.md) $k$ makes $V$ a [module](module-mathematics.md) over the [polynomial ring](polynomial-ring.md) $k[t]$: let $t$ act as $T$, let constants act as the original scalars, and define $p(t)\cdot v=p(T)v$. The identity $(pq)(T)=p(T)q(T)$ for [polynomials](polynomial-split.md) $p,q$ verifies the multiplication axiom. The [submodules](submodule.md) are precisely the [invariant subspaces](invariant-subspace.md) of $T$. This construction is described in [Keith Conrad's Introductory Notes on Modules, section 6](https://kconrad.math.uconn.edu/blurbs/linmultialg/moduleintro.pdf).

For a computed example, take $k=\mathbb Q$, $V=k^2$, and

$$
T=\begin{pmatrix}0&1\\0&0\end{pmatrix},\qquad e_1=(1,0),\qquad e_2=(0,1).
$$

Then $Te_2=e_1$, $Te_1=0$, and $T^2=0$. Consequently

$$
(2+3t+t^2)\cdot e_2=2e_2+3e_1=(3,2).
$$

Every $(a,b)$ equals $(b+at)\cdot e_2$. The [module homomorphism](module-homomorphism.md) $k[t]\to V$, $p\mapsto p(T)e_2$, is therefore [surjective](surjective-function.md), and its [kernel](kernel-of-a-linear-map-split.md) is the [ideal](ideal.md) $(t^2)$. It induces a [module isomorphism](module-isomorphism.md) $V\cong k[t]/(t^2)$. This is a [cyclic module](cyclic-module.md) and a [torsion module](torsion-module.md) over $k[t]$, since $t^2V=0$. Over $k$ it is a [free module](free-module.md) with [basis](basis.md) $(e_1,e_2)$ and has no nonzero [torsion elements of a module](torsion-element-of-a-module.md). Over $\mathbb Q$ its nonzero elements also have infinite additive [order of a group element](order-of-a-group-element.md). Changing scalars changes the questions one asks about the same addition law.

## ↑ Ancestors (7)

1. [Module (mathematics)](module-mathematics.md)
2. [Module theory](module-theory-split.md)
3. [Commutative algebra](commutative-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Torsion element of a module](torsion-element-of-a-module.md)
- [Torsion module](torsion-module.md)
