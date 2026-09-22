<h1 id="19h/solution">Solution</h1>

↑ **Parent:** [19H](../19h.md)

Write a matrix as $(r,b)$, where $r=a^2$ is a nonzero [quadratic residue](../../../../../quadratic-residue.md) modulo $11$. The square subgroup is

$$
Q=\langle4\rangle=\{1,4,5,9,3\}\cong C_5.
$$

Matrix multiplication becomes

$$
(r,b)(s,c)=(rs,b+rc),
\qquad
(r,b)^{-1}=(r^{-1},-r^{-1}b).
$$

Thus $H$ is the [affine semidirect product of cyclic groups of orders eleven and five](../../../../../affine-semidirect-product-of-cyclic-groups-of-orders-eleven-and-five.md)

$$
H\cong(\mathbb F_{11},+)\rtimes Q\cong C_{11}\rtimes C_5.
$$

There are five choices for $r$ and eleven for $b$, so $|H|=55$. It is nonabelian, since

$$
(4,0)(1,1)=(4,4)\ne(4,1)=(1,1)(4,0).
$$

Let

$$
N=\{(1,b):b\in\mathbb F_{11}\}\cong C_{11}.
$$

Conjugation by the complement gives

$$
(r,0)(1,b)(r,0)^{-1}=(1,rb).
$$

Hence the ten nonidentity translations split into the two orbits

$$
T_Q=\{(1,b):b\in Q\},
\qquad
T_N=\{(1,b):b\in2Q\},
$$

each of size five. For $r\ne1$,

$$
(1,t)(r,b)(1,t)^{-1}
=(r,b+(1-r)t).
$$

Since $1-r\ne0$, varying $t$ gives every $b\in\mathbb F_{11}$. Conjugation cannot change $r$ in the abelian quotient $H/N$. Therefore, with

$$
C_k=\{(4^k,b):b\in\mathbb F_{11}\},
\qquad 1\leq k\leq4,
$$

the seven conjugacy classes are

$$
\{1\},\quad T_Q,\quad T_N,\quad C_1,\quad C_2,\quad C_3,\quad C_4,
$$

of sizes $1,5,5,11,11,11,11$, agreeing with the [conjugacy classes in the affine semidirect product of orders eleven and five](../../../../../conjugacy-classes-in-the-affine-semidirect-product-of-orders-eleven-and-five.md).

The commutators with $(4,0)$ generate every translation because multiplication by $4-1=3$ is invertible in $\mathbb F_{11}$. Hence the [commutator subgroup](../../../../../commutator-subgroup.md) is $N$, and the [abelianization](../../../../../abelianization.md) is

$$
H^{\mathrm{ab}}\cong H/N\cong C_5.
$$

Put $\zeta=e^{2\pi i/5}$. The [one-dimensional characters factor through the abelianization](../../../../../one-dimensional-characters-factor-through-the-abelianization.md), giving five characters

$$
\chi_j(4^k,b)=\zeta^{jk},
\qquad 0\leq j\leq4.
$$

For the remaining characters, put $\omega=e^{2\pi i/11}$ and define a character of $N$ by

$$
\theta_m(1,b)=\omega^{mb}.
$$

The complement has two free orbits on the nontrivial $\theta_m$, indexed by $m\in Q$ and $m\in2Q$. By [induction from an abelian normal subgroup with a free character orbit](../../../../../induction-from-an-abelian-normal-subgroup-with-a-free-character-orbit.md), the characters

$$
\psi_Q=\operatorname{Ind}_N^H\theta_1,
\qquad
\psi_N=\operatorname{Ind}_N^H\theta_2
$$

are irreducible of degree five and vanish outside $N$.

Set

$$
\eta=\sum_{q\in Q}\omega^q
=\frac{-1+i\sqrt{11}}2.
$$

The [quadratic periods modulo eleven](../../../../../quadratic-periods-modulo-eleven.md) give the nonsquare sum $\overline\eta=(-1-i\sqrt{11})/2$. Multiplication by a square preserves $Q$ and multiplication by a nonsquare exchanges the two square classes, so the complete [character table](../../../../../character-table.md) is

$$
\begin{array}{c|ccc|cccc}
 &1&T_Q&T_N&C_1&C_2&C_3&C_4\\
\text{class size}&1&5&5&11&11&11&11\\ \hline
\chi_0&1&1&1&1&1&1&1\\
\chi_1&1&1&1&\zeta&\zeta^2&\zeta^3&\zeta^4\\
\chi_2&1&1&1&\zeta^2&\zeta^4&\zeta&\zeta^3\\
\chi_3&1&1&1&\zeta^3&\zeta&\zeta^4&\zeta^2\\
\chi_4&1&1&1&\zeta^4&\zeta^3&\zeta^2&\zeta\\
\psi_Q&5&\eta&\overline\eta&0&0&0&0\\
\psi_N&5&\overline\eta&\eta&0&0&0&0
\end{array}.
$$

Finally,

$$
5\cdot1^2+2\cdot5^2=55=|H|,
$$

and there are seven rows for the seven conjugacy classes. Thus these are all irreducible characters, as described by the [irreducible characters of the affine semidirect product of orders eleven and five](../../../../../irreducible-characters-of-the-affine-semidirect-product-of-orders-eleven-and-five.md).

## ↑ Ancestors (10)

1. [19H](../19h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
