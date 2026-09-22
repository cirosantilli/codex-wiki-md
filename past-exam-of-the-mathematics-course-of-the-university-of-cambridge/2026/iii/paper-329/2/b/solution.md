<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

When internal pressure gradients matter, axial lubrication flow in the low-viscosity interior has volume flux

$$
Q=-\frac{\pi a^4}{8\lambda\mu}P_z.
$$

Conservation of cross-sectional area, $(\pi a^2)_t+Q_z=0$, and the normal-stress expression for $P$ give

$$
\boxed{2aa_t=\frac1{8\lambda\mu}\frac\partial{\partial z}
\left[a^4\frac\partial{\partial z}\left(\frac{2\mu a_t}{a}+\frac\gamma a\right)\right]}.
$$

Let $\tau=t^*-t$. Balancing $2\mu a_t/a$ with $\gamma/a$ gives $a\sim\tau$, so $p=1$. Balancing either pressure contribution after two axial derivatives with $aa_t$ then gives $q=1$. Define

$$
C=\frac\gamma{2\mu},
\qquad
a=C\tau A(\zeta),
\qquad
\zeta=\frac{z-z^*}{L\tau},
\qquad
L=\frac{C}{\sqrt{8\lambda}}.
$$

At fixed $z$, $a_t=C(\zeta A'-A)$, and

$$
\frac{2\mu a_t}{a}+\frac\gamma a
=\frac{2\mu}{\tau}
\left(\frac{\zeta A'}A-1+\frac1A\right).
$$

Substitution leaves the parameter-free third-order equation

$$
\boxed{
\frac d{d\zeta}\left[
A^4\frac d{d\zeta}
\left(\frac{\zeta A'}A-1+\frac1A\right)
\right]
=A(\zeta A'-A)}.
$$

Thus the similarity exponents are $\boxed{p=q=1}$; boundary and matching conditions would select a particular profile $A$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
