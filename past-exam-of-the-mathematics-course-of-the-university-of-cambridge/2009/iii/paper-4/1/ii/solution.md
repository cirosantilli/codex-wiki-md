<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We prove closure of $N$ through [character kernels](../../../../../../kernel-of-a-character.md), rather than assuming that a conjugacy-invariant set is a subgroup. Let $\eta\in\operatorname{Irr}(H)\setminus\{1_H\}$, write $d=\eta(1)$, and define the [generalised character](../../../../../../virtual-character.md)

$$
\Psi_\eta=(\eta-d1_H)^G+d1_G.
$$

Here $1_H,1_G$ are the [trivial characters](../../../../../../trivial-character.md). Since $(\eta-d1_H)(1)=0$, part (i) gives $(\Psi_\eta)_H=\eta$ and $\Psi_\eta(1)=d$. Put $\vartheta=\eta-d1_H$. By [Frobenius reciprocity](../../../../../../frobenius-reciprocity.md) and [character orthogonality](../../../../../../character-orthogonality.md),

$$
\langle\vartheta^G,\vartheta^G\rangle_G=\langle\vartheta,(\vartheta^G)_H\rangle_H=\langle\vartheta,\vartheta\rangle_H=1+d^2,\qquad \langle\vartheta^G,1_G\rangle_G=-d.
$$

Consequently

$$
\langle\Psi_\eta,\Psi_\eta\rangle_G=(1+d^2)-2d^2+d^2=1.
$$

To justify the resulting irreducibility, write any [generalised character](../../../../../../virtual-character.md) as an integer combination $\sum_\chi a_\chi\chi$ of [irreducible characters](../../../../../../irreducible-character.md). Its squared norm is $\sum a_\chi^2$, so norm one makes it $\chi$ or $-\chi$ for one irreducible $\chi$. Positive degree rules out the negative sign. Thus $\Psi_\eta$ is an [irreducible character](../../../../../../irreducible-character.md), an instance of the fact that [positive-degree norm-one virtual characters are irreducible](../../../../../../positive-degree-norm-one-virtual-characters-are-irreducible.md).

If $x\in N\setminus\{1\}$, no conjugate of $x$ lies in $H$, so the induction formula gives $\vartheta^G(x)=0$. At $1$ it is also zero. Hence $\Psi_\eta(x)=d$ for all $x\in N$. For a finite-group representation we may choose an invariant positive Hermitian form, making every representing matrix unitary. Its trace equals its dimension only when all its unit-modulus eigenvalues are $1$. Thus the [kernel of a character](../../../../../../kernel-of-a-character.md) is $\{g:\Psi_\eta(g)=\Psi_\eta(1)\}$, and $N\subseteq\ker\Psi_\eta$.

Conversely, if $g\notin N$, then $g$ is conjugate to some $h\in H\setminus\{1\}$. The character of the [regular representation](../../../../../../regular-representation.md) of $H$ is

$$
\rho_H=\sum_{\eta\in\operatorname{Irr}(H)}\eta(1)\eta,\qquad \rho_H(1)=|H|,\qquad \rho_H(h)=0.
$$

If every nontrivial $\eta$ satisfied $\eta(h)=\eta(1)$, the sum at $h$ would instead equal $\sum\eta(1)^2=|H|$, a contradiction. Choose an $\eta$ for which these values differ. Since $\Psi_\eta$ restricts to $\eta$, it has $\Psi_\eta(g)=\eta(h)\ne d$, so $g\notin\ker\Psi_\eta$. Therefore

$$
\boxed{N=\bigcap_{\eta\in\operatorname{Irr}(H)\setminus\{1_H\}}\ker\Psi_\eta\triangleleft G.}
$$

This proves the [Frobenius kernel theorem](../../../../../../frobenius-kernel-theorem.md)'s subgroup assertion. The definition also gives $N\cap H=\{1\}$. Using the permitted cardinality $|N|=[G:H]$, normality ensures $NH$ is a subgroup and

$$
|NH|=\frac{|N||H|}{|N\cap H|}=|G|,\qquad \boxed{NH=G\quad\text{and}\quad G=N\rtimes H.}
$$

Thus $N$ is the [Frobenius kernel](../../../../../../frobenius-kernel.md), and $H$ supplies the complementary factor.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
