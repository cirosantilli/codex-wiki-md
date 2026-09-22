<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Regard the antisymmetric tensor as a real differential-form potential $A_p$. For a free [massless p-form gauge field](../../../../../../massless-p-form-gauge-field.md), its field strength is $F_{p+1}=dA_p$ and its gauge transformation is $A_p\mapsto A_p+d\Lambda_{p-1}$. The [Bianchi identity for an Abelian p-form](../../../../../../bianchi-identity-for-an-abelian-p-form.md) and the source-free field equation are

$$
dF=0,\qquad d*F=0.
$$

The [Hodge star](../../../../../../hodge-star-operator.md) makes $*F$ a closed $(D-p-1)$-form. On a contractible patch, the [Poincaré lemma](../../../../../../poincare-lemma.md) gives $*F=dB_q$, hence

$$
\boxed{q_{\rm massless}=D-p-2,\qquad dB=*dA.}
$$

Conversely, the original Bianchi identity becomes the dual field equation $d*dB=0$, up to the harmless signature sign in $**$. The original equation becomes the dual Bianchi identity. This establishes [massless p-form duality](../../../../../../massless-p-form-duality.md) between gauge-equivalence classes of local solutions. It requires $0\le p\le D-2$ for an ordinary dual potential; global flux sectors and sources require extra data.

For a [massive p-form field](../../../../../../massive-p-form-field.md) of mass $m>0$, let $\delta$ denote the formal [codifferential](../../../../../../codifferential.md) and take its free equation to be

$$
\delta F+m^2A=0,\qquad F=dA.
$$

Applying $\delta$ yields $\delta A=0$, since $\delta^2=0$. Define

$$
B_q=\frac1m*F,\qquad\boxed{q_{\rm massive}=D-p-1.}
$$

Here the dual field is the Hodge dual of the field strength itself, rather than a potential for it. For definiteness, use one timelike direction and $**\omega_r=(-1)^{r(D-r)+1}\omega_r$. With $\delta\omega_r=(-1)^{D(r+1)}*d*\omega_r$, write $\eta=(-1)^{D(p+2)}$. The massive equation implies

$$
*dB=-\eta mA,\qquad A=-\frac\eta m*dB.
$$

This gives an invertible differential map at nonzero mass. Also $\delta B=0$ follows from $dF=0$, and substitution yields $\delta dB+m^2B=0$. Indeed the two codifferential signs multiply to $(-1)^{D(p+q+4)}=(-1)^{D(D+3)}=1$. Thus [massive p-form duality](../../../../../../massive-p-form-duality.md) exchanges the equations of two massive tensors of the displayed ranks.

The polarization counts confirm the distinction: a massive tensor in its rest frame has $\binom{D-1}{p}$ states, equal to $\binom{D-1}{D-p-1}$, whereas a massless gauge field has $\binom{D-2}{p}$, equal to $\binom{D-2}{D-p-2}$. The ordinary massive dual applies for $0\le p\le D-1$. A massless $(D-1)$-form has no local wave but may carry a constant top-form flux; its formal negative dual rank is a warning that it is not described by an ordinary dual potential. A degree-$D$ potential likewise has no local propagating field strength. These nondynamical endpoint cases do not change the duality of propagating fields.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
