<h1 id="21i/solution">Solution</h1>

↑ **Parent:** [21I](../21i.md)

The [Snake lemma](../../../../../snake-lemma.md) associates to a [commutative diagram](../../../../../commutative-diagram.md) with [exact](../../../../../exact-sequence.md) rows an [exact sequence](../../../../../exact-sequence.md)

$$
\ker f_1\to\ker f_2\to\ker f_3
\xrightarrow{\delta}\operatorname{coker}f_1
\to\operatorname{coker}f_2\to\operatorname{coker}f_3.
$$

For $K=L_1\cup L_2$, apply it degree by degree to the short exact sequence of chain complexes

$$
0\to C_*(L_1\cap L_2)
\xrightarrow{c\mapsto(c,-c)}
C_*(L_1)\oplus C_*(L_2)
\xrightarrow{(a,b)\mapsto a+b}
C_*(K)\to0.
$$

The resulting [connecting maps](../../../../../connecting-homomorphism.md) splice the [kernels](../../../../../kernel-of-a-linear-map.md) modulo [boundaries](../../../../../chain-boundary.md) into the [Mayer--Vietoris sequence](../../../../../mayer-vietoris-sequence.md)

$$
\cdots\to H_n(L_1\cap L_2)\to
H_n(L_1)\oplus H_n(L_2)\to H_n(K)
\xrightarrow{\partial}H_{n-1}(L_1\cap L_2)\to\cdots.
$$

Now let $K$ satisfy the stated [simplicial pseudomanifold](../../../../../simplicial-pseudomanifold.md) conditions. In an $n$-[cycle](../../../../../chain-cycle.md), cancellation at a common $(n-1)$-[face](../../../../../face-of-a-simplex.md) determines the [coefficient](../../../../../chain-coefficient.md) of either incident $n$-[simplex](../../../../../simplex.md) from the other, up to the [orientation](../../../../../orientation-of-a-simplex.md) sign. Connectivity through such faces therefore determines every top-simplex coefficient from one [integer](../../../../../integer.md). If the signs are globally compatible, their oriented sum is a cycle and [generates](../../../../../generator-of-a-group.md) $H_n(K)\cong\mathbb Z$; if they are inconsistent, that integer must be zero and $H_n(K)=0$.

Let $x$ be the resulting [fundamental class](../../../../../fundamental-class-of-an-orientable-simplicial-pseudomanifold.md), represented by $z$. Since the intersection has dimension below $n$, split uniquely  
$z=z_1+z_2$ into top chains in $L_1$ and $L_2$. Then

$$
\partial z_1=-\partial z_2\in C_{n-1}(L_1\cap L_2),
$$

and the Mayer--Vietoris boundary is

$$
\boxed{\partial x=[\partial z_1]=-[\partial z_2]}.
$$

It is nonzero exactly when both $L_1$ and $L_2$ contain top-dimensional simplices; if one side contains none, the fundamental cycle already lies in the other side, while if both do, connectedness forces a nonempty interface and its oriented boundary represents a nonzero class.

Finally take $K\cong S^3$, $L_1\cong S^1\times D^2$, and  
$L_1\cap L_2\cong T^2$. The preceding boundary

$$
H_3(S^3)\longrightarrow H_2(T^2)
$$

is a nonzero map between copies of $\mathbb Z$ and sends the fundamental class to the oriented boundary torus, hence is an isomorphism. Exactness then gives

$$
H_2(L_2)=0.
$$

The next part of the sequence is

$$
0\to H_1(T^2)\cong\mathbb Z^2
\to H_1(L_1)\oplus H_1(L_2)
\to0.
$$

Since $H_1(L_1)\cong\mathbb Z$, it follows that  
$H_1(L_2)\cong\mathbb Z$. The degree-zero sequence makes $L_2$ connected. Therefore

$$
\boxed{H_0(L_2)\cong\mathbb Z,\quad
H_1(L_2)\cong\mathbb Z,\quad
H_i(L_2)=0\ (i\geq2)}.
$$

## ↑ Ancestors (10)

1. [21I](../21i.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
