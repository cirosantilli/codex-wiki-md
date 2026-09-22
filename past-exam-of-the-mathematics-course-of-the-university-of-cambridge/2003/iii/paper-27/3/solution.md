<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [Morse function](../../../../../morse-function.md) is a smooth real-valued function all of whose [critical points](../../../../../critical-point.md) have nonsingular [Hessian matrices](../../../../../hessian-matrix.md). We use the descending convention for a [gradient-like vector field](../../../../../gradient-like-vector-field.md) $V$: away from critical points, $df(V)<0$, and near a critical point of [Morse index](../../../../../morse-index.md) $\lambda$, in [Morse lemma](../../../../../morse-lemma.md) coordinates $f=f(p)-|u|^2+|v|^2$, the field can be chosen as $V=(2u,-2v)$.

For its flow $\phi_t$, define the [unstable manifold](../../../../../unstable-manifold.md) $W^u(p)=\{x:\lim_{t\to-\infty}\phi_t(x)=p\}$ and the [stable manifold](../../../../../stable-manifold.md) $W^s(q)=\{x:\lim_{t\to+\infty}\phi_t(x)=q\}$. Their dimensions are $\operatorname{ind}p$ and $m-\operatorname{ind}q$. The [Morse-Smale transversality condition](../../../../../morse-smale-gradient-flow.md) is

$$
T_xW^u(p)+T_xW^s(q)=T_xM\quad\text{for every }x\in W^u(p)\cap W^s(q).
$$

For a closed [manifold](../../../../../topological-manifold.md), this lets us form the [Morse-Smale complex](../../../../../morse-smale-complex.md) over $\mathbb Z$. Orient each unstable manifold and take

$$
C_j=\bigoplus_{\operatorname{ind}p=j}\mathbb Zp,\qquad \partial p=\sum_{\operatorname{ind}q=j-1}n(p,q)q.
$$

The transverse intersection for an index difference of one is one-dimensional; quotienting by flow time gives a finite set of trajectories, and $n(p,q)$ counts them with orientation signs. Compactifying the one-dimensional spaces of trajectories for an index difference of two adds broken trajectories. Their oriented boundary count is zero, giving $\partial^2=0$. The descending cells are the unstable manifolds, and these counts are the incidence numbers of the corresponding [cellular chain complex](../../../../../cellular-chain-complex.md), so **the homology of this complex is $H_*(M;\mathbb Z)$**. Ambient orientability is unnecessary: orientations of the unstable cells provide the requisite coorientations and trajectory signs.

For the [Klein bottle](../../../../../klein-bottle.md), use the quotient of $\mathbb R^2$ by $(s,t)\sim(s+2\pi,-t)$ and $(s,t)\sim(s,t+2\pi)$. A model of the standard four-critical-point height function is

$$
f(s,t)=\cos s+\varepsilon\cos t,\qquad0<\varepsilon<1.
$$

It is well defined under both identifications. Its [critical points](../../../../../critical-point.md), their [Morse indices](../../../../../morse-index.md), and critical values are

$$
\begin{array}{c|c|c}
\text{point}&\text{index}&f\\\hline
m=(\pi,\pi)&0&-1-\varepsilon\\
b=(\pi,0)&1&-1+\varepsilon\\
a=(0,\pi)&1&1-\varepsilon\\
q=(0,0)&2&1+\varepsilon.
\end{array}
$$

The [Hessian matrix](../../../../../hessian-matrix.md) is diagonal with entries $-\cos s$ and $-\varepsilon\cos t$, so each point is nondegenerate. The flat quotient metric gives descending equations $\dot s=\sin s$, $\dot t=\varepsilon\sin t$. Their saddle separatrices are the coordinate lines; the two saddle-to-saddle intersections are empty, and all remaining stable and unstable intersections are transverse. This is a [Morse-Smale gradient flow](../../../../../morse-smale-gradient-flow.md). If one insists on the exact local-model version of a [gradient-like vector field](../../../../../gradient-like-vector-field.md) above, change the two coordinate speeds near the critical points to the standard quadratic-model speeds. This preserves the separatrices, signs and transversality.

Both branches of either saddle flow to the minimum with opposite endpoint signs, so $\partial a=\partial b=0$. From the maximum to $a$, the two trajectories lie on $s=0$ and approach $t=\pi$ from opposite directions. The identification in $t$ is a translation, so their incidence signs are opposite and cancel. The two trajectories to $b$ lie on $t=0$ and approach $s=\pi$ from opposite directions. The identification in $s$ reverses the transverse $t$-coordinate, reversing one additional orientation sign. These two contributions consequently have the same sign. Choosing the orientation of $b$ gives $\partial q=2b$.

One can check the coefficient directly from the [cell attachment](../../../../../cell-attachment.md) of the top cell: its boundary word is $aba^{-1}b$, with exponent sums zero on the base loop $a$ and two on the fiber loop $b$. Thus the [integral Morse complex of the Klein bottle](../../../../../integral-morse-complex-of-the-klein-bottle.md) is

$$
0\longrightarrow\mathbb Zq\xrightarrow{\binom{0}{2}}\mathbb Za\oplus\mathbb Zb\xrightarrow{0}\mathbb Zm\longrightarrow0,
$$

and

$$
\boxed{H_0(K;\mathbb Z)=\mathbb Z,\quad H_1(K;\mathbb Z)=\mathbb Z\oplus\mathbb Z/2,\quad H_2(K;\mathbb Z)=0.}
$$

Counting trajectories without signs, or working only modulo two, would miss the order-two class.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
