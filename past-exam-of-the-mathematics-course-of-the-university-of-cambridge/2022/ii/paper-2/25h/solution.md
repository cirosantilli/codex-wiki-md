<h1 id="25h/solution">Solution</h1>

↑ **Parent:** [25H](../25h.md)

The [Riemann-Hurwitz formula](../../../../../riemann-hurwitz-formula.md) for a nonconstant degree-$n$ morphism  
$f:C\to C'$ of smooth projective connected curves in characteristic zero is

$$
2g(C)-2=n(2g(C')-2)+\deg R_f,
$$

where $R_f$ is the effective ramification divisor. If $g(C')\geq2$ and  
$g(C)<g(C')$, the right side is at least $2g(C')-2>2g(C)-2$, impossible. If $g(C')=1$, then $g(C)=0$ and the left side is $-2$ while the right side is nonnegative. Thus every morphism is constant.

Choose $p\in C_d$ and project from $p$ to the pencil of lines through it. Bézout's theorem says that a general such line meets $C_d$ in $p$ plus $d-1$ further points, so the resolved projection

$$
\phi:C_d\to\mathbb P^1
$$

has degree $d-1$. Since the [genus of a smooth plane curve](../../../../../genus-of-a-smooth-plane-curve.md) is  
$g=(d-1)(d-2)/2$, Riemann--Hurwitz gives

$$
\deg R_\phi
=2g-2+2(d-1)
=(d-2)(d+1).
$$

Every branch point receives at least one ramification point, hence

$$
\boxed{|B|\leq(d-2)(d+1)}.
$$

The adjunction formula gives

$$
K_{C_d}\sim(d-3)D.
$$

Since $\deg D=d$ and $\deg K_{C_d}=d(d-3)$, linear equivalence  
$D\sim K_{C_d}$ would force $d=d(d-3)$, hence $d=4$. It is therefore impossible for $d\geq5$.

For a smooth plane quartic, projection from a point of the curve gives a degree-three map, so its [gonality](../../../../../gonality.md) is at most three. Its genus is three and  
$K_C\sim D$, so its plane embedding is the [canonical map](../../../../../canonical-map.md). A genus-three curve with a degree-two map to $\mathbb P^1$ would be [hyperelliptic](../../../../../hyperelliptic-curve.md), and its canonical map would factor through that double cover and map onto a conic rather than embed the curve. Thus no degree-two map exists, and a degree-one map is excluded by the genus. The quartic's gonality is

$$
\boxed{3}.
$$

For a genus-one curve, Riemann--Roch supplies a degree-two map to $\mathbb P^1$, while degree one would make it isomorphic to $\mathbb P^1$. Its gonality is therefore

$$
\boxed{2}.
$$

## ↑ Ancestors (10)

1. [25H](../25h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
