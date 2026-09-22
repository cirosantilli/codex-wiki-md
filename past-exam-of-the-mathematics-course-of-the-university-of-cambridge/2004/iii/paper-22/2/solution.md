<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Put $B=\partial M$ and let $v$ be the cone vertex. Specify the convention away from the Witt case: first take [intersection cohomology](../../../../../intersection-cohomology.md) to mean the [hypercohomology](../../../../../hypercohomology.md) of the [intersection complex](../../../../../intersection-complex.md) $IC_{\bar m}$, normalized in degree zero on the regular stratum. The [lower middle perversity](../../../../../lower-middle-perversity.md) at the vertex is $\bar m(2m+1)=m-1$. The standard local cone calculation for this convention says

$$
IH_{\bar m}^i(\widehat U)=\begin{cases}H^i(B;\mathbb Q),&i<m,\\0,&i\ge m,\end{cases}
$$

and restriction to $U\simeq B$ is the identity below the cutoff. Here this can also be read directly from the construction $IC_{\bar m}=\tau_{\le m-1}Rj_*\mathbb Q$, with $j:\widehat M\setminus\{v\}\hookrightarrow\widehat M$: punctured conical neighbourhoods retract onto $B$, and the truncation discards the degrees above $m-1$.

Define relative [intersection cohomology](../../../../../intersection-cohomology.md) as the [hypercohomology](../../../../../hypercohomology.md) of the homotopy fibre of restriction, namely $R\Gamma(\widehat M,\widehat U;IC)=\operatorname{Cone}(R\Gamma(\widehat M;IC)\to R\Gamma(\widehat U;IC))[-1]$. Restricting to the pair $(M,U)$ gives a map to the corresponding ordinary relative [cohomology](../../../../../cohomology-split.md), since $IC|_M=\mathbb Q_M$. The induced map of [exact triangles](../../../../../exact-triangle-in-a-derived-category.md) gives the requested [commutative diagram](../../../../../commutative-diagram.md):

$$
\begin{array}{ccccccccc}
\cdots\to&IH^i(\widehat M,\widehat U)&\to&IH^i(\widehat M)&\to&IH^i(\widehat U)&\to&IH^{i+1}(\widehat M,\widehat U)&\to\cdots\\
&\downarrow&&\downarrow&&\downarrow&&\downarrow&\\
\cdots\to&H^i(M,U)&\to&H^i(M)&\to&H^i(U)&\to&H^{i+1}(M,U)&\to\cdots .
\end{array}
$$

Both rows are [long exact cohomology sequences of a pair](../../../../../long-exact-cohomology-sequence-of-a-pair.md). Commutativity includes the [connecting homomorphisms](../../../../../connecting-homomorphism.md), because they arise from the same map of restriction cones, with a common sign convention. The relative vertical maps are isomorphisms: [excision](../../../../../excision-theorem.md) removes the common conical neighbourhood, leaving precisely the [manifold](../../../../../topological-manifold.md) pair outside it, where $IC$ is constant. Also the collar retracts onto $B$, so $H^*(M,U)\cong H^*(M,B)$.

The only possible nonmanifold stratum is $v$, with link $B$ of dimension $2m$. Since [intersection homology](../../../../../intersection-homology.md) of a [manifold](../../../../../topological-manifold.md) is ordinary homology, the exact necessary and sufficient condition is

$$
\boxed{\widehat M\text{ is Witt}\quad\Longleftrightarrow\quad H^m(B;\mathbb Q)=0.}
$$

The equivalence with the defining $H_m(B;\mathbb Q)=0$ follows from the [universal coefficient theorem for cohomology](../../../../../universal-coefficient-theorem-for-cohomology.md) over $\mathbb Q$. In the Witt case the cone restriction is an isomorphism through degree $m$, since both degree-$m$ groups are zero. Comparing the two exact rows, or applying the [Five lemma](../../../../../five-lemma.md) to each five-term segment, gives $IH^i(\widehat M)\cong H^i(M)$ for $i\le m$. For $i>m$, both $IH^{i-1}(\widehat U)$ and $IH^i(\widehat U)$ vanish, so the top row identifies the absolute group with the relative one. Hence

$$
\boxed{IH^i(\widehat M)\cong\begin{cases}H^i(M;\mathbb Q),&i\le m,\\H^i(M,B;\mathbb Q),&i>m.\end{cases}}
$$

Without the Witt hypothesis, comparison still gives $IH_{\bar m}^i(\widehat M)\cong H^i(M)$ for $i<m$. At degree $m$ the upper row reads

$$
H^{m-1}(B)\xrightarrow{\delta}H^m(M,B)\longrightarrow IH_{\bar m}^m(\widehat M)\longrightarrow0.
$$

The lower row identifies the quotient by $\operatorname{im}\delta$ with the image of the relative-to-absolute map. In higher degrees both cone terms vanish. Thus the full lower-middle Deligne answer is

$$
\boxed{IH_{\bar m}^i(\widehat M)\cong\begin{cases}H^i(M),&i<m,\\\operatorname{im}(H^m(M,B)\to H^m(M)),&i=m,\\H^i(M,B),&i>m.\end{cases}}
$$

For clarity, if $IH^i$ is instead defined as the linear dual of the lower-middle [intersection chains](../../../../../intersection-chains.md) of question 1, it corresponds to the complementary [upper middle perversity](../../../../../upper-middle-perversity.md) Deligne [sheaf](../../../../../sheaf-mathematics.md). Its cone group retains $H^m(B)$ as well. The same diagram then gives

$$
\boxed{IH_{\bar n}^i(\widehat M)\cong\begin{cases}H^i(M),&i\le m,\\\operatorname{im}(H^{m+1}(M,B)\to H^{m+1}(M)),&i=m+1,\\H^i(M,B),&i>m+1.\end{cases}}
$$

Equivalently the exceptional group is $H^{m+1}(M,B)/\operatorname{im}(H^m(B)\xrightarrow{\delta}H^{m+1}(M,B))$. These conventions agree under the stated Witt condition, explaining why that condition removes the ambiguity.

Take the solid [torus](../../../../../torus.md) $M=S^1\times D^2$, whose boundary is the two-dimensional [torus](../../../../../torus.md) $B=T^2$. Its ordinary [cohomology](../../../../../cohomology-split.md) is $H^0(M)=H^1(M)=\mathbb Q$, zero otherwise; [Poincare duality](../../../../../poincare-duality.md) for a [manifold](../../../../../topological-manifold.md) with boundary gives $H^2(M,B)=H^3(M,B)=\mathbb Q$ and all other relative groups zero. The lower-middle Deligne formula gives

$$
\boxed{\dim IH_{\bar m}^i(\widehat M)=(1,0,1,1)\quad\text{for }i=0,1,2,3.}
$$

Thus degrees one and two have different dimensions, so there can be no three-dimensional [Poincare duality](../../../../../poincare-duality.md). In the dual-lower-chain convention the dimensions are $(1,1,0,1)$, which likewise fail duality. Both computations exhibit the obstruction $H^1(T^2)=\mathbb Q^2\ne0$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
