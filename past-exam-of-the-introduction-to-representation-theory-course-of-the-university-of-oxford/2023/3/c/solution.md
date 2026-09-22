<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $N=\langle a\rangle$. The relation $bab^{-1}=a^2$ lets every element be expressed as $a^ib^j$ with $0\leq i<7$ and $0\leq j<3$. There are 21 such expressions, so the assumption $|G|=21$ makes them distinct. In particular $a$ has order seven, $b$ has order three, and $N$ is a [normal subgroup](../../../../normal-subgroup.md). This is the [nonabelian group of order 21](../../../../nonabelian-group-of-order-21.md), the [semidirect product](../../../../semidirect-product.md) $C_7\rtimes C_3$ with the action given by multiplication by two modulo seven.

Conjugation by $a$ fixes $N$, while conjugation by $b$ sends $a^i$ to $a^{2i}$. The nonidentity [conjugacy classes](../../../../conjugacy-class.md) inside $N$ are therefore

$$
K_1=\{a,a^2,a^4\},\qquad
K_2=\{a^3,a^5,a^6\}.
$$

For the other elements, direct calculation gives

$$
a^t(a^ib^j)a^{-t}=a^{i+(1-2^j)t}b^j.
$$

When $j=1$ or $2$, the coefficient $1-2^j$ is nonzero modulo seven, so letting $t$ vary gives every member of the [coset](../../../../coset.md) $Nb^j$. These [cosets](../../../../coset.md) cannot merge under [conjugation](../../../../conjugation.md), since $G/N$ is an [abelian group](../../../../abelian-group.md) and conjugation acts trivially on that [quotient group](../../../../quotient-group.md). Thus the five [conjugacy classes](../../../../conjugacy-class.md) have representatives and sizes

$$
\begin{array}{c|ccccc}
\text{representative}&1&a&a^3&b&b^2\\\hline
\text{class size}&1&3&3&7&7
\end{array}.
$$

To find the [linear characters](../../../../linear-character.md), note that the [commutator subgroup](../../../../commutator-subgroup.md) $G'$ contains $bab^{-1}a^{-1}=a$. The [quotient group](../../../../quotient-group.md) $G/N\cong C_3$ is abelian, so $G'\subseteq N$; hence $G'=N$. The [abelianization](../../../../abelianization.md) is $C_3$. With $\omega=e^{2\pi i/3}$, its three [linear characters](../../../../linear-character.md) are

$$
\lambda_j(a)=1,\qquad\lambda_j(b)=\omega^j,\qquad j=0,1,2.
$$

This exhausts the [linear characters](../../../../linear-character.md) because [one-dimensional characters factor through the abelianization](../../../../one-dimensional-characters-factor-through-the-abelianization.md).

For the remaining [irreducible characters](../../../../irreducible-character.md), put $\zeta=e^{2\pi i/7}$ and take the [linear characters](../../../../linear-character.md) $\theta_t$ of $N$ defined by $\theta_t(a)=\zeta^t$. The six nontrivial [linear characters](../../../../linear-character.md) form two orbits under conjugation, with exponent sets $\{1,2,4\}$ and $\{3,5,6\}$. Define the [induced characters](../../../../induced-character.md)

$$
\psi=\operatorname{Ind}_N^G\theta_1,\qquad
\overline\psi=\operatorname{Ind}_N^G\theta_3.
$$

For $a^i\in N$, the [character formula for an induced representation](../../../../character-formula-for-an-induced-representation.md) gives

$$
\psi(a^i)=\zeta^i+\zeta^{2i}+\zeta^{4i},\qquad
\overline\psi(a^i)=\zeta^{3i}+\zeta^{5i}+\zeta^{6i}.
$$

Both vanish outside $N$, since no element outside a [normal subgroup](../../../../normal-subgroup.md) can be conjugate into it. This is [induction from an abelian normal subgroup with a free character orbit](../../../../induction-from-an-abelian-normal-subgroup-with-a-free-character-orbit.md). For completeness, its irreducibility here follows directly from [Frobenius reciprocity](../../../../frobenius-reciprocity.md) and [character orthogonality](../../../../character-orthogonality.md) on the [cyclic group](../../../../cyclic-group.md) $N$:

$$
\langle\psi,\psi\rangle_G
=\langle\theta_1,\operatorname{Res}_N^G\psi\rangle_N
=\langle\theta_1,\theta_1+\theta_2+\theta_4\rangle_N=1.
$$

The same calculation with $\theta_3,\theta_5,\theta_6$ proves that $\overline\psi$ is an [irreducible character](../../../../irreducible-character.md).

Let

$$
\alpha=\zeta+\zeta^2+\zeta^4,\qquad
\beta=\zeta^3+\zeta^5+\zeta^6=\overline\alpha.
$$

The sum of the nontrivial seventh [roots of unity](../../../../root-of-unity.md) gives $\alpha+\beta=-1$. Squaring and reducing exponents modulo seven gives

$$
\alpha^2=\alpha+2\beta=-\alpha-2.
$$

Thus $\alpha,\beta$ are the two [polynomial roots](../../../../root-of-a-polynomial.md) of $T^2+T+2$, and

$$
\alpha=\frac{-1+i\sqrt7}{2},\qquad
\beta=\frac{-1-i\sqrt7}{2}.
$$

To fix the signs with our specified $\zeta$, observe that $\operatorname{Im}\alpha=\sin(2\pi/7)+\sin(3\pi/7)-\sin(\pi/7)>0$, using the increase of sine on $(0,\pi/2)$. These [Gaussian periods for seventh roots of unity](../../../../gaussian-periods-for-seventh-roots-of-unity.md) make the answer explicit.

The resulting [character table](../../../../character-table.md) is

$$
\boxed{\begin{array}{c|ccccc}
&1&a&a^3&b&b^2\\\hline
\text{class size}&1&3&3&7&7\\\hline
\lambda_0&1&1&1&1&1\\
\lambda_1&1&1&1&\omega&\omega^2\\
\lambda_2&1&1&1&\omega^2&\omega\\
\psi&3&\alpha&\beta&0&0\\
\overline\psi&3&\beta&\alpha&0&0
\end{array}.}
$$

The two degree-three [irreducible characters](../../../../irreducible-character.md) are distinct because $\alpha\ne\beta$. Together with the three [linear characters](../../../../linear-character.md), they exhaust the [irreducible characters](../../../../irreducible-character.md): the [sum of squares of irreducible degrees](../../../../sum-of-squares-of-irreducible-degrees.md) is $3\cdot1^2+2\cdot3^2=21=|G|$. Equivalently, we have five distinct [irreducible characters](../../../../irreducible-character.md) for the five [conjugacy classes](../../../../conjugacy-class.md).

As a check on part (b), inversion interchanges $K_1$ and $K_2$, and also interchanges the two [conjugacy classes](../../../../conjugacy-class.md) outside $N$. Only the identity [conjugacy class](../../../../conjugacy-class.md) is real. Correspondingly $\lambda_0$ is the only [real-valued character](../../../../real-valued-character.md) among the [irreducible characters](../../../../irreducible-character.md); $\lambda_1,\lambda_2$ and $\psi,\overline\psi$ are two conjugate pairs.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the introduction to representation theory course of the University of Oxford](../../../split.md)
5. [Introduction to representation theory course of the University of Oxford](../../../../introduction-to-representation-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
