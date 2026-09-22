<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Orient each [edge](../../../../../../edge-of-a-graph.md) both ways. A [unit flow](../../../../../../unit-flow.md) $j$ from $x$ to $y$ is antisymmetric, $j(u,v)=-j(v,u)$, with [divergence of a flow](../../../../../../divergence-of-a-flow.md) equal to $+1$ at $x$, $-1$ at $y$ and zero elsewhere. Its energy is

$$
\mathcal E_r(j)=\sum_{e\in E}r_ej(e)^2,
$$

where each unoriented [edge](../../../../../../edge-of-a-graph.md) is counted once. Put $c_e=1/r_e$. The electrical unit current is $i(u,v)=c_{uv}(V(u)-V(v))$, where the potential $V$ solves the [Kirchhoff node law](../../../../../../kirchhoff-node-law.md) with those source and sink divergences. Because $G$ is a [connected graph](../../../../../../connected-graph.md), this potential is unique up to an additive constant. The [effective resistance](../../../../../../effective-resistance.md) is the [electric potential difference](../../../../../../electric-potential-difference.md) needed for unit current,

$$
R(x,y)=V(x)-V(y).
$$

Discrete summation by parts gives $\mathcal E_r(i)=\sum_uV(u)\operatorname{div}i(u)=R(x,y)$.

The [Thomson principle](../../../../../../thomson-principle.md) says that this current minimizes energy among all [unit flows](../../../../../../unit-flow.md). Indeed write any other [unit flow](../../../../../../unit-flow.md) as $j=i+k$, where $\operatorname{div}k=0$. Then

$$
\sum_er_ei(e)k(e)=\sum_{e=(u,v)}(V(u)-V(v))k(u,v)=\sum_uV(u)\operatorname{div}k(u)=0.
$$

Consequently

$$
\mathcal E_r(j)=R(x,y)+\mathcal E_r(k)\ge R(x,y),\qquad
\boxed{R(x,y)=\min_{j\text{ unit flow }x\to y}\mathcal E_r(j).}
$$

This also proves uniqueness of the minimizing current.

If $r'_e\ge r_e$ for every [edge](../../../../../../edge-of-a-graph.md), then $\mathcal E_{r'}(j)\ge\mathcal E_r(j)$ for every admissible [flow](../../../../../../flow.md). The admissible set is unchanged, so taking its minimum proves the [Rayleigh monotonicity principle](../../../../../../rayleigh-monotonicity-principle.md):

$$
\boxed{R_{r'}(x,y)\ge R_r(x,y).}
$$

Deletion is the limiting operation $r_e\to\infty$: finite-energy [flows](../../../../../../flow.md) must then carry zero current on that [edge](../../../../../../edge-of-a-graph.md). If the terminals become disconnected, the [effective resistance](../../../../../../effective-resistance.md) is infinite.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
