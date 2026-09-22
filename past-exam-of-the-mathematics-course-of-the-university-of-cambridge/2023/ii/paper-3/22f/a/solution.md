<h1 id="22f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A weak solution is a function $u\in H_0^1(U)$ satisfying

$$
\boxed{
\int_U\left(\nabla u\cdot\nabla v+m^2uv\right)\,dx
=\int_Ufv\,dx
\quad\text{for every }v\in H_0^1(U).}
$$

The zero boundary condition is encoded by membership in $H_0^1(U)$.

On the Hilbert space $H_0^1(U)$ define

$$
a(u,v)=\int_U(\nabla u\cdot\nabla v+m^2uv),
\qquad
\ell_f(v)=\int_Ufv.
$$

The form is bounded and coercive:

$$
a(u,u)=\|\nabla u\|_2^2+m^2\|u\|_2^2
\geq\min(1,m^2)\|u\|_{H^1}^2.
$$

The functional $\ell_f$ is bounded by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). The [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md) therefore gives a unique weak solution and a bound

$$
\|Tf\|_{H_0^1}\leq C\|f\|_2.
$$

Thus $T:L^2(U)\to H_0^1(U)$ is bounded. Composing it with the compact [Rellich-Kondrashov compactness theorem for H01](../../../../../../rellich-kondrashov-compactness-theorem-for-h01.md) embedding

$$
H_0^1(U)\hookrightarrow L^2(U)
$$

shows that $T:L^2(U)\to L^2(U)$ is the [compact massive-Laplacian resolvent](../../../../../../compact-massive-laplacian-resolvent.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [22F](../../22f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
