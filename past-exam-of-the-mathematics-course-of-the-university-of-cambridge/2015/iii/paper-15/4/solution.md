<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**Cells and attaching maps.** Regard $\mathbb{RP}^k$ as the lines in $\mathbb R^{k+1}$ and include $\mathbb{RP}^{k-1}$ as the lines whose last coordinate is zero. Its complement consists of lines with a unique representative $(x_1,\ldots,x_k,1)$, and is therefore an open $k$-cell. Inductively this makes [Real projective space](../../../../../real-projective-space.md) a [CW complex](../../../../../cw-complex.md) with one cell in each dimension from zero to $n$.

A characteristic map is obtained from the northern closed hemisphere of $S^k$: send a unit vector to the line it spans. Its interior maps homeomorphically onto the open cell, while its equator has the antipodal identification. Thus the $k$-cell is attached by the quotient map

$$
S^{k-1}\longrightarrow \mathbb{RP}^{k-1},\qquad x\longmapsto[x],
$$

which is the antipodal two-sheeted covering. This includes the two endpoints of the one-cell attaching to the zero-cell.

The [cellular chain complex](../../../../../cellular-chain-complex.md) has $C_k^{\mathrm{cell}}=\mathbb Z$ for $0\leq k\leq n$ and zero otherwise. To compute its differential, follow the attaching map by collapse of the $(k-2)$-skeleton. The resulting map to $\mathbb{RP}^{k-1}/\mathbb{RP}^{k-2}\cong S^{k-1}$ has two local contributions. They differ by the [mapping degree](../../../../../degree-of-a-continuous-mapping.md) $(-1)^k$ of the [antipodal map](../../../../../antipodal-map.md) on $S^{k-1}$. With compatible cell orientations,

$$
\boxed{d_k=1+(-1)^k=
\begin{cases}2,&k\text{ even},\\0,&k\text{ odd}.\end{cases}}
$$

For $k=1$ the two oriented endpoints cancel, giving the same formula. Consecutive differentials compose to zero, as required.

**The mod-two cup products.** Modulo two every cellular differential vanishes, so [cellular cohomology](../../../../../cellular-cohomology.md) gives a one-dimensional group in each degree $0,\ldots,n$. Let $a\in H^1(\mathbb{RP}^n;\mathbb F_2)$ be the [Poincare dual](../../../../../poincare-dual.md) of a projective hyperplane. This class is nonzero: a projective line transverse to that hyperplane meets it once. Intersecting $j$ generic projective hyperplanes produces $\mathbb{RP}^{n-j}$, and the [cup product](../../../../../cup-product.md) of their [Poincare duals](../../../../../poincare-dual.md) is the [Poincare dual](../../../../../poincare-dual.md) of that intersection. In particular, $a^n$ evaluates to one on the mod-two [fundamental class](../../../../../fundamental-class.md). Therefore every $a^j$, $0\leq j\leq n$, is nonzero, since otherwise multiplying it by $a^{n-j}$ would contradict $a^n\ne0$. Dimension makes $a^{n+1}=0$. The [mod-two cohomology ring of real projective space](../../../../../mod-two-cohomology-ring-of-real-projective-space.md) is

$$
\boxed{H^*(\mathbb{RP}^n;\mathbb F_2)
\cong\mathbb F_2[a]/(a^{n+1}),\qquad |a|=1.}
$$

For $n=0$ this simply means the cohomology of a point.

**The product with integral coefficients.** The final product's coefficients are unstated; take $\mathbb Z$ as the default. Dualizing the [cellular chain complex](../../../../../cellular-chain-complex.md) above gives

$$
\begin{aligned}
&H^*(\mathbb{RP}^2;\mathbb Z):\quad H^0=\mathbb Z,\ H^2=\mathbb Z/2,\\
&H^*(\mathbb{RP}^3;\mathbb Z):\quad H^0=\mathbb Z,\ H^2=\mathbb Z/2,\ H^3=\mathbb Z,\\
&H^*(\mathbb{RP}^4;\mathbb Z):\quad H^0=\mathbb Z,\ H^2=H^4=\mathbb Z/2,
\end{aligned}
$$

with all unlisted groups zero. The integral [Künneth theorem](../../../../../kunneth-theorem.md) has tensor terms with $i+j=q$ and [Tor functor](../../../../../tor-functor.md) terms with $i+j=q+1$:

$$
0\to\bigoplus_{i+j=q}H^i(A;\mathbb Z)\otimes H^j(B;\mathbb Z)
\to H^q(A\times B;\mathbb Z)
\to\bigoplus_{i+j=q+1}\operatorname{Tor}^{\mathbb Z}_1(H^i(A;\mathbb Z),H^j(B;\mathbb Z))
\to0.
$$

For these finite free cellular complexes it splits additively, though not canonically. Both the tensor and [Tor functor](../../../../../tor-functor.md) of two $\mathbb Z/2$ summands give $\mathbb Z/2$, so no order-four summands occur.

For an efficient count, write $F_A(t)$ for the free-rank polynomial and $T_A(t)$ for the number of $\mathbb Z/2$ summands in each degree. The [integral Künneth torsion polynomial](../../../../../integral-kunneth-torsion-polynomial.md) rule is

$$
F_{A\times B}=F_AF_B,\qquad
T_{A\times B}=F_AT_B+T_AF_B+(1+t^{-1})T_AT_B.
$$

The last two factors record respectively the tensor contribution in summed degree and the [Tor functor](../../../../../tor-functor.md) contribution one degree lower. The three factors have

$$
(F_2,T_2)=(1,t^2),\quad
(F_3,T_3)=(1+t^3,t^2),\quad
(F_4,T_4)=(1,t^2+t^4).
$$

The first two give $F_{23}=1+t^3$ and $T_{23}=2t^2+t^3+t^4+t^5$. Multiplying by the third gives

$$
F=1+t^3,\qquad
T=3t^2+3t^3+5t^4+6t^5+5t^6+4t^7+2t^8+t^9.
$$

Consequently the [integral cohomology of a product of finite real projective spaces](../../../../../integral-cohomology-of-a-product-of-finite-real-projective-spaces.md) in this case is

$$
\boxed{
H^q(\mathbb{RP}^2\times\mathbb{RP}^3\times\mathbb{RP}^4;\mathbb Z)
\cong
\begin{cases}
\mathbb Z,&q=0,\\
0,&q=1,\\
(\mathbb Z/2)^3,&q=2,\\
\mathbb Z\oplus(\mathbb Z/2)^3,&q=3,\\
(\mathbb Z/2)^5,&q=4,\\
(\mathbb Z/2)^6,&q=5,\\
(\mathbb Z/2)^5,&q=6,\\
(\mathbb Z/2)^4,&q=7,\\
(\mathbb Z/2)^2,&q=8,\\
\mathbb Z/2,&q=9,\\
0,&\text{otherwise}.
\end{cases}}
$$

If the intended coefficients were instead $\mathbb F_2$, the [Künneth theorem](../../../../../kunneth-theorem.md) over a field gives the dimension polynomial

$$
(1+t+t^2)(1+t+t^2+t^3)(1+t+t^2+t^3+t^4).
$$

Thus the mod-two groups in degrees zero through nine are respectively

$$
\boxed{\bigl(\dim_{\mathbb F_2}H^q\bigr)_{q=0}^{9}=(1,3,6,9,11,11,9,6,3,1),}
$$

and all other degrees vanish.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
