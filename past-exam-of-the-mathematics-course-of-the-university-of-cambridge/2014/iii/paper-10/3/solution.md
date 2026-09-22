<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

An [ordinary line](../../../../../ordinary-line.md) contains exactly two points of the configuration. We give a [cubic covering from few ordinary lines](../../../../../cubic-covering-from-few-ordinary-lines.md) by using [point-line duality](../../../../../point-line-duality.md), a defect count and cubic interpolation. Cubics may be reducible: a line with equation $L=0$ is contained in the cubic $L^3=0$, and a conic can be multiplied by a linear factor.

Pass to the [real projective plane](../../../../../real-projective-plane.md), which preserves collinearities and ordinary-line counts. If all points are collinear, one cubic already suffices. Otherwise dualize each point $p=[a:b:c]$ to the line $p^*:aX+bY+cZ=0$. The dual lines form an embedded graph $\Gamma$: its vertices are their intersections and its edges are the consecutive segments on each projective line. A vertex where $k$ dual lines meet has graph degree $2k$ and corresponds to a primal line containing $k$ points.

Let $t_k$ count vertices incident to exactly $k$ dual lines, and let $f_j$ count faces with $j$ sides. In particular $t_2<5n$. If $v,e,f$ are the graph's numbers of vertices, edges and faces, then

$$
v=\sum_{k\ge2}t_k,\qquad
e=\sum_{k\ge2}kt_k,\qquad
f=\sum_{j\ge3}f_j,\qquad
2e=\sum_{j\ge3}jf_j.
$$

The [Euler characteristic](../../../../../euler-characteristic.md) of the projective plane is one, so $v-e+f=1$. Substituting the counts gives the [Euler defect identity for a projective line arrangement](../../../../../euler-defect-identity-for-a-projective-line-arrangement.md)

$$
\boxed{t_2=3+\sum_{k\ge4}(k-3)t_k+\sum_{j\ge4}(j-3)f_j.}
$$

Thus both sums measuring departure from a degree-six triangular grid are $O(n)$.

Call an edge a [good dual-arrangement edge](../../../../../good-edge-of-a-dual-line-arrangement.md) if both endpoints have degree six and both adjacent faces are triangles; call it bad otherwise. Count all edge incidences at the defective vertices and faces. Since $k\le4(k-3)$ for $k\ge4$ and $j\le4(j-3)$ for $j\ge4$,

$$
\begin{aligned}
\#\{\text{bad edges}\}
&\le4t_2+2\sum_{k\ge4}kt_k+\sum_{j\ge4}jf_j\\
&\le4t_2+8\sum_{k\ge4}(k-3)t_k
+4\sum_{j\ge4}(j-3)f_j\\
&\le16t_2<80n.
\end{aligned}
$$

This controls actual bad edges, not merely the number of defective vertices.

Strengthen the local condition: an edge is a [safe dual-arrangement edge](../../../../../safe-edge-of-a-dual-line-arrangement.md) if every edge on every path of length at most two from either endpoint is good. The [bounded-radius propagation of edge defects](../../../../../bounded-radius-propagation-of-edge-defects.md) says that only $O(n)$ edges fail this test. Indeed, trace from an unsafe edge to the first bad edge. Every intervening edge is good, so the intermediate vertices have degree six. Reversing such paths offers only a bounded number of choices, at most a fixed constant times the bad-edge count. Every edge belongs to exactly one dual line, so the [pigeonhole principle](../../../../../pigeonhole-principle.md) gives a dual line $p^*$ containing only $O(1)$ unsafe edges.

The algebraic input is [cubic propagation along a triangular strip](../../../../../cubic-propagation-along-a-triangular-strip.md): a consecutive strip of safe edges on $p^*$ has all of its crossing dual lines represented by primal points on a single cubic. Here is the mechanism, rather than an appeal to the desired covering theorem. The triangles on either side extend two cells outward into three indexed line families. After dualizing back, their points $a_i,b_j,c_k$ satisfy collinearities whenever $i+j+k=0$. Adjacent three-by-three blocks are the [eight-point cubic completion for two triples of lines](../../../../../eight-point-cubic-completion-for-two-triples-of-lines.md) configuration. A nonzero homogeneous cubic can be fitted to nine starting points because its coefficient space has dimension ten; each successive block has eight points already on that cubic and forces its remaining point onto it. Continuing along the strip keeps every crossing point on the same cubic. One concrete seed is $a_{-1},a_0,a_1,a_2,b_{-3},b_{-2},b_{-1},c_1,c_2$. The first overlapping block forces $c_3$, the next forces $b_{-4}$, and the next forces $c_4$; another block then forces $a_{-2}$. Alternating these completion steps extends the $b$ and $c$ families for the full length of the strip.

For clarity, the completion fact has a short algebraic proof. Let $F=L_1L_2L_3$ and $G=M_1M_2M_3$, with the two line triples meeting in nine distinct points, and let a cubic $H$ vanish at all but $L_3\cap M_3$. On $L_1$, both $H$ and $G$ have the same three zeros, so $H-\lambda G$ is divisible by $L_1$ for a suitable scalar $\lambda$. Its quadratic quotient vanishes at the three intersections on $L_2$, hence is divisible by $L_2$. The remaining linear quotient vanishes at the two known intersections on $L_3$, hence is a multiple of $L_3$. Thus

$$
H=\lambda G+\mu F,
$$

which also vanishes at the ninth point. This is the line-triple case of the [Cayley-Bacharach theorem](../../../../../cayley-bacharach-theorem.md). In the strip construction, degree-six vertices and the two-cell neighbourhood ensure that the local nine points are distinct; the initial nine-point interpolation and repeated completion provide the required cubic.

It remains to account for every point, including defects and degeneracies. If some dual line has at most two distinct intersection vertices, all other dual lines pass through one of them. Dualizing back covers $P$ by at most two primal lines, hence by cubics, and we are done. Otherwise every dual line has at least three vertices, and the local strip construction applies.

On the chosen $p^*$, cut the cyclic edge sequence at its $b=O(1)$ unsafe edges, adding one arbitrary cut if necessary. There are at most $b+1$ safe runs, each covered by a cubic via the strip argument. Intersection vertices incident to cut or unsafe edges number at most $2b+2$. At each such exceptional vertex $w$, all crossing dual lines represent primal points on the single primal line $w^*$, which is itself contained in a cubic. Include one further cubic through $p$ if it has not already been covered. Every other primal point is accounted for by where its dual line intersects $p^*$. Therefore

$$
\boxed{P\subseteq\bigcup_{j=1}^{C}\gamma_j,\qquad
C\le(b+1)+(2b+2)+1=3b+4=O(1).}
$$

The absolute bound on $b$ comes from $t_2<5n$ and does not depend on the number of points. This completes the requested proof sketch.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
