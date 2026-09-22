<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

We prove the [Birkhoff–Grothendieck theorem](../../../../../birkhoff-grothendieck-theorem.md) by induction on the rank of the [vector bundle](../../../../../vector-bundle.md) $E$. Rank zero is immediate; rank one is the classification $\operatorname{Pic}(\mathbb P^1_k)\cong\mathbb Z$ established above.

First there is a largest integer $a$ with $H^0(E(-a))\ne0$. To see existence and boundedness directly, trivialize $E$ on the two standard affine charts: the associated finite projective modules over the [principal ideal domains](../../../../../principal-ideal-domain.md) $k[t]$ and $k[t^{-1}]$ are free. Let $A(t)\in GL_r(k[t,t^{-1}])$ be its transition matrix, so a section of $E(-a)$ is a pair satisfying

$$
p(t)=t^{-a}A(t)q(t^{-1}),\qquad p\in k[t]^r,\quad q\in k[t^{-1}]^r.
$$

If $a$ exceeds the largest exponent in any entry of $A$, the right side has only strictly negative powers; the left side has nonnegative powers. Hence both vanish. For $a$ sufficiently negative, take a nonzero constant vector $p$ and put $q=t^aA(t)^{-1}p$; all its exponents are nonpositive, so it supplies a nonzero section. Thus a largest $a$ exists.

Such a section gives a nonzero map $\mathcal O(a)\to E$. It is injective, since it is nonzero generically and the source is torsion-free. Saturate its image. The resulting [line subbundle](../../../../../line-subbundle.md) is $\mathcal O(a+d)$ for the degree $d\geq0$ of the [effective divisor](../../../../../effective-cartier-divisor.md) of zeros of the original map. If $d>0$, its inclusion in $E$ would give a nonzero section of $E(-a-d)$, contradicting maximality. Therefore $d=0$ and

$$
0\longrightarrow\mathcal O(a)\longrightarrow E\longrightarrow Q\longrightarrow0
$$

has a [locally free](../../../../../locally-free-sheaf.md) quotient. By induction, $Q\cong\bigoplus_j\mathcal O(b_j)$.

Twist this exact sequence by $\mathcal O(-a-1)$. The outer groups $H^0(\mathcal O(-1))$ and $H^1(\mathcal O(-1))$ are zero by the [Čech cohomology of twists on the projective line](../../../../../cech-cohomology-of-twists-on-the-projective-line.md). The [long exact sequence in sheaf cohomology](../../../../../long-exact-sequence-in-sheaf-cohomology.md) therefore gives

$$
H^0(E(-a-1))\cong H^0(Q(-a-1)).
$$

The first is zero by the choice of $a$, so each $H^0(\mathcal O(b_j-a-1))$ vanishes. Thus $b_j\leq a$ for every $j$. The extension class lies in

$$
\operatorname{Ext}^1(Q,\mathcal O(a))\cong\bigoplus_jH^1(\mathcal O(a-b_j))=0,
$$

since $a-b_j\geq0$. The identification of this [Ext functor](../../../../../ext-functor.md) with cohomology can be seen without additional duality: local splittings of a vector-bundle extension differ by a [Čech cocycle](../../../../../cech-cocycle-condition.md) in $\mathcal H om(Q,\mathcal O(a))$, and a [coboundary](../../../../../coboundary.md) changes them to compatible splittings. Vanishing therefore gives a global splitting. Consequently

$$
\boxed{E\cong\mathcal O(a)\oplus\bigoplus_j\mathcal O(b_j),}
$$

completing the induction over any [field](../../../../../field.md) $k$.

The degrees can be arranged in nonincreasing order and their multiset is unique. Indeed, for any such decomposition,

$$
h^0(E(m))-h^0(E(m-1))=\#\{i:a_i\geq-m\},
$$

so the dimensions of the twisted [global sections](../../../../../global-section.md) recover the number of summands of every degree.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 23](../../paper-23-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
