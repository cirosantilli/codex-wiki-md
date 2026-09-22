<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Work in finite-dimensional Euclidean spaces. Suppose the [graph of a set-valued mapping](../../../../../../graph-of-a-set-valued-mapping.md),

$$
\operatorname{gph}S=\{(u,v):v\in S(u)\},
$$

is locally closed at $(\bar u,\bar v)\in\operatorname{gph}S$. Local closedness means that its intersection with some neighborhood of this point is closed relative to that neighborhood. This assumption is part of the criterion.

For a set $C$ and $z\in C$, define the [Fréchet normal cone](../../../../../../frechet-normal-cone.md) by

$$
\widehat N_C(z)=\left\{w:\limsup_{\substack{z'\to z\\z'\in C,\ z'\ne z}}
\frac{\langle w,z'-z\rangle}{\|z'-z\|_2}\leq0\right\}.
$$

At an isolated point the condition is vacuous, so all vectors are regular normals. The [limiting normal cone](../../../../../../limiting-normal-cone.md) consists of limits of these regular normals at nearby points:

$$
N_C(z)=\left\{w:\exists z_k\in C,\ z_k\to z,\ \exists w_k\in\widehat N_C(z_k),\ w_k\to w\right\}.
$$

It can be nonconvex. The [Mordukhovich coderivative](../../../../../../limiting-coderivative.md) is

$$
\boxed{D^*S(\bar u\mid\bar v)(v^*)
=\{u^*:(u^*,-v^*)\in N_{\operatorname{gph}S}(\bar u,\bar v)\}}.
$$

The minus sign in the output-dual component is part of the definition. For a single-valued continuously differentiable mapping $s$, the graph normal is $(Ds(\bar u)^Tv^*,-v^*)$, giving $D^*s(\bar u\mid s(\bar u))(v^*)=\{Ds(\bar u)^Tv^*\}$. Thus the [coderivative](../../../../../../limiting-coderivative.md) extends a transpose derivative, rather than the ordinary forward derivative.

The exact [Mordukhovich criterion](../../../../../../mordukhovich-criterion.md) is

$$
\boxed{S\text{ has the Aubin property at }(\bar u,\bar v)
\iff D^*S(\bar u\mid\bar v)(0)=\{0\}}.
$$

This is equivalent to excluding a nonzero horizontal limiting graph normal $(u^*,0)$. One must use the [limiting normal cone](../../../../../../limiting-normal-cone.md); simply checking regular normals at the reference point can miss normals inherited from neighboring graph pieces.

For [sensitivity analysis](../../../../../../sensitivity-analysis.md), apply this test to a solution map or use [coderivative](../../../../../../limiting-coderivative.md) and [normal cone](../../../../../../normal-cone.md) calculus to express its graph normals through optimality constraints. Triviality of this kernel then proves [Lipschitz-like](../../../../../../aubin-property.md) stability without solving the perturbed problem explicitly. Under these same finite-dimensional, locally closed assumptions, the exact Lipschitz modulus is the outer norm

$$
\operatorname{lip}S(\bar u\mid\bar v)
=\sup\{\|u^*\|_2:u^*\in D^*S(\bar u\mid\bar v)(v^*),\ \|v^*\|_2\leq1\}.
$$

The zero-kernel condition is the qualitative criterion; the modulus quantifies the sensitivity bound. For the next problem an explicit local formula is simpler than evaluating these graph normals.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 325](../../../paper-325-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
