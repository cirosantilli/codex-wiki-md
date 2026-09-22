<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For [chain maps](../../../../../chain-map.md) $f,g:C_*\to D_*$, a [chain homotopy](../../../../../chain-homotopy.md) from $g$ to $f$ is a family of [group homomorphisms](../../../../../group-homomorphism.md) $s_q:C_q\to D_{q+1}$ satisfying

$$
\boxed{f_q-g_q=d^D_{q+1}s_q+s_{q-1}d^C_q\quad\text{for every }q.}
$$

If $z$ is a [chain cycle](../../../../../chain-cycle.md), then $(f-g)(z)=d^Ds(z)$ is a [chain boundary](../../../../../chain-boundary.md). Consequently $[f(z)]=[g(z)]$, so $\boxed{f_*=g_*}$ on every [homology group](../../../../../homology-group.md).

Order the vertices of the [simplex](../../../../../simplex.md) as $v_0,\ldots,v_n$. Its [simplicial chain complex](../../../../../simplicial-chain-complex.md) has

$$
S_q(\Delta^n)=\bigoplus_{0\leq i_0<\cdots<i_q\leq n}\mathbb Z[v_{i_0},\ldots,v_{i_q}]
\quad(0\leq q\leq n),
$$

and zero groups otherwise. An arbitrary ordering represents the sign of the [permutation](../../../../../permutation.md) times the increasing ordering. Its [boundary operator](../../../../../boundary-operator.md) is

$$
d_q[v_{i_0},\ldots,v_{i_q}]
=\sum_{r=0}^q(-1)^r[v_{i_0},\ldots,\widehat v_{i_r},\ldots,v_{i_q}]
\quad(q\geq1),\qquad d_0=0.
$$

In $d^2$ each face obtained by deleting the vertices in positions $r<t$ occurs twice. Deleting $r$ first gives sign $(-1)^r(-1)^{t-1}$, whereas deleting $t$ first gives $(-1)^t(-1)^r$. These signs are opposite, so all terms cancel. The case $d_0d_1=0$ follows directly from $d_0=0$. Thus $\boxed{d^2=0}$.

For the [homology](../../../../../homology-split.md) calculation, add the augmentation $\varepsilon:S_0\to\mathbb Z$ sending every vertex to $1$. Regard $\mathbb Z$ as the group in degree $-1$ of an [augmented chain complex](../../../../../augmented-chain-complex.md). Define the [simplicial cone chain contraction](../../../../../simplicial-cone-chain-contraction.md) by

$$
s_{-1}(1)=[v_0],\qquad
s_q[v_{i_0},\ldots,v_{i_q}]=
\begin{cases}
[v_0,v_{i_0},\ldots,v_{i_q}],&i_0>0,\\
0,&i_0=0.
\end{cases}
$$

If the simplex does not contain $v_0$, expansion of its coned boundary gives $ds(\sigma)=\sigma-sd(\sigma)$. If it contains $v_0$, the only face on which $s$ is nonzero is the face omitting $v_0$, and $sd(\sigma)=\sigma$. In degree zero this uses the augmentation, and in degree $-1$ it says $\varepsilon s_{-1}=1$. Hence

$$
\boxed{ds+sd=1\quad\text{on the augmented complex}.}
$$

Every positive-degree [chain cycle](../../../../../chain-cycle.md) is therefore a [chain boundary](../../../../../chain-boundary.md). In degree zero, the same identity says $z-\varepsilon(z)[v_0]=ds_0(z)$, so the augmentation induces an isomorphism $H_0\to\mathbb Z$, with inverse $1\mapsto[v_0]$. Thus, including $n=0$,

$$
\boxed{H_q(S_*(\Delta^n))\cong
\begin{cases}\mathbb Z,&q=0,\\0,&q>0.\end{cases}}
$$

This is a direct [chain homotopy](../../../../../chain-homotopy.md) calculation and uses no result about [cellular homology](../../../../../cellular-chain-complex.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 114](../../paper-114-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
