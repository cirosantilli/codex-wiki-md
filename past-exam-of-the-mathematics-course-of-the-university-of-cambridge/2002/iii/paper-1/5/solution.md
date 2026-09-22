<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Write $x_{ij}(t)=I+tE_{ij}$ for $i\ne j$ and $t\in\mathbb F_q$. When $t\ne0$ these are [transvections](../../../../../transvection.md), and their inverses are $x_{ij}(-t)$. Row addition by such an [elementary transvection matrix](../../../../../elementary-transvection-matrix.md) preserves the [determinant](../../../../../determinant.md). It also realizes signed interchanges and compensating diagonal scalings: in any two coordinate positions,

$$
w(a)=\begin{pmatrix}1&a\\0&1\end{pmatrix}
\begin{pmatrix}1&0\\-a^{-1}&1\end{pmatrix}
\begin{pmatrix}1&a\\0&1\end{pmatrix}
=\begin{pmatrix}0&a\\-a^{-1}&0\end{pmatrix},\qquad
w(a)w(-1)=\begin{pmatrix}a&0\\0&a^{-1}\end{pmatrix}.
$$

Thus elimination can reduce any invertible [matrix](../../../../../matrix.md) to diagonal form using only row additions and signed interchanges, all products of [transvections](../../../../../transvection.md). For a diagonal [matrix](../../../../../matrix.md) with determinant one, $\operatorname{diag}(d_1,\ldots,d_n)$, use the displayed two-coordinate diagonal [matrices](../../../../../matrix.md) in positions $(i,n)$ with parameter $d_i$, for $1\leq i<n$. Their product has diagonal entries $d_1,\ldots,d_{n-1},\prod_{i<n}d_i^{-1}=d_n$. Hence the residual diagonal [matrix](../../../../../matrix.md) is also a product of [transvections](../../../../../transvection.md), and reversing elimination proves

$$
\boxed{SL_n(q)=\langle x_{ij}(t):i\ne j,\ t\in\mathbb F_q\rangle.}
$$

This proves [transvections generate the special linear group](../../../../../transvections-generate-the-special-linear-group.md), including the small fields.

For perfectness, use the convention $[x,y]=xyx^{-1}y^{-1}$ in the following calculations. If $n\geq3$ and $i,j,k$ are distinct, direct [matrix](../../../../../matrix.md) multiplication gives

$$
[x_{ik}(a),x_{kj}(b)]=x_{ij}(ab).
$$

Taking $b=1$ puts every elementary generator in the [commutator subgroup](../../../../../commutator-subgroup.md). Thus $SL_n(q)$ is [perfect](../../../../../perfect-group.md). When $n=2$ and $q>3$, choose $s\in\mathbb F_q^\times$ with $s^2\ne1$; such an element exists because a degree-two polynomial has at most two roots and $q-1>2$. For $D=\operatorname{diag}(s,s^{-1})$,

$$
[D,x_{12}(t)]=x_{12}((s^2-1)t),\qquad
[D,x_{21}(t)]=x_{21}((s^{-2}-1)t).
$$

Both coefficients are nonzero, so varying $t$ supplies every upper and lower elementary generator as a commutator. Therefore

$$
\boxed{SL_n(q)\text{ is perfect for }n\geq3\text{ or }(n=2,q>3).}
$$

The exceptions really fail: $SL_2(2)\cong S_3$ has a nontrivial sign quotient, and $SL_2(3)$ has quotient $PSL_2(3)\cong A_4$, which has the nontrivial [Abelian](../../../../../abelian-group.md) quotient $A_4/V_4\cong C_3$. For the latter identification, the faithful projective action embeds the order-twelve [group](../../../../../group-split.md) $PSL_2(3)$ as an index-two [subgroup](../../../../../subgroup.md) of $S_4$, necessarily $A_4$.

The [Iwasawa simplicity lemma](../../../../../iwasawa-simplicity-lemma.md) states that, in a faithful [primitive group action](../../../../../primitive-group-action.md), if a point stabilizer has an [Abelian](../../../../../abelian-group.md) [normal subgroup](../../../../../normal-subgroup.md) whose conjugates generate the whole [group](../../../../../group-split.md), then every nontrivial [normal subgroup](../../../../../normal-subgroup.md) contains the [commutator subgroup](../../../../../commutator-subgroup.md). In particular a nontrivial perfect [group](../../../../../group-split.md) with this property is simple. The lemma is applied here, as allowed, without assuming the desired simplicity theorem.

Let $SL_n(q)$ act on the one-dimensional subspaces of $\mathbb F_q^n$. This action is [two-transitive](../../../../../two-transitive-group-action.md): a linear map taking two specified distinct lines to two others can be made determinant one by rescaling one of the target basis [vectors](../../../../../vector.md), without changing either target line. Its kernel consists exactly of scalar [matrices](../../../../../matrix.md). Indeed fixing all lines makes a [matrix](../../../../../matrix.md) diagonal in any fixed basis, and fixing the lines through $e_i+e_j$ makes all its diagonal entries equal. The scalar [matrices](../../../../../matrix.md) in $SL_n(q)$ are $aI$ with $a^n=1$. They also form its [group center](../../../../../center-of-a-group.md), since a central [matrix](../../../../../matrix.md) commutes with every elementary generator, forcing all off-diagonal entries to vanish and all diagonal entries to agree. Their number is $\gcd(n,q-1)$. Consequently the quotient $PSL_n(q)$ acts faithfully and primitively.

Fix a line $L=\langle v\rangle$ and consider

$$
T_L=\{I+vf:f\in(\mathbb F_q^n)^*,\ f(v)=0\}.
$$

