<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Give a vertex $S\subseteq[n]$ the binary value $\nu(S)=\sum_{i\in S}2^{i-1}$. The [binary order on the discrete cube](../../../../../binary-order-on-the-discrete-cube.md) orders vertices by increasing $\nu$; its initial segment $I_m$ consists of the values $0,\ldots,m-1$. Write $e(\mathcal A)$ for the number of cube edges whose two endpoints lie in $\mathcal A$, and $\partial_e\mathcal A$ for its external [edge boundary](../../../../../edge-boundary-in-a-graph.md). The degree sum identity is

$$
|\partial_e\mathcal A|=n|\mathcal A|-2e(\mathcal A).
$$

The **exact edge-isoperimetric inequality** is

$$
\boxed{|\partial_e\mathcal A|\geq nm-2\sum_{j=0}^{m-1}\operatorname{wt}(j),\qquad m=|\mathcal A|,}
$$

where $\operatorname{wt}(j)$ is the number of ones in the binary expansion of $j$. Equality is attained by $I_m$. Indeed, $I_m$ is a [down-set](../../../../../down-set.md), so every downward neighbour of each vertex is also present. Counting each internal edge at its upper endpoint gives $e(I_m)=\sum_{j<m}\operatorname{wt}(j)$. We prove the equivalent [edge-isoperimetric theorem for binary initial segments](../../../../../edge-isoperimetric-theorem-for-binary-initial-segments.md), $e(\mathcal A)\leq e(I_m)$, by [mathematical induction](../../../../../mathematical-induction.md) using [section compression in binary order](../../../../../section-compression-in-binary-order.md).

Fix a coordinate $i$ and write $\mathcal A_0,\mathcal A_1\subseteq Q_{n-1}$ for the two sections with coordinate $i$ absent or present, deleting that coordinate. Their inherited binary order is the binary order on the remaining coordinates. Replace each section by the [binary initial segment](../../../../../binary-initial-segment.md) of its own size. This preserves $|\mathcal A|$. The edges split into internal edges in the two sections and crossing edges, giving

$$
e(\mathcal A)=e(\mathcal A_0)+e(\mathcal A_1)+|\mathcal A_0\cap\mathcal A_1|.
$$

By the [mathematical induction](../../../../../mathematical-induction.md) hypothesis, the two section edge counts do not decrease. After compression, the sections are nested initial segments, so their intersection has the largest possible size, $\min\{|\mathcal A_0|,|\mathcal A_1|\}$. Thus **each section compression does not decrease the internal edge count**.

Apply these compressions repeatedly whenever one changes the family. The integer potential $\sum_{S\in\mathcal A}\nu(S)$ decreases strictly at every nontrivial step: within either fixed-coordinate section, the initial segment uniquely minimizes the sum of the vertex values among sets of the prescribed size. Therefore the process terminates with a family compressed in every section.

We need a small structural fact about [families compressed in every binary section](../../../../../families-compressed-in-every-binary-section.md). If such a family is not a [binary initial segment](../../../../../binary-initial-segment.md), choose a missing vertex $x$ and a present vertex $y$ with $\nu(x)<\nu(y)$. They cannot agree in any coordinate: in that coordinate's section, the compressed initial segment would contain $x$ whenever it contains $y$. Thus $y=[n]\setminus x$. The same argument applies to every inversion. There cannot be any vertex strictly between $x$ and $y$ in binary order: a present one would form an inversion with $x$, and a missing one would form an inversion with $y$, forcing it to be $y$ or $x$, respectively. Hence $\nu(y)=\nu(x)+1$. Together with $\nu(x)+\nu(y)=2^n-1$, this gives

$$
\nu(x)=2^{n-1}-1,\qquad \nu(y)=2^{n-1}.
$$

Every vertex below $x$ must be present, and every vertex above $y$ absent, by the same inversion argument. Therefore **the only possible exception to a [binary initial segment](../../../../../binary-initial-segment.md)** is

$$
\mathcal E_n=\left(\mathcal P([n-1])\setminus\{[n-1]\}\right)\cup\{\{n\}\},\qquad |\mathcal E_n|=2^{n-1}.
$$

For $n\geq2$, this replaces the top vertex of an $(n-1)$-dimensional [subcube](../../../../../face-of-the-boolean-hypercube.md) by the singleton $\{n\}$. Removing that vertex loses $n-1$ internal edges, and adding the singleton creates exactly one edge, to the empty set. Thus

$$
e(\mathcal E_n)=e(I_{2^{n-1}})-(n-2)\leq e(I_{2^{n-1}}).
$$

The dimensions $n=0,1$ are immediate. This finishes the [mathematical induction](../../../../../mathematical-induction.md): compression leads either to the desired initial segment or to an exception with no larger edge count. Hence the exact [edge-isoperimetric inequality in the discrete cube](../../../../../edge-isoperimetric-inequality-in-the-discrete-cube.md) holds, and **[binary initial segments](../../../../../binary-initial-segment.md) maximize the number of contained edges** at every size.

For the square-face assertion, let $f(\mathcal A)$ count the two-dimensional [cube faces](../../../../../face-of-the-boolean-hypercube.md) all of whose vertices are in $\mathcal A$. We use [mathematical induction](../../../../../mathematical-induction.md) again, now also using the edge theorem just proved. Faces lying wholly in one coordinate section contribute $f(\mathcal A_0)+f(\mathcal A_1)$. Every face crossing coordinate $i$ is determined by an edge lying in both sections, so

$$
f(\mathcal A)=f(\mathcal A_0)+f(\mathcal A_1)+e(\mathcal A_0\cap\mathcal A_1).
$$

Compress the two sections as before. Their internal face counts do not decrease by [mathematical induction](../../../../../mathematical-induction.md). Put $c=|\mathcal A_0\cap\mathcal A_1|$ and $b=\min\{|\mathcal A_0|,|\mathcal A_1|\}$. The edge theorem and nesting of [binary initial segments](../../../../../binary-initial-segment.md) give

$$
e(\mathcal A_0\cap\mathcal A_1)\leq e(I_c)\leq e(I_b).
$$

After compression, the intersection is precisely $I_b$. Thus **section compression does not decrease the face count either**. The same decreasing potential gives termination, and the same classification leaves only a [binary initial segment](../../../../../binary-initial-segment.md) or $\mathcal E_n$.

In the exceptional family, removing the top vertex loses $\binom{n-1}2$ square faces, one for each pair of downward coordinate directions. The added singleton lies in no square face, because it is the only vertex in its upper section. Consequently

$$
f(\mathcal E_n)=f(I_{2^{n-1}})-\binom{n-1}2\leq f(I_{2^{n-1}}).
$$

Dimensions below two have no square faces and start the [mathematical induction](../../../../../mathematical-induction.md). We have proved **that [binary initial segments](../../../../../binary-initial-segment.md) maximize contained square faces**:

$$
\boxed{f(\mathcal A)\leq f(I_{|\mathcal A|}).}
$$

For an explicit value, the [down-set](../../../../../down-set.md) property counts every face at its unique top vertex, giving

$$
\boxed{f(I_m)=\sum_{j=0}^{m-1}\binom{\operatorname{wt}(j)}2.}
$$

This establishes [binary initial segments maximize contained square faces](../../../../../binary-initial-segments-maximize-contained-square-faces.md) for arbitrary sizes, rather than only sizes that are powers of two.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 109](../../paper-109-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
