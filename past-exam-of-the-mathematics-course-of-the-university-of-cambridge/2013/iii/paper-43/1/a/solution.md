<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix the [Minkowski metric](../../../../../../minkowski-metric.md) convention $\eta=\operatorname{diag}(1,-1,-1,-1)$ and the [Levi-Civita symbol](../../../../../../levi-civita-symbol.md) $\epsilon_{123}=1$. The antisymmetry of the [Lorentz algebra](../../../../../../lorentz-algebra.md) generators gives $M_{i0}=-K_i$ and the inverse relation $M_{ij}=\epsilon_{ijk}J_k$. Inserting one temporal index in each generator immediately yields

$$
[K_i,K_j]=-i\eta_{00}M_{ij}=-i\epsilon_{ijk}J_k.
$$

Two [Lorentz boosts](../../../../../../lorentz-boost.md) therefore generate a rotation through their [commutator](../../../../../../commutator.md); the minus sign distinguishes this algebra from the rotation algebra in four-dimensional Euclidean space.

For a spatial generator and a boost, the same [Lorentz algebra](../../../../../../lorentz-algebra.md) gives

$$
[M_{ab},M_{0j}]=i(\delta_{aj}K_b-\delta_{bj}K_a).
$$

Contracting with $\epsilon_{iab}/2$ gives

$$
[J_i,K_j]=\frac i2\epsilon_{iab}(\delta_{aj}K_b-\delta_{bj}K_a)
=i\epsilon_{ijk}K_k.
$$

Thus the three [Lorentz boosts](../../../../../../lorentz-boost.md) transform as a spatial vector under rotations.

Finally, the all-spatial bracket becomes

$$
[M_{ab},M_{cd}]
=i(-\delta_{bc}M_{ad}-\delta_{ad}M_{bc}+\delta_{bd}M_{ac}+\delta_{ac}M_{bd}).
$$

Use $M_{ab}=\epsilon_{abr}J_r$ in the double contraction with $\epsilon_{iab}\epsilon_{jcd}/4$. The epsilon contraction identity reduces it to $[J_i,J_j]=i\epsilon_{ijk}J_k$. One can check the sign directly: $J_1=M_{23}$ and $J_2=M_{31}$ give $[J_1,J_2]=iM_{12}=iJ_3$; cyclic permutations give the other nonzero brackets. The requested coefficients are

$$
\boxed{(A_1,B_1)=(-1,0),\qquad(A_2,B_2)=(0,1),\qquad(A_3,B_3)=(1,0).}
$$

These are [rotation and boost commutators with a fixed metric signature](../../../../../../rotation-and-boost-commutators-with-a-fixed-metric-signature.md). The PDF does not explicitly specify the signature. Keeping its generator convention but choosing $\eta=\operatorname{diag}(-1,1,1,1)$ reverses every displayed algebra coefficient: the pairs become $(1,0),(0,-1),(-1,0)$. More generally, if $s=\eta_{00}=\pm1$, the three nonzero coefficients are $A_1=-s$, $B_2=s$ and $A_3=s$. Specifying the [Minkowski metric](../../../../../../minkowski-metric.md) is therefore necessary to make the numerical signs unambiguous.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
