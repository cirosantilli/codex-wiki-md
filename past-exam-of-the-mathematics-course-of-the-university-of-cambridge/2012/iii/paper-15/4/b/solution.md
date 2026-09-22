<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First observe that the [Liouville one-form](../../../../../../canonical-one-form-on-a-cotangent-bundle.md) is zero as an ambient covector exactly on the [zero section](../../../../../../zero-section-of-a-vector-bundle.md). Indeed, $\alpha_{(x,p)}=p\circ d\pi$, and $d\pi$ is surjective. Since $dg$ is invertible, $g^*\alpha=\alpha$ therefore implies that $g$ maps the [zero section](../../../../../../zero-section-of-a-vector-bundle.md) onto itself. It induces a [diffeomorphism](../../../../../../diffeomorphism.md) $f:X\to X$ defined by $g(x,0)=(f(x),0)$.

The map $g$ is a [symplectomorphism](../../../../../../symplectomorphism.md), since it preserves $-d\alpha$. Let $E=\sum_i p_i\partial_{p_i}$ be the vertical [Liouville vector field](../../../../../../liouville-vector-field.md). With the chosen sign convention,

$$
\iota_E\omega=-\alpha.
$$

Preservation of both $\omega$ and $\alpha$ forces $g_*E=E$ because $\omega$ is [nondegenerate](../../../../../../nondegenerate-bilinear-form.md). Its complete [cotangent fiber-dilation flow](../../../../../../cotangent-fiber-dilation-flow.md) is

$$
D_s(x,p)=(x,e^sp),\qquad s\in\mathbb R.
$$

Uniqueness of integral curves gives $g\circ D_s=D_s\circ g$. If $g(x,p)=(y,P)$, let $s\to-\infty$. Continuity and this commutation yield

$$
(f(x),0)=g(x,0)=\lim_{s\to-\infty}g(x,e^sp)
=\lim_{s\to-\infty}(y,e^sP)=(y,0).
$$

Thus $y=f(x)$ for every $p$: the whole cotangent fiber over $x$ maps into the fiber over $f(x)$. This step proves that $g$ covers $f$; it was not assumed.

Now write $g(x,p)=(f(x),P(x,p))$. For any $u\in T_xX$, choose a tangent vector to $T^*X$ projecting to $u$. Evaluating $g^*\alpha=\alpha$ on it gives

$$
P(x,p)(df_xu)=p(u).
$$

Since $df_x$ is invertible, $P(x,p)=p\circ(df_x)^{-1}$. Therefore

$$
\boxed{g=f_\#,\qquad f=\pi\circ g\circ i_0,}
$$

and $f$ is unique. This [rigidity of cotangent Liouville-form preservation](../../../../../../rigidity-of-cotangent-liouville-form-preservation.md) uses smoothness at the [zero section](../../../../../../zero-section-of-a-vector-bundle.md); it follows from the canonical form and its dilation dynamics on the entire [cotangent bundle](../../../../../../cotangent-bundle.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
