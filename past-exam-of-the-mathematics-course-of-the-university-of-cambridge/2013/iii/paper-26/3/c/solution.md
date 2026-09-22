<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For every site, $P(R(x)\geq r)=\beta_r$. This event depends only on [edges](../../../../../../edge-of-a-graph.md) with both endpoints in $x+\Lambda_r$: any connecting path can be stopped on its first hit of that boundary. Since $\lambda>0$, $\beta_r\to0$, so all clusters have finite radius almost surely, by a countable union over sites. Set the radius of an isolated site to zero.

Write $a_n=(d/\lambda)\log n$. It suffices to take $0<\epsilon<1$, since larger error intervals contain one such interval. For any small $\delta>0$, the decay-rate limit gives, for all large $r$,

$$
e^{-(\lambda+\delta)r}\leq\beta_r\leq e^{-(\lambda-\delta)r}.
$$

For the upper tail use $r_+=\lceil(1+\epsilon)a_n\rceil$ and a [union bound](../../../../../../boole-s-inequality.md):

$$
P(M_n\geq r_+)\leq(2n+1)^d\beta_{r_+}
\leq Cn^{d-(\lambda-\delta)(1+\epsilon)d/\lambda}\longrightarrow0,
$$

provided $\delta<\lambda\epsilon/(1+\epsilon)$.

For the lower tail let $r_-=\lfloor(1-\epsilon)a_n\rfloor+1$. Choose sites in $\Lambda_{n-r_-}$ spaced by $2r_-+1$ in each coordinate. Their radius-$r_-$ boxes are vertex-disjoint, so their local connection events are independent. There are $N_n\geq c(n/r_-)^d$ such sites for large $n$. If $M_n\leq(1-\epsilon)a_n$, none of these events occurs. Thus

$$
P(M_n\leq(1-\epsilon)a_n)\leq(1-\beta_{r_-})^{N_n}\leq e^{-N_n\beta_{r_-}},
$$

where

$$
N_n\beta_{r_-}\geq\frac{c}{(\log n)^d}
 n^{d-(\lambda+\delta)(1-\epsilon)d/\lambda}\longrightarrow\infty
$$

if $\delta<\lambda\epsilon/(1-\epsilon)$. Choose one $\delta$ satisfying both restrictions. The integer choices give the required strict inequalities. Thus the [maximum cluster radius under exponential one-arm decay](../../../../../../maximum-cluster-radius-under-exponential-one-arm-decay.md) has [convergence in probability](../../../../../../convergence-in-probability.md):

$$
\boxed{\frac{M_n}{(d/\lambda)\log n}\longrightarrow1\quad\text{in probability}}.
$$

The logarithmic box-packing loss does not change the leading constant $d/\lambda$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