Here $vf$ is the rank-at-most-one map $z\mapsto f(z)v$. These [matrices](../../../../../matrix.md) have determinant one, and $(vf)(vh)=0$, so $T_L$ is [Abelian](../../../../../abelian-group.md) under addition of the functionals. If $gL=L$, then $gv=av$ and $g(I+vf)g^{-1}=I+av(fg^{-1})\in T_L$. Thus $T_L$ is normal in the line stabilizer. Its image in $PSL_n(q)$ is a nontrivial [Abelian](../../../../../abelian-group.md) [normal subgroup](../../../../../normal-subgroup.md) of the point stabilizer. Conjugates of these [groups](../../../../../group-split.md) include every elementary [transvection](../../../../../transvection.md), hence generate $PSL_n(q)$. Perfectness passes to a quotient. The [Iwasawa simplicity lemma](../../../../../iwasawa-simplicity-lemma.md) therefore gives

$$
\boxed{PSL_n(q)\text{ is simple unless }(n,q)=(2,2),(2,3).}
$$

In those exceptions the projective [groups](../../../../../group-split.md) are $S_3$ and $A_4$, as above.

For $q=4$, counting columns gives $|SL_2(4)|=4(4^2-1)=60$. Its scalar [group center](../../../../../center-of-a-group.md) is trivial, so $PSL_2(4)$ has order sixty. Its faithful action on the five points of the [projective line](../../../../../projective-line.md) embeds it in $S_5$. Because it is perfect, its sign homomorphism is trivial and its image lies in $A_5$. Equal orders then give

$$
\boxed{PSL_2(4)\cong A_5.}
$$

For $q=5$, use an explicit [subgroup](../../../../../subgroup.md) to obtain a five-point action. In $SL_2(5)$ set

$$
i=\begin{pmatrix}0&1\\4&0\end{pmatrix},\qquad
j=\begin{pmatrix}2&0\\0&3\end{pmatrix},\qquad
r=\begin{pmatrix}3&2\\1&1\end{pmatrix}.
$$

All three have determinant one. [Matrix](../../../../../matrix.md) multiplication gives $i^2=j^2=-I$, $ij=-ji$, and $r^3=I$. The eight distinct [matrices](../../../../../matrix.md) $\{\pm I,\pm i,\pm j,\pm ij\}$ form a [quaternion group](../../../../../quaternion-group.md). Moreover,

$$
r i r^{-1}=ij,\qquad r(ij)r^{-1}=j,\qquad r j r^{-1}=i.
$$

Thus $r$ normalizes that quaternion [group](../../../../../group-split.md) and has order three. Their generated [subgroup](../../../../../subgroup.md) has order $24$ and contains the scalar [group center](../../../../../center-of-a-group.md) $\{\pm I\}$. Its image in $PSL_2(5)$ has order twelve, hence index five since $|PSL_2(5)|=5(25-1)/2=60$. The resulting [coset](../../../../../coset.md) action is nontrivial and, by the simplicity already proved, faithful. Perfectness again puts its image in $A_5$, and equal orders imply

$$
\boxed{PSL_2(5)\cong A_5.}
$$

This is the [quaternion construction of an index-five subgroup of PSL2 over F5](../../../../../quaternion-construction-of-an-index-five-subgroup-of-psl2-over-f5.md); it avoids assuming a classification of [groups](../../../../../group-split.md) of order sixty.

For the last comparison, the [order of a general linear group over a finite field](../../../../../order-of-a-general-linear-group-over-a-finite-field.md) comes from choosing independent columns:

$$
|GL_n(q)|=\prod_{i=0}^{n-1}(q^n-q^i).
$$

The determinant map onto $\mathbb F_q^\times$ has kernel $SL_n(q)$, and the scalar quotient divides by $\gcd(n,q-1)$. Hence

$$
|PSL_4(2)|=(16-1)(16-2)(16-4)(16-8)=20160,
$$



$$
|PSL_3(4)|=\frac{(64-1)(64-4)(64-16)}{(4-1)\gcd(3,3)}=20160.
$$

The highest power of two dividing either order is $64$. Their Sylow $2$-subgroups are respectively the [upper unitriangular groups](../../../../../upper-unitriangular-group.md) $U_4(2)$ of order $2^6$ and the image of $U_3(4)$ of order $4^3$. The latter image is isomorphic to $U_3(4)$ because its intersection with the odd-order scalar [group center](../../../../../center-of-a-group.md) is trivial.

The [center of an upper unitriangular group](../../../../../center-of-an-upper-unitriangular-group.md) can be computed directly here. Commuting $X\in U_4(2)$ with $I+E_{12}$ forces $X_{23}=X_{24}=0$; commuting with $I+E_{23}$ forces $X_{12}=X_{34}=0$; commuting with $I+E_{34}$ forces $X_{13}=0$. Only $X_{14}$ can remain, and those [matrices](../../../../../matrix.md) commute with the whole [group](../../../../../group-split.md). Thus $Z(U_4(2))=\{I+tE_{14}:t\in\mathbb F_2\}$ has order two. In $U_3(4)$, commutation with $I+E_{12}$ and $I+E_{23}$ similarly forces $X_{23}=X_{12}=0$, leaving the arbitrary entry $X_{13}\in\mathbb F_4$. Its [group center](../../../../../center-of-a-group.md) has order four. An isomorphism of the whole [groups](../../../../../group-split.md) would send a [Sylow subgroup](../../../../../sylow-subgroup.md) to a [Sylow subgroup](../../../../../sylow-subgroup.md) and preserve its [group center](../../../../../center-of-a-group.md) order, which is impossible. Therefore

$$
\boxed{|PSL_4(2)|=|PSL_3(4)|=20160,\qquad PSL_4(2)\not\cong PSL_3(4).}
$$

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
