<h1 id="14e/solution">Solution</h1>

↑ **Parent:** [14E](../14e.md)

An [interval covering relation](../../../../../interval-covering-relation.md) $I\to J$ means $F(I)\supseteq J$. The associated directed graph has one vertex for each interval and an edge $i\to j$ for each covering. Its [transition matrix](../../../../../stochastic-matrix.md) is $A_{ij}=1$ when that edge exists, and zero otherwise. [Matrix](../../../../../matrix.md) multiplication counts walks; thus $\boxed{\operatorname{tr}(A^n)}$ counts closed length-$n$ itineraries, with a distinguished starting vertex.

To see how itineraries force [periodic orbits](../../../../../periodic-orbit.md), a [continuous map](../../../../../continuous-map.md) covering a closed interval has a closed subinterval mapping onto it: choose successive first/last crossings of its endpoints. Pull these subintervals back along a closed walk. This yields $K\subseteq I_{i_0}$ with $F^n(K)\supseteq I_{i_0}\supseteq K$. At the two preimages of the ends of $K$, $F^n(x)-x$ has opposite weak signs; the [intermediate value theorem](../../../../../intermediate-value-theorem.md) gives a [fixed point](../../../../../fixed-point.md) of $F^n$.

A graph alone does not give an exact count of periodic points for a general [continuous map](../../../../../continuous-map.md): extra oscillations or a fixed interval can create additional points. For example on $I=[0,1]$, both $F(x)=x$ and $F(x)=1-x$ have [matrix](../../../../../matrix.md) $A=(1)$; the first has infinitely many [fixed points](../../../../../fixed-point.md) and the second only one. Distinct itineraries give distinct points when their interval interiors are disjoint and the [periodic orbit](../../../../../periodic-orbit.md) avoids shared endpoints. In that setting, $\operatorname{tr}(A^n)$ is a guaranteed lower bound, not a universal equality. Likewise, the primitive-word count $(1/n)\sum_{d\mid n}\mu(d)\operatorname{tr}(A^{n/d})$ counts guaranteed least-period itineraries under this separation condition. With overlapping intervals, even distinctness needs qualification. This is the scope of [counting cycles in an interval covering graph](../../../../../counting-cycles-in-an-interval-covering-graph.md).

For the first five-cycle, put $I_j=[x_j,x_{j+1}]$, $0\le j\le3$. The graph and [matrix](../../../../../matrix.md) are

$$
0\to1,\quad1\to2,\quad2\to3,\quad3\to0,1,2,3,
\qquad
A=\begin{pmatrix}0&1&0&0\\0&0&1&0\\0&0&0&1\\1&1&1&1\end{pmatrix}.
$$

The four traces are $1,3,7,15$. Shared endpoints have least period five, so they do not spoil the distinctness argument for the requested periods. Primitive cyclic itineraries are: $3$ for period one; $(3,2)$ for period two; $(3,1,2)$ and $(3,3,2)$ for period three; $(0,1,2,3)$, $(3,3,1,2)$ and $(3,3,3,2)$ for period four. Consequently the [monotone five-cycle interval covering pattern](../../../../../monotone-five-cycle-interval-covering-pattern.md) guarantees

$$
\boxed{\text{at least }1,1,2,3\text{ cycles of least periods }1,2,3,4.}
$$

These words specify the successive intervals containing their points; cyclic rotations denote the same orbit.

There is a [horseshoe for an interval map](../../../../../horseshoe-for-an-interval-map.md) for $F^2$: both $I_2$ and $I_3$ cover $I_2\cup I_3$ under that iterate, and their interiors are disjoint. Repeated binary choices produce at least $2^n$ separated length-$n$ itineraries for the second iterate, hence positive [topological entropy](../../../../../topological-entropy.md), at least $(\log2)/2$ for $F$. Thus the dynamics are chaotic in this standard interval-map sense. No conclusion of global transitivity on all of $\mathbb R$ follows.

A one-step horseshoe is not guaranteed if that is the intended definition. For example the unimodal [continuous map](../../../../../continuous-map.md) $F(x)=x+1$ for $x\le3$ and $F(x)=16-4x$ for $x\ge3$ has cycle $0,1,2,3,4$. A left-branch interval cannot cover itself, since its image is shifted to the right. Two right-branch intervals cannot each cover their union because that branch is injective. If one interval straddles the maximum and covers itself, its right endpoint must map below its left endpoint; every disjoint interval farther to the right then maps below it and cannot self-cover. A disjoint interval to the left also cannot self-cover. So this example has no one-step two-branch horseshoe, although its second iterate does. It also proves that **$F$ can be unimodal**.

For the second order, write $J_0=[x_3,x_1]$, $J_1=[x_1,x_0]$, $J_2=[x_0,x_2]$, $J_3=[x_2,x_4]$. Endpoint images give

$$
0\to3,\quad1\to1,2,\quad2\to0,\quad3\to0,1,
\qquad B=\begin{pmatrix}0&0&0&1\\0&1&1&0\\1&0&0&0\\1&1&0&0\end{pmatrix}.
$$

The traces are $1,3,1,7$. The guaranteed primitive words are $1$, $(0,3)$ and $(1,2,0,3)$, giving $\boxed{\text{periods }1,2,4\text{ but not necessarily }3}$. To prove the last qualification, take ordered points $0,1,2,3,4$ and linearly interpolate the map values $4,3,1,0,2$ on $[0,4]$, extending by $G(x)=4-x$ for $x<0$ and $G(x)=2$ for $x>4$. Both exterior regions enter $[0,4]$ after at most two steps, so they introduce no extra periodic points. Its only closed length-three itinerary is $111$; on $J_1$ it is $x\mapsto5-2x$, whose third iterate has only the same [fixed point](../../../../../fixed-point.md). Endpoints have least period five, so this example has no three-cycle.

The distinct fourth-iterate return walks $1111$ and $1203$ yield two subintervals of $J_1$ that return over $J_1$, giving a horseshoe for $G^4$ and positive entropy at least $(\log2)/4$. Thus $G$ too must have chaotic interval dynamics and a horseshoe in some iterate. The affine example has no one-step horseshoe: its increasing branch lies strictly below the diagonal, while on the decreasing branch injectivity prevents two self-covering intervals; a minimum-straddling self-covering interval excludes a self-covering interval on either side by the same endpoint argument. The distinction between a map and its iterate is essential for both patterns.

## ↑ Ancestors (10)

1. [14E](../14e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
