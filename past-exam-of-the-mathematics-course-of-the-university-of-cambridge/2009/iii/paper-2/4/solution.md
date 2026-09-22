<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [special linear group over a finite field](../../../../../special-linear-group-over-a-finite-field.md) $SL_n(q)$ consists of the determinant-one invertible matrices over $\mathbb F_q$. Counting an ordered [basis](../../../../../basis.md) gives

$$
|GL_n(q)|=\prod_{i=0}^{n-1}(q^n-q^i)
=q^{n(n-1)/2}\prod_{j=1}^n(q^j-1).
$$

The [determinant](../../../../../determinant.md) map is onto $\mathbb F_q^*$, so

$$
\boxed{|SL_n(q)|=q^{n(n-1)/2}\prod_{j=2}^n(q^j-1).}
$$

A [transvection](../../../../../transvection.md) has the form $I+vf$, where $v\ne0$, the [linear functional](../../../../../linear-functional.md) $f$ is nonzero and $f(v)=0$. It has [determinant](../../../../../determinant.md) one, fixes the [hyperplane](../../../../../hyperplane.md) $\ker f$ pointwise, and its displacement has image the line $\langle v\rangle$. In particular $E_{ij}(t)=I+te_{ij}$ for $i\ne j$ is an elementary [transvection](../../../../../transvection.md) when $t\ne0$.

Row addition is multiplication by such a [matrix](../../../../../matrix.md). [Gaussian elimination](../../../../../gaussian-elimination.md) reduces a determinant-one [matrix](../../../../../matrix.md) to diagonal form using row additions and determinant-one pivot exchanges. The latter, and all remaining diagonal factors, are themselves products of [transvections](../../../../../transvection.md): within two coordinates,

$$
w(t)=E_{12}(t)E_{21}(-t^{-1})E_{12}(t)=\begin{pmatrix}0&t\\-t^{-1}&0\end{pmatrix},\qquad
w(t)w(-1)=\operatorname{diag}(t,t^{-1}).
$$

A diagonal [matrix](../../../../../matrix.md) with product of entries one is a product of these two-coordinate diagonal matrices. Thus **[transvections](../../../../../transvection.md) generate $SL_n(q)$**. This generation statement actually holds for every $n\ge2$ and every [finite field](../../../../../finite-field.md); the exclusions in the question are needed for the subsequent simplicity assertion.

Commuting with all elementary matrices forces the [group center](../../../../../center-of-a-group.md) to consist of scalar matrices $\lambda I$ with $\lambda^n=1$, so its order is $d=\gcd(n,q-1)$. The projective quotient acts faithfully on the one-dimensional subspaces. Its action is two-transitive: send an ordered pair of independent representative vectors to any other pair and adjust the [determinant](../../../../../determinant.md) by rescaling a representative without changing its line. Therefore it is primitive.

The [Iwasawa simplicity lemma](../../../../../iwasawa-simplicity-lemma.md) says that in a faithful primitive action, if a [point stabilizer](../../../../../stabilizer-subgroup.md) has an abelian [normal subgroup](../../../../../normal-subgroup.md) whose conjugates generate the [group](../../../../../group-split.md), every nontrivial [normal subgroup](../../../../../normal-subgroup.md) contains the derived [subgroup](../../../../../subgroup.md). In particular a nontrivial [perfect group](../../../../../perfect-group.md) satisfying these conditions is simple. No proof of the lemma is required here.

For the point $\ell=\langle v\rangle$, the [subgroup](../../../../../subgroup.md)

$$
U_\ell=\{I+vf:f(v)=0\}
$$

is abelian, is normal in the line stabilizer, and its conjugates contain all [transvections](../../../../../transvection.md). Its image in the projective quotient has the same properties. Perfectness follows explicitly from elementary [commutators](../../../../../commutator.md). If $n\ge3$, choose a third index $r$ to obtain

$$
[E_{ir}(a),E_{rj}(b)]=E_{ij}(ab).
$$

If $n=2,q>3$, choose $t$ with $t^2\ne1$ and set $h(t)=\operatorname{diag}(t,t^{-1})$. Then

$$
[h(t),E_{12}(c)]=E_{12}((t^2-1)c).
$$

