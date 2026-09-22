<h1 id="21j/solution">Solution</h1>

↑ **Parent:** [21J](../21j.md)

The [Seifert-van Kampen theorem](../../../../../seifert-van-kampen-theorem.md) says that if $X=U\cup V$, where $U,V,U\cap V$ are path connected [open sets](../../../../../open-set.md) containing $x_0$, then

$$
\pi_1(X,x_0)\cong
\bigl(\pi_1(U,x_0)*\pi_1(V,x_0)\bigr)\big/
\langle\!\langle i_{U*}(\gamma)i_{V*}(\gamma)^{-1}:
\gamma\in\pi_1(U\cap V,x_0)\rangle\!\rangle.
$$

The cell attachment is the quotient

$$
X\cup_fD^n=(X\sqcup D^n)/(u\sim f(u)\text{ for }u\in\partial D^n),
$$

with the image of $x_0=f(*)$ as base point. For $n=2$, take one [open set](../../../../../open-set.md) that deformation retracts onto $X$ together with a boundary collar, and another that consists of the interior of the disc with a collar and is contractible. Their intersection deformation retracts onto $S^1$. Its generator maps to $[f]$ in the first set and to the identity in the second. Van Kampen therefore proves the [fundamental group after attaching a 2-cell](../../../../../fundamental-group-after-attaching-a-2-cell.md) formula

$$
\boxed{\pi_1(X\cup_fD^2,x_0)
\cong\pi_1(X,x_0)/\langle\!\langle[f]\rangle\!\rangle}.
$$

Applying van Kampen to the two circles gives

$$
\pi_1(S^1\vee S^1,*)\cong F(a,b).
$$

Attach three discs along loops representing $a^2$, $b^3$, and $(ab)^2$. The resulting [presentation complex for the symmetric group on three letters](../../../../../presentation-complex-for-the-symmetric-group-on-three-letters.md) has [group](../../../../../group-split.md)

$$
\langle a,b\mid a^2=b^3=(ab)^2=1\rangle.
$$

Sending $a$ to $(12)$ and $b$ to $(123)$ gives a surjection onto $S_3$. The relations imply $aba=b^{-1}$, so every word reduces to one of

$$
1,b,b^2,a,ab,ab^2.
$$

The presented [group](../../../../../group-split.md) has at most six elements and surjects onto the six-element [group](../../../../../group-split.md) $S_3$, so this map is an isomorphism.

## ↑ Ancestors (10)

1. [21J](../21j.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
