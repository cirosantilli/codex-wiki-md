<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [highest root](../../../../highest-root.md) of the [D5 root system](../../../../d5-root-system.md) in our numbering is $\theta=e_1+e_2=\alpha_1+2\alpha_2+2\alpha_3+\alpha_4+\alpha_5$. Adjoin $\alpha_0=-\theta$. The [Extended Dynkin diagram](../../../../extended-dynkin-diagram.md) has an extra bond $0-2$. Deleting node $2$ leaves the two isolated nodes $0,1$ and the chain $4-3-5$, hence the [root subsystem](../../../../root-subsystem.md) $A_1\oplus A_1\oplus A_3$.

This is a [maximal Lie subalgebra](../../../../maximal-lie-subalgebra.md), not merely a full-rank [Lie subalgebra](../../../../lie-subalgebra.md). In the orthogonal realization it is $\mathfrak{so}(4)\oplus\mathfrak{so}(6)\subset\mathfrak{so}(10)$, acting on a $4+6$ decomposition. The remaining off-diagonal part transforms as the irreducible [tensor product representation](../../../../tensor-product-of-group-representations.md) $(\mathbf4,\mathbf6)$ of dimension $24$. Any intermediate [Lie subalgebra](../../../../lie-subalgebra.md) containing one nonzero vector in that complement must contain the entire complement, because this [representation](../../../../group-representation.md) is [irreducible](../../../../irreducible-representation.md), and hence all $6+15+24=45$ dimensions. This proves maximality.

To apply the supplied projection, write a [D5 root system](../../../../d5-root-system.md) [weight](../../../../weight-representation-theory.md) as the column $w=(a,b,c,d,e)^T$ of [Dynkin labels](../../../../dynkin-label.md). Then

$$
Pw=(c+d+e,\ c,\ a+b+c+e,\ b+c+d,\ -a-b-c-d)^T.
$$

For example, the [highest weight](../../../../highest-weight-of-a-representation.md) $w=(0,0,0,0,1)^T$ maps to $(1,0;1,0,0)^T$, and $w=(-1,0,1,-1,0)^T$ maps to $(0,1;0,0,1)^T$. Applying the same expression to all sixteen [weights](../../../../weight-representation-theory.md) in [solution](../b/solution.md) gives exactly

$$
\{(\epsilon,0;f):\epsilon=\pm1,\ f\in F\}
\ \cup\ 
\{(0,\epsilon;\bar f):\epsilon=\pm1,\ \bar f\in\overline F\},
$$

where $F$ and $\overline F$ are the four-element [weight systems](../../../../weight-system.md) in [solution](../a/solution.md). Each set has eight distinct [weights](../../../../weight-representation-theory.md), each of multiplicity one. Since an $A_1$ doublet has [weights](../../../../weight-representation-theory.md) $\pm1$ and an $A_1$ singlet has [weight](../../../../weight-representation-theory.md) zero, the [branching of a representation](../../../../branching-of-a-representation.md) is

$$
\boxed{\mathbf{16}\longrightarrow R=(\mathbf2,\mathbf1,\mathbf4)\oplus(\mathbf1,\mathbf2,\overline{\mathbf4}).}
$$

The [highest weights](../../../../highest-weight-of-a-representation.md) of these two summands are $(1,0;1,0,0)$ and $(0,1;0,0,1)$, and $2\cdot1\cdot4+1\cdot2\cdot4=16$ checks the dimensions. Here $SU(2)\times SU(2)\times SU(4)$ is the convenient covering [group](../../../../group-split.md); its image inside $\operatorname{Spin}(10)$ has a common $\mathbb Z_2$ central identification. Both summands are trivial on $(-I_2,-I_2,-I_4)$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../d/solution.md)
