<h1 id="4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

All classes in the nontrivial homological equalities are taken in $H_1(X_{(p,q)};\mathbb Z)$, where $X_{(p,q)}=M_{S^2}(p^*/q,-q^*/p,*)$. The two internal gluing [torus](../../../../../../../torus.md) components still have inclusion maps into this [knot exterior](../../../../../../../knot-exterior.md). Interpreting the maps instead as maps into the closed $S^3$ would make every displayed class zero.

Before the two [Dehn fillings](../../../../../../../dehn-filling.md), $H_1(S^1\times\text{pair of pants};\mathbb Z)$ has generators $f,h_1,h_2,h_3$ and relation $h_1+h_2+h_3=0$. The [Dehn fillings](../../../../../../../dehn-filling.md) add $p^*f-qh_1=0$ and $-q^*f-ph_2=0$. Put $m=-h_3$. Eliminating the relations using $pp^*-qq^*=1$ gives

$$
\boxed{H_1(X_{(p,q)};\mathbb Z)=\mathbb Z\langle m\rangle,\quad
f=pq\,m,\quad h_1=pp^*m,\quad h_2=-qq^*m.}
$$

For completeness, the three relation rows in generators $(f,h_1,h_2)$ are $(p^*,-q,0)$, $(-q^*,0,-p)$, $(0,1,1)$ when computing the quotient by $m$. Their [determinant](../../../../../../../determinant.md) is $pp^*-qq^*=1$, so $m$ really generates the entire [first homology group](../../../../../../../first-homology.md), and no finite torsion or index is hidden in the elimination.

Orient each exceptional-fiber longitude by $\mu_i\cdot\lambda_i=1$. In the boundary basis $(m_i,\tilde f_i)=(-\tilde h_i,\tilde f_i)$, write $\mu_i=\alpha_i m_i+\beta_i\tilde f_i$ and $\lambda_i=u_i m_i+v_i\tilde f_i$, where $\alpha_i v_i-\beta_i u_i=1$. Then

$$
\tilde f_i=-u_i\mu_i+\alpha_i\lambda_i.
$$

The filled [meridian of a solid torus](../../../../../../../meridian-of-a-solid-torus.md) maps to zero, and $(\alpha_1,\alpha_2)=(q,p)$, yielding

$$
\boxed{f=pq\,\iota_{3*}(m)=q\,\iota_{1*}(\lambda_1)=p\,\iota_{2*}(\lambda_2).}
$$

Adding multiples of $\mu_i$ to $\lambda_i$ has no effect. The word “any” therefore means any longitude with this compatible orientation; negating a longitude would negate the corresponding equality.

To compute [Turaev torsion](../../../../../../../turaev-torsion.md), use the general product formula $\tau(S^1\times F)\doteq(1-[f])^{-\chi(F)}$ and multiplicativity under gluing along [torus](../../../../../../../torus.md) components. For a [pair of pants](../../../../../../../pair-of-pants-mathematics.md), $\chi(F)=-1$, so the unfilled piece contributes $1-[f]$. The two filling [solid torus](../../../../../../../solid-torus.md) pieces contribute $(1-[\lambda_1])^{-1}$ and $(1-[\lambda_2])^{-1}$. With $t=[m]$, the equalities above give $[f]=t^{pq}$, $[\lambda_1]=t^p$, and $[\lambda_2]=t^q$. Therefore

$$
\boxed{\tau(X_{(p,q)})\doteq\frac{1-t^{pq}}{(1-t^p)(1-t^q)}.}
$$

Here $\doteq$ allows the unit $\pm t^n$: a fully refined [Turaev torsion](../../../../../../../turaev-torsion.md) requires an [Euler structure](../../../../../../../euler-structure.md) and a [homology orientation](../../../../../../../homology-orientation.md), neither of which the statement specifies. The displayed rational function is the representative whose expansion at $t=0$ starts with $1$, equivalently the standard nonnegative-exponent normalization.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 141](../../../../paper-141-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
