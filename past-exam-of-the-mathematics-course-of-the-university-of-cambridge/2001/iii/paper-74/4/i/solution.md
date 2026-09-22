<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use $R=\mathcal O_{k_{\mathfrak p}}$, the valuation ring of the [completion of a number field at a prime ideal](../../../../../../completion-of-a-number-field-at-a-prime-ideal.md), with [uniformizer](../../../../../../uniformizer.md) $\pi$ and [residue field](../../../../../../residue-field.md) $\kappa$. This completeness is essential for [coprime-factor Hensel lifting](../../../../../../coprime-factor-hensel-lifting.md). Normalize the two residue factors to be monic first; if the original factors have reciprocal leading units, undo the normalization by multiplying the eventual factors by reciprocal lifts of those units.

Let the two monic residue degrees be $d_1,d_2$. Start with monic lifts $g_1,h_1$ satisfying $f\equiv g_1h_1\pmod\pi$. Suppose monic lifts $g_r,h_r$ of these degrees satisfy $f-g_rh_r\in\pi^rR[X]$. Put $E_r=(f-g_rh_r)/\pi^r$, of degree less than $d_1+d_2$. Over $\kappa$, the linear map

$$
\kappa[X]_{<d_1}\oplus\kappa[X]_{<d_2}\longrightarrow\kappa[X]_{<d_1+d_2},\qquad (u,v)\longmapsto u\phi_2+v\phi_1
$$

is injective: a zero image makes $\phi_1$ divide $u$, by coprimality, forcing $u=0$ by its degree bound, and then $v=0$. The dimensions agree, so this map is a bijection. Choose lifts $u_r,v_r$ whose image is $\overline E_r$, and set

$$
g_{r+1}=g_r+\pi^ru_r,\qquad h_{r+1}=h_r+\pi^rv_r.
$$

Their product agrees with $f$ modulo $\pi^{r+1}$; the new cross term has factor $\pi^{2r}$ and $2r\ge r+1$. The degree bounds preserve monicity. Each coefficient is a Cauchy sequence in the complete [discrete valuation ring](../../../../../../discrete-valuation-ring.md) $R$, so the limits $f_1,f_2$ satisfy

$$
\boxed{f=f_1f_2,\qquad \overline f_1=\phi_1,\quad\overline f_2=\phi_2.}
$$

If $\mathfrak o_{\mathfrak p}$ were interpreted only as an ordinary localization rather than the completed valuation ring, the assertion would be false. For example $X^2-2$ splits modulo seven but is irreducible over $\mathbb Q$. The completion notation in the next part provides the intended local-field interpretation.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
