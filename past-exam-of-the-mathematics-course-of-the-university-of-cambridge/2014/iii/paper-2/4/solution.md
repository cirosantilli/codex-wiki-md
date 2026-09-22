<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The appropriate abstract object is a finite reduced [crystallographic root system](../../../../../crystallographic-root-system.md) $R$ in a real [inner product space](../../../../../inner-product-space.md) $E$. Its axioms are: $R$ is finite, spans $E$, and does not contain zero; for $\alpha\in R$, $R\cap\mathbb R\alpha=\{\alpha,-\alpha\}$; each [root reflection](../../../../../root-reflection.md)

$$
s_\alpha(v)=v-\frac{2(v,\alpha)}{(\alpha,\alpha)}\alpha
$$

permutes $R$; and every [Cartan integer](../../../../../cartan-integer.md) $n_{\alpha\beta}=2(\alpha,\beta)/(\beta,\beta)$ is an [integer](../../../../../integer.md). The restriction to a [reduced root system](../../../../../reduced-root-system.md) and crystallographic integrality distinguishes roots of complex [semisimple Lie algebras](../../../../../semisimple-lie-algebra-split.md) from more general reflection configurations.

For any two [roots of a root system](../../../../../root-of-a-root-system.md), the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives

$$
0\le n_{\alpha\beta}n_{\beta\alpha}=\frac{4(\alpha,\beta)^2}{(\alpha,\alpha)(\beta,\beta)}\le4.
$$

If the inner product is zero, both [Cartan integers](../../../../../cartan-integer.md) vanish. Otherwise their signs agree, and the absolute value of each is a positive [integer](../../../../../integer.md). Dividing their product by an integer of absolute value at least one proves

$$
\boxed{0\le|n_{\alpha\beta}|\le4.}
$$

For nonproportional roots the product is strictly less than four. In a [reduced root system](../../../../../reduced-root-system.md), proportional roots are just $\pm\alpha$ and have Cartan integers $\pm2$, so the printed bound is intentionally looser than the resulting bound of three.

A [fundamental system of a root system](../../../../../fundamental-system-of-a-root-system.md) is a [basis](../../../../../basis.md) $\Delta$ of $E$ made of roots, such that each root is an integer combination of $\Delta$ with either all coefficients nonnegative or all nonpositive. Its members are the [simple roots](../../../../../simple-root.md). Suppose distinct $\alpha,\beta\in\Delta$ had $n_{\alpha\beta}>0$. Then

$$
s_\beta(\alpha)=\alpha-n_{\alpha\beta}\beta\in R
$$

has a positive coefficient of $\alpha$ and a negative coefficient of $\beta$, contradicting the defining sign condition. Thus $n_{\alpha\beta}\le0$. Distinct [simple roots](../../../../../simple-root.md) are linearly independent, so their Cartan-integer product is strictly less than four. Combining integrality and the sign condition gives

$$
\boxed{n_{\alpha\beta}\in\{0,-1,-2,-3\}\quad(\alpha\ne\beta\text{ simple}).}
$$

Here **nonpositive** is the intended sense of the printed convention that includes zero among “negative” numbers; orthogonal simple roots really do give zero.

To form a [Dynkin diagram](../../../../../dynkin-diagram.md), place a vertex at each [simple root](../../../../../simple-root.md). Join two vertices by $n_{\alpha\beta}n_{\beta\alpha}$ bonds, hence zero, one, two or three. A multiple bond has an arrow toward the [short root](../../../../../short-root.md). Indeed $n_{\alpha\beta}/n_{\beta\alpha}=(\alpha,\alpha)/(\beta,\beta)$ determines the squared length ratio, and the diagram with the [Cartan matrix](../../../../../cartan-matrix.md) reconstructs the angles and relative lengths. A single bond joins equal-length roots.

The connected finite [Dynkin diagrams](../../../../../dynkin-diagram.md) are the following. The descriptions include bond multiplicities and arrow directions, so distinguish dual diagrams:

- [An Dynkin diagram](../../../../../an-dynkin-diagram.md), $A_n$ for $n\ge1$: a chain of $n$ vertices with only single bonds.
- [Bn Dynkin diagram and affine extension](../../../../../bn-dynkin-diagram-and-affine-extension.md), $B_n$ for $n\ge2$: a chain whose last bond is double, with its arrow toward the terminal short root; all earlier bonds are single. Only its finite diagram is used here.
- [Cn Dynkin diagram](../../../../../cn-dynkin-diagram.md), $C_n$ for $n\ge3$: the same chain with the double-bond arrow toward the penultimate short root and away from the terminal long root. $C_2$ and $B_2$ describe the same rank-two type after relabelling.
- [Dn Dynkin diagram](../../../../../dn-dynkin-diagram.md), $D_n$ for $n\ge4$: a simply laced tree with one trivalent vertex and arms of lengths $1,1,n-3$, counting edges.
- [En Dynkin diagram](../../../../../en-dynkin-diagram.md), $E_6,E_7,E_8$: simply laced trees with a trivalent vertex and arms of lengths respectively $(1,2,2)$, $(1,2,3)$, $(1,2,4)$.
- [F4 Dynkin diagram](../../../../../f4-dynkin-diagram.md), $F_4$: a chain of four vertices, with a double central bond and two single outer bonds. Two consecutive vertices are long and two are short; the arrow goes from the long pair toward the short pair.
- [G2 Dynkin diagram](../../../../../g2-dynkin-diagram.md), $G_2$: two vertices joined by a triple bond, with arrow toward the short root.

There are no other connected finite [Dynkin diagrams](../../../../../dynkin-diagram.md). Low-rank conventions also identify $B_1=C_1=A_1$ and $D_3=A_3$; $D_2$ is disconnected, so introduces no further connected type. Affine diagrams are outside this finite classification.

Finally suppose the underlying graph contained a cycle on $m\ge3$ distinct [simple roots](../../../../../simple-root.md) $\alpha_1,\ldots,\alpha_m$. Put $u_i=\alpha_i/\|\alpha_i\|$. Any bonded pair has

$$
(u_i,u_j)=-\frac12\sqrt{n_{\alpha_i\alpha_j}n_{\alpha_j\alpha_i}}\le-\frac12,
$$

and all other distinct pairs have nonpositive inner products. The cycle contributes at least $m$ bonded pairs, so

$$
\left\|\sum_{i=1}^m u_i\right\|^2=m+2\sum_{i<j}(u_i,u_j)\le m-m=0.
$$

But the [simple roots](../../../../../simple-root.md), and hence these normalized vectors, are linearly independent, making the displayed sum nonzero. Positive definiteness gives a contradiction. Thus **the underlying graph of a finite Dynkin diagram has no cycle**. This [acyclicity of a finite Dynkin diagram](../../../../../acyclicity-of-a-finite-dynkin-diagram.md) argument also excludes cycles with extra chords or multiple bonds; multiple bonds themselves are not treated as two-edge cycles.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
