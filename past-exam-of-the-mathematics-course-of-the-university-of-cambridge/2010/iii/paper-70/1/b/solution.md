<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Work above the plane, with $e^{-i\omega t}$ time dependence and $0<\theta<\pi$ away from grazing incidence. Put $a=k\cos\theta$ and $b=k\sin\theta$. The incident field and its chosen flat Dirichlet reflection cancel in value at the plane, while their [normal derivative](../../../../../../normal-derivative.md) is $-2ib e^{iax}$. Thus the diffracted correction has zero trace on the negative half-line and prescribed [normal derivative](../../../../../../normal-derivative.md) $2ib e^{iax}$ on the positive half-line.

There is an incompatibility in the stated edge data: a [normal derivative](../../../../../../normal-derivative.md) that is identically zero on the Neumann half-line cannot diverge as that half-line approaches the junction. **The inverse-square-root normal-derivative singularity belongs to the Dirichlet side, $x\to0^-$; on $x>0$ the total [normal derivative](../../../../../../normal-derivative.md) remains zero.** The following solution satisfies the mixed conditions and bounded-field edge behavior, with that corrected side.

Take the transform and its inverse as

$$
\widehat f(\alpha)=\int_{\mathbb R}f(x)e^{i\alpha x}dx,\qquad
f(x)=\frac1{2\pi}\int_C\widehat f(\alpha)e^{-i\alpha x}d\alpha.
$$

Let $U_+$ be the transform of the diffracted boundary value, and $V_-$ the transform of its unknown [normal derivative](../../../../../../normal-derivative.md) on the negative half-line. The outgoing transformed field is $U_+(\alpha)e^{i\beta(\alpha)y}$, where

$$
\beta=\sqrt{k^2-\alpha^2}=\beta_+\beta_-,\qquad\beta_+=\sqrt{k+\alpha},\quad\beta_-=\sqrt{k-\alpha}.
$$

Continue $k$ into the upper half-plane. Choose branches so that $\beta(0)=k$, outgoing propagating waves have positive vertical [wavenumber](../../../../../../wavenumber.md), and [evanescent waves](../../../../../../evanescent-wave.md) decay. The [branch point](../../../../../../branch-point.md) $-k$ lies below $C$ and belongs to $\beta_+$; $k$ lies above $C$ and belongs to $\beta_-$. Since $\int_0^\infty e^{i(\alpha+a)x}dx=i/(\alpha+a)$, the boundary transform equation is

$$
i\beta_+U_+=\frac{V_-}{\beta_-}-\frac{2b}{(\alpha+a)\beta_-}.
$$

The forcing splits by subtracting its numerator at the incident [pole](../../../../../../pole.md):

$$
H_+=-\frac{2b}{\beta_-(-a)(\alpha+a)},\qquad
H_-=-\frac{2b}{\alpha+a}\left(\frac1{\beta_-(\alpha)}-\frac1{\beta_-(-a)}\right).
$$

The [pole](../../../../../../pole.md) in $H_-$ is removable; $H_-$ is analytic below $C$, while $H_+$ is analytic above it. Hence $i\beta_+U_+-H_+=V_-/\beta_-+H_-$ is entire. The bounded mixed-boundary edge solution has $U_+=O(\alpha^{-3/2})$ and $V_-=O(\alpha^{-1/2})$, making both sides decay at infinity. These orders can also be obtained locally from the leading wedge solution $r^{1/2}\cos(\varphi/2)$, which is Neumann at $\varphi=0$ and Dirichlet at $\varphi=\pi$. [Liouville's theorem](../../../../../../liouville-theorem.md) sets the entire remainder to zero. Therefore

$$
\boxed{U_+(\alpha)=\frac{2ib}{\sqrt{k+a}\,(\alpha+a)\sqrt{k+\alpha}}.}
$$

The solution of [mixed Dirichlet-Neumann half-plane diffraction](../../../../../../mixed-dirichlet-neumann-half-plane-diffraction.md) is consequently

$$
\boxed{\phi_d(x,y)=\frac{ib}{\pi\sqrt{k+a}}\int_C\frac{e^{-i\alpha x+i\sqrt{k^2-\alpha^2}\,y}}{(\alpha+a)\sqrt{k+\alpha}}\,d\alpha,\qquad
\phi_t=e^{iax-iby}-e^{iax+iby}+\phi_d.}
$$

For $k=k_0+i\varepsilon$, take $C$ from left to right inside $-\varepsilon<\operatorname{Im}\alpha<\varepsilon$ and above the incident [pole](../../../../../../pole.md) $-a$. Cuts from $-k$ run into the lower half-plane and cuts from $k$ into the upper half-plane, without crossing $C$. For example choose $\operatorname{Im}\alpha=c$ with $\max(-\varepsilon,-\varepsilon\cos\theta)<c<\varepsilon$. Then let $\varepsilon\downarrow0$, keeping the contour above $-a$ and $-k$ and below $k$. Any subsequent deformation for asymptotic evaluation must preserve these bypasses or include the [residues](../../../../../../residue.md) of crossed [poles](../../../../../../pole.md). This prescription fixes the reflected-wave contributions and the [radiation condition](../../../../../../radiation-condition.md); a principal-value [integral](../../../../../../integral.md) alone would not do so.

As a boundary check, $i\beta U_+=-2b\beta_-/[\sqrt{k+a}(\alpha+a)]$. On the positive half-line the lower-contour [residue](../../../../../../residue.md) gives $2ib e^{iax}$, cancelling the incident-plus-reflected [derivative](../../../../../../derivative.md). The boundary trace vanishes on the negative half-line by upper-half-plane analyticity. Finally $U_+=O(\alpha^{-3/2})$ gives a square-root boundary value and hence a bounded field at the junction; the singular [derivative](../../../../../../derivative.md) occurs on its Dirichlet side.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
