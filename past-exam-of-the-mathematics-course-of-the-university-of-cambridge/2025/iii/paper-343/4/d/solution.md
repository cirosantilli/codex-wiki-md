<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The two-dimensional [Kramers--Wannier projected entangled pair operator](../../../../../../kramers-wannier-projected-entangled-pair-operator.md) puts an input bit $s_v$ at every vertex and an output bit $t_e$ at every edge. A COPY tensor at each vertex sends $s_v$ to every incident virtual leg, and an XOR tensor on $e=(uv)$ imposes

$$
t_e=s_u+s_v\pmod2.
$$

Contracting the vertex-edge virtual legs gives the requested PEPO. Algebraically it is

$$
D_2=\sum_{\{s_v\}}|\{s_u+s_v\}_{e=(uv)}\rangle_Z\langle\{s_v\}|_X.
$$

The output domain walls are not independent. Around every plaquette $p$, each vertex bit occurs twice, so

$$
\boxed{B_p=\prod_{e\in\partial p}\widetilde Z_e=1}.
$$

Products of these loop operators generate a $\mathbb Z_2$ [one-form symmetry](../../../../../../one-form-symmetry.md): its charged objects are line operators, and contractible closed loops act trivially on the PEPO image. This symmetry is unavoidable because edge variables obtained as discrete gradients have zero flux around every contractible loop.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 343](../../../paper-343-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
