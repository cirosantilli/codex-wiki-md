<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use binary encoding $b(S)=\sum_{i\in S}2^{i-1}$ for [vertices](../../../../../vertex-graph-theory.md) of the [hypercube graph](../../../../../hypercube-graph.md), and write $I_m=\{S:b(S)<m\}$. Let $e(\mathcal A)$ count [edges](../../../../../edge-of-a-graph.md) with both endpoints in a family. The exact [edge-isoperimetric theorem for binary initial segments](../../../../../edge-isoperimetric-theorem-for-binary-initial-segments.md), due to Harper, Lindsey, Bernstein and Hart, is

$$
\boxed{e(\mathcal A)\le e(I_m)=\sum_{j=0}^{m-1}s_2(j),\qquad m=|\mathcal A|,}
$$

where $s_2(j)$ is the number of ones in the binary expansion. Equivalently,

$$
\boxed{|\partial_e\mathcal A|\ge nm-2\sum_{j=0}^{m-1}s_2(j).}
$$

The equality for $I_m$ follows by assigning each internal edge to its larger endpoint: each one-bit of that endpoint can be cleared, giving an earlier endpoint still in $I_m$. This is the exact extremal statement, stronger than the logarithmic entropy bound.

We prove it by induction on $n$. The case $n=1$ follows by checking sizes zero, one and two. Fix a coordinate $i$ and delete it from the two sections $\mathcal A_0,\mathcal A_1$. The edge count splits as

$$
e(\mathcal A)=e(\mathcal A_0)+e(\mathcal A_1)+|\mathcal A_0\cap\mathcal A_1|.
$$

Replace each section by a [binary initial segment](../../../../../binary-initial-segment.md) of the same size. By induction its internal [edges](../../../../../edge-of-a-graph.md) cannot decrease. The two replacement segments are nested, so their intersection size is the smaller section size, at least the previous intersection size. Thus this [section compression in binary order](../../../../../section-compression-in-binary-order.md) cannot decrease $e(\mathcal A)$.

Repeatedly perform any nontrivial section compression. The sum $\sum_{S\in\mathcal A}b(S)$ strictly decreases each time: in a fixed section, the original numerical order is exactly the numerical order after deleting its fixed coordinate. This nonnegative integer potential ensures termination at a family compressed in every coordinate section.

Classify such a terminal family. If an absent vertex $S$ precedes a present vertex $T$, they cannot agree in any coordinate, because their common section is compressed and its earlier vertex would then have to be present. Hence $T=[n]\setminus S$. There can be no vertex strictly between them: if present, it would also have to be the complement of $S$; if absent, it would have to be the complement of $T$. Thus they are consecutive complementary binary integers, forcing

$$
b(S)=2^{n-1}-1,\qquad b(T)=2^{n-1}.
$$

No other inversion is possible for the same reason. Therefore a terminal family is either a [binary initial segment](../../../../../binary-initial-segment.md) or the sole exceptional form

$$
\bigl(\mathcal P([n-1])\setminus\{[n-1]\}\bigr)\cup\{\{n\}\}.
$$

This exception has size $2^{n-1}$. For $n\ge2$, compared with the half-cube $I_{2^{n-1}}$, it removes a vertex of internal degree $n-1$ and adds a vertex joined only to the retained empty set. Its edge count is thus $e(I_{2^{n-1}})-(n-1)+1\le e(I_{2^{n-1}})$. The $n=1$ case was already handled. Since compression never decreased [edges](../../../../../edge-of-a-graph.md), every original family has at most the [initial segment](../../../../../initial-segment.md)'s edge count. This proves the theorem, including the exceptional terminal configuration rather than assuming all compressed families are [initial segments](../../../../../initial-segment.md).

For the remaining requests it is useful to obtain the [entropy proof of cube edge-isoperimetry](../../../../../entropy-proof-of-cube-edge-isoperimetry.md), including its equality cases. Inductively a family of size $m$ satisfies

$$
e(\mathcal A)\le\tfrac12m\log_2m.
$$

Indeed let the two sections have sizes $a\ge b\ge0$, $m=a+b>0$. Their internal [edges](../../../../../edge-of-a-graph.md) are bounded inductively and the crossing [edges](../../../../../edge-of-a-graph.md) are at most $b$, so

$$
\begin{aligned}
e(\mathcal A)&\le\tfrac12(a\log_2a+b\log_2b)+b\\
&=\tfrac12m\log_2m-\tfrac12mH_2(t)+mt,
\qquad t=b/m.
\end{aligned}
$$

Here $0\log_20=0$ and $H_2(t)=-t\log_2t-(1-t)\log_2(1-t)$ is the [binary entropy function](../../../../../binary-entropy-function.md). Its concavity and its endpoint values at zero and one-half give $H_2(t)\ge2t$ for $0\le t\le1/2$. This proves the bound, starting from the zero-dimensional cube.

Define the [isoperimetric number of a graph](../../../../../isoperimetric-number-of-a-graph.md) by

$$
i(G)=\min_{0<|A|\le|V(G)|/2}\frac{|\partial_eA|}{|A|}.
$$

Since every cube vertex has degree $n$, the internal-edge bound gives

$$
|\partial_eA|=n|A|-2e(A)\ge |A|\log_2\frac{2^n}{|A|}\ge|A|
$$

when $|A|\le2^{n-1}$. A coordinate half-cube has one crossing edge per vertex, attaining ratio one. Hence, for $n\ge1$,

$$
\boxed{i(Q_n)=1.}
$$

Now establish the [equality cases of entropy cube edge-isoperimetry](../../../../../equality-cases-of-entropy-cube-edge-isoperimetry.md). Strict concavity of $H_2$ makes $H_2(t)>2t$ for $0<t<1/2$. Equality in the internal-edge bound therefore requires either one section to be empty, or two equal-size sections. In the equal-size case equality in the crossing bound forces the sections to coincide; each section must also attain its inductive internal-edge bound. Induction gives exactly [coordinate subcubes](../../../../../face-of-the-boolean-hypercube.md): the empty-section case fixes the coordinate, and the coincident-section case frees it. Conversely every [coordinate subcube](../../../../../face-of-the-boolean-hypercube.md) attains that bound.

At size $m=2^{n-1}$, an [edge boundary](../../../../../edge-boundary-in-a-graph.md) of size $m$ means $e(A)=\tfrac12m(n-1)=\tfrac12m\log_2m$, so these equality cases apply. The subcube has dimension $n-1$ and fixes precisely one coordinate. Therefore

$$
\boxed{A=\{x\in\{0,1\}^n:x_i=\epsilon\},\quad i\in[n],\ \epsilon\in\{0,1\}.}
$$

These **$2n$ coordinate half-cubes are the only extremizers** of the requested size.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
