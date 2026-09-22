<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Factor the odd parameter on the left, $\delta=\epsilon s$. The resulting [left-acting BRST differential](../../../../../../left-acting-brst-differential.md) obeys the [graded Leibniz rule](../../../../../../graded-leibniz-rule.md)

$$
s(XY)=(sX)Y+(-1)^{|X|}X(sY).
$$

For the odd [Grassmann field](../../../../../../grassmann-field.md) $c$, the bracket in the transformation is a [graded commutator](../../../../../../graded-commutator.md): $[c,c]_{\rm gr}=2c^2$, not the identically zero ordinary commutator of a matrix with itself. Thus $sc=ic^2$, while $sA_\mu=D_\mu c$, $s\bar c=h$ and $sh=0$.

On the ghost,

$$
s^2c=i[(sc)c-c(sc)]=i[ic^2c-ic c^2]=0.
$$

On the gauge field, variation of the connection and the [adjoint covariant derivative](../../../../../../adjoint-covariant-derivative.md) gives

$$
s^2A_\mu=D_\mu(sc)-i[sA_\mu,c]_{\rm gr}
=iD_\mu(c^2)-i[(D_\mu c)c+c(D_\mu c)]=0.
$$

Here $D_\mu$ is even and therefore obeys the ordinary product rule. Also $s^2\bar c=sh=0$ and $s^2h=0$, without using any field equation; this is off-shell nilpotence supplied by the [Nakanishi-Lautrup field](../../../../../../nakanishi-lautrup-field.md).

Applying the [graded Leibniz rule](../../../../../../graded-leibniz-rule.md) twice cancels the two cross terms:

$$
s^2(XY)=(s^2X)Y+Xs^2Y.
$$

The square is consequently an even [graded derivation](../../../../../../graded-derivation.md). Since it vanishes on every generator, it vanishes inductively on every polynomial in the fields. Hence **$s^2\mathcal O=0$ for every such operator**. This genuine result is stronger than the automatic vanishing obtained by merely setting $\epsilon^2=0$; two independent transformation parameters also give a vanishing commutator.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
