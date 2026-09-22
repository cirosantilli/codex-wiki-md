<h1 id="b/6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $N=M_1\mathbin{\#}M_2$ and $A_i=M_i\setminus\operatorname{int}D_i$. Use open thickenings of the two pieces, whose intersection deformation retracts onto $S^{n-1}$. The [Mayer-Vietoris sequence](../../../../../mayer-vietoris-sequence.md) then has terms from $H_k(A_1)\oplus H_k(A_2)$ and $H_k(S^{n-1})$.

For $n\geq2$, the pieces and intersection are [connected](../../../../../connected-space.md). The map on $H_0$ from the intersection is $1\mapsto(1,-1)$ and is injective; it gives $H_0(N)=\mathbb Z$ and contributes no extra degree-one class. In intermediate degrees the [sphere](../../../../../sphere.md) has no homology, except potentially at $n-1$. At that degree its map to $H_{n-1}(A_1)\oplus H_{n-1}(A_2)$ is zero because each oriented boundary [sphere](../../../../../sphere.md) bounds the punctured piece's relative fundamental chain. Using $H_n(A_i)=0$, the top part of the sequence therefore gives $H_n(N)\cong\mathbb Z$ and $H_{n-1}(N)\cong H_{n-1}(A_1)\oplus H_{n-1}(A_2)$. The $H_0$ injection just noted handles the adjacent term when $n=2$.

Together with part (ii), the answer is

$$
\boxed{H_k(N;\mathbb Z)\cong\begin{cases}
\mathbb Z,&k=0\text{ or }k=n,\\
H_k(M_1;\mathbb Z)\oplus H_k(M_2;\mathbb Z),&0<k<n,\\
0,&k>n.
\end{cases}}
$$

For $n=1$, each [connected](../../../../../connected-space.md) [closed manifold](../../../../../closed-manifold.md) is a [circle](../../../../../circle.md) and each punctured piece is an interval. The intersection is $S^0$ with two components: its $H_0$ map to the two interval components has rank one and kernel $\mathbb Z$. Mayer-Vietoris gives $H_1(N)=H_0(N)=\mathbb Z$, so the same displayed formula holds, with no intermediate degrees. The usual [connected](../../../../../connected-space.md)-sum construction here uses positive dimension.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the topology and Groups and Algebraic Topology course of the University of Oxford](../../../../split.md)
6. [Topology and Groups and Algebraic Topology course of the University of Oxford](../../../../../topology-and-groups-and-algebraic-topology-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
