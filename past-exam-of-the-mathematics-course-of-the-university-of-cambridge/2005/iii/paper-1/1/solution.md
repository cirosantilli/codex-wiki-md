<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Work with finite [groups](../../../../../group-split.md), as required for these [Sylow subgroup](../../../../../sylow-subgroup.md) counts. Let $P$ act by [conjugation](../../../../../conjugation.md) on the set of Sylow $p$-subgroups. The [stabilizer](../../../../../stabilizer-subgroup.md) of $Q$ is $P\cap N_G(Q)$. Since $Q$ is the normal [Sylow subgroup](../../../../../sylow-subgroup.md) of its own [normalizer](../../../../../normalizer.md), every $p$-subgroup of that [normalizer](../../../../../normalizer.md) lies in $Q$. Consequently the [stabilizer](../../../../../stabilizer-subgroup.md) is exactly $P\cap Q$, and the [orbit-stabilizer theorem](../../../../../orbit-stabilizer-theorem.md) gives orbit size $[P:P\cap Q]$. The orbit of $P$ has size one. Every other orbit size is a power of $p$ at least $p^a$, hence is divisible by $p^a$. Adding orbit sizes proves the [strengthened Sylow congruence from intersections](../../../../../strengthened-sylow-congruence-from-intersections.md):

$$
\boxed{n_p\equiv1\pmod{p^a}.}
$$

Now suppose $G$ is simple of order $2^e\cdot15$. If $e=0$, its Sylow $5$-subgroup is normal because its number divides three and is one modulo five. If $e=1$, an involution in the regular [permutation action](../../../../../group-action.md) of $G$ swaps fifteen pairs, so its sign is negative. The [sign of a permutation](../../../../../sign-of-a-permutation.md) would give a nontrivial [group homomorphism](../../../../../group-homomorphism.md) $G\to C_2$ with a proper nontrivial normal kernel. Both cases contradict simplicity. Thus $e\ge2$.

The [Sylow theorems](../../../../../sylow-theorems.md) make $n_2$ a divisor of fifteen. It is not one, since a nontrivial [Sylow subgroup](../../../../../sylow-subgroup.md) would then be normal. It is not three, since the [conjugation action](../../../../../conjugation-action.md) on three [Sylow subgroups](../../../../../sylow-subgroup.md) would give a faithful [group homomorphism](../../../../../group-homomorphism.md) $G\hookrightarrow S_3$, impossible by order. If $n_2=5$, take a [Sylow subgroup](../../../../../sylow-subgroup.md) $P$ itself: its [normalizer](../../../../../normalizer.md) has [subgroup index](../../../../../index-of-a-subgroup.md) five. If $n_2=15$, not all distinct [Sylow subgroups](../../../../../sylow-subgroup.md) can intersect $P$ in [subgroup index](../../../../../index-of-a-subgroup.md) at least four, since that would give $15\equiv1\pmod4$. Choose $Q\ne P$ with $[P:P\cap Q]=2$. Put $R=P\cap Q$, of order $2^{e-1}$. It has [subgroup index](../../../../../index-of-a-subgroup.md) two in both $P,Q$, so is normal in each. Hence $N_G(R)$ contains both distinct [Sylow subgroups](../../../../../sylow-subgroup.md) and has order greater than $2^e$. It is proper: otherwise $R$ would be a nontrivial proper [normal subgroup](../../../../../normal-subgroup.md) of $G$. Its order is therefore $2^e\cdot3$ or $2^e\cdot5$. The latter would give an index-three subgroup and again an impossible faithful action on three [cosets](../../../../../coset.md). Thus $[G:N_G(R)]=5$.

In either case we have the requested subgroup of order $2^e$ or $2^{e-1}$ with index-five [normalizer](../../../../../normalizer.md). The action on the five [cosets](../../../../../coset.md) of that [normalizer](../../../../../normalizer.md) is nontrivial and faithful by simplicity. Its image lies in $A_5$, since composing with sign cannot give a nontrivial map from this [simple group](../../../../../simple-group.md) of order greater than two to $C_2$. Thus $2^e\cdot15$ divides $60$, forcing $e=2$ and equality of orders. This proves the [simple groups with order a power of two times fifteen](../../../../../simple-groups-with-order-a-power-of-two-times-fifteen.md) conclusion:

$$
\boxed{G\cong A_5.}
$$

For $SL_2(5)$, choose the first column: there are $5^2-1=24$ nonzero choices. For each, determinant one is a nonzero linear equation in the second column and has five solutions. Therefore $|SL_2(5)|=120$. A central [matrix](../../../../../matrix.md) commuting with $\left(\begin{smallmatrix}1&1\\0&1\end{smallmatrix}\right)$ has zero lower-left entry and equal diagonal entries; commuting also with $\left(\begin{smallmatrix}1&0\\1&1\end{smallmatrix}\right)$ makes the upper-right entry zero. It is scalar. Determinant one then gives

$$
\boxed{|SL_2(5)|=120,\qquad Z=\{I,-I\},\quad |Z|=2.}
$$

To establish the [projective special linear group over the field with five elements](../../../../../projective-special-linear-group-over-the-field-with-five-elements.md) isomorphism without assuming its simplicity, compute its classes. For determinant-one matrices, the [characteristic polynomial](../../../../../characteristic-polynomial.md) is $X^2-tX+1$ with trace $t$. The possibilities over $\mathbb F_5$ exhaust the group:

$$
\begin{array}{c|c|c}
\text{type in }SL_2(5)&\text{centralizer order}&\text{class sizes in }SL_2(5)\\\hline
\pm I&120&1,1\\
t=0&4&30\\
t=1,-1&6&20,20\\
t=2,-2,\ \text{noncentral}&10&12,12,12,12
\end{array}
$$

For trace zero the [eigenvalues](../../../../../eigenvalue.md) are $2,3$, so the determinant-one [centralizer](../../../../../centralizer.md) is the split diagonal torus of order four. For traces $\pm1$, the discriminant is the nonsquare $2$: the [centralizer](../../../../../centralizer.md) is the norm-one subgroup of $\mathbb F_{25}^{\times}$, of order six. In both semisimple cases the determinant map on the full linear [centralizer](../../../../../centralizer.md) is surjective onto $\mathbb F_5^{\times}$; consequently each trace type is a single special-linear class. For the noncentral traces $\pm2$, a [Jordan block](../../../../../jordan-block.md) has full linear [centralizer](../../../../../centralizer.md) $\left\{\left(\begin{smallmatrix}a&b\\0&a\end{smallmatrix}\right):a\ne0\right\}$ with determinant $a^2$. The [determinant](../../../../../determinant.md) image consists of the two squares, so each general-linear class splits into two special-linear classes; the determinant-one [centralizer](../../../../../centralizer.md) has order $2\cdot5=10$. These sizes sum to $120$.

Quotienting by $Z$ identifies a matrix with its negative. The trace-zero class gives one projective class of size fifteen; the two traces $\pm1$ give one class of size twenty; the four noncentral unipotent classes give two classes of size twelve. Their respective projective orders are $2,3,5,5$, by the [characteristic polynomial](../../../../../characteristic-polynomial.md)s. A [normal subgroup](../../../../../normal-subgroup.md) is a union of classes containing the identity. The nontrivial proper possible union sizes are $13,16,21,25,28,33,36,40,45,48$, none of which divides $60$. Thus the quotient is simple. Applying the order-$60$ result above gives

$$
\boxed{PSL_2(5)\cong A_5.}
$$

Finally, if $A^2=I$ over an odd-characteristic field, its [minimal polynomial](../../../../../minimal-polynomial.md) divides the square-free polynomial $(X-1)(X+1)$, so it is diagonalizable with [eigenvalues](../../../../../eigenvalue.md) $\pm1$. In dimension two, determinant one requires both eigenvalues equal. Hence $A=I$ or $A=-I$. This proves the [unique involution in SL2 over an odd field](../../../../../unique-involution-in-sl2-over-an-odd-field.md) assertion: **the only element of order two in $SL_2(5)$ is $-I$**. If an index-two subgroup $H$ existed, it would be normal and have order sixty. By [Cauchy theorem](../../../../../cauchy-s-integral-theorem.md) it would contain an involution, hence contain $Z$. Then $H/Z$ would be a [normal subgroup](../../../../../normal-subgroup.md) of order thirty in the simple quotient $PSL_2(5)$, a contradiction. Thus **$SL_2(5)$ has no index-two subgroup**.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