Every upper [transvection](../../../../../transvection.md) is a [commutator](../../../../../commutator.md), and [conjugation](../../../../../conjugation.md) gives the lower ones. The [group](../../../../../group-split.md) and its projective quotient are perfect. [Iwasawa's simplicity lemma](../../../../../iwasawa-simplicity-lemma.md) now proves

$$
\boxed{PSL_n(q)\text{ is simple for }n\ge3\text{ or }n=2,\ q>3.}
$$

The order of $PSL_2(4)$ is $4(4^2-1)=60$. Its faithful projective-line action has degree five, so its image is an index-two [subgroup](../../../../../subgroup.md) of $S_5$, necessarily $A_5$. Thus $PSL_2(4)\cong A_5$.

For $PSL_2(5)$ the order is $5(5^2-1)/2=60$. We construct a faithful degree-five action. In $SL_2(5)$ take

$$
i=\begin{pmatrix}2&0\\0&3\end{pmatrix},\qquad
j=\begin{pmatrix}0&1\\4&0\end{pmatrix}.
$$

They satisfy $i^2=j^2=-I$ and $ij=-ji$. Their quaternion [subgroup](../../../../../subgroup.md) projects to a Sylow 2-subgroup $V\cong C_2^2$. Its projective [centralizer](../../../../../centralizer.md) is $V$: a lift of a centralizing element conjugates each of $i,j$ to itself or its negative. In the [matrix](../../../../../matrix.md) [basis](../../../../../basis.md) $I,i,j,ij$, those four sign choices each leave a one-dimensional space, and [determinant](../../../../../determinant.md) one leaves just its two quaternion representatives. The [matrix](../../../../../matrix.md)

$$
r=\frac{-I+i+j+ij}{2}=\begin{pmatrix}3&4\\3&1\end{pmatrix}
$$

has order three and cyclically permutes the three nonidentity elements of $V$. The [normalizer](../../../../../normalizer.md) quotient embeds in $S_3$ and has order dividing both $6$ and $60/4=15$, so it has order exactly three. Hence $|N(V)|=12$ and there are five Sylow 2-subgroups. Their [conjugation](../../../../../conjugation.md) action is nontrivial and transitive, and simplicity makes it faithful. Its image again has order $60$ in $S_5$, proving

$$
\boxed{PSL_2(4)\cong PSL_2(5)\cong A_5.}
$$

Finally,

$$
|PSL_3(4)|=\frac{4^3(4^2-1)(4^3-1)}3=20160,qquad
|PSL_4(2)|=2^6(2^2-1)(2^3-1)(2^4-1)=20160.
$$

In [characteristic two](../../../../../characteristic-two.md) an involutory [matrix](../../../../../matrix.md) has form $I+N$ with $N^2=0$. Its Jordan blocks have size at most two. A projective [involution](../../../../../involution.md) in $PSL_3(4)$ has a unique involutory lift to $SL_3(4)$: its square is central, and squaring is an automorphism of the scalar center of order three, allowing a unique scalar adjustment. The nonidentity Jordan form in [dimension](../../../../../dimension-vector-space.md) three is only $(2,1)$. This GL-class remains a single SL-class, since the [centralizer](../../../../../centralizer.md) contains $\operatorname{diag}(I_2,c)$ of every [determinant](../../../../../determinant.md) $c\in\mathbb F_4^*$. Thus $PSL_3(4)$ has one [involution](../../../../../involution.md) class.

In $PSL_4(2)=SL_4(2)=GL_4(2)$ there are two forms, $(2,1,1)$ and $(2,2)$, so there are two [involution](../../../../../involution.md) classes. More concretely, the first [group](../../../../../group-split.md)'s single class has $21\cdot5\cdot3=315$ elements, counting image line, [kernel](../../../../../kernel-of-a-linear-map.md) plane through it and nonzero map between the quotient and image. The rank-one class in [dimension](../../../../../dimension-vector-space.md) four over $\mathbb F_2$ has $15\cdot7=105$ elements; the rank-two class has $35\cdot|GL_2(2)|=210$. [Isomorphisms](../../../../../isomorphism.md) preserve conjugacy classes, so

$$
\boxed{PSL_3(4)\not\cong PSL_4(2),\quad\text{despite their common order }20160.}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
