<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $A=\mathbb C[x,y,z]$. This [polynomial ring](../../../../../polynomial-ring.md) is a [unique factorization domain](../../../../../unique-factorization-domain.md) of [Krull dimension](../../../../../krull-dimension.md) three. For a [height-one prime in a unique factorization domain](../../../../../height-one-prime-in-a-unique-factorization-domain.md) $\mathfrak p$, choose a nonzero element of it and an irreducible factor $q$ belonging to $\mathfrak p$. In a [unique factorization domain](../../../../../unique-factorization-domain.md), $q$ is prime, so $(q)$ is a nonzero [prime ideal](../../../../../prime-ideal.md) contained in $\mathfrak p$. Strict containment would give a chain $(0)\subsetneq(q)\subsetneq\mathfrak p$ of length two. Thus

$$
\boxed{\operatorname{ht}\mathfrak p=1\Longrightarrow\mathfrak p=(q)}.
$$

If $\mathfrak p$ has height three, it is maximal: any strictly larger proper prime would extend a length-three chain and contradict $\dim A=3$. The [Weak Hilbert Nullstellensatz](../../../../../weak-hilbert-nullstellensatz.md) over the [algebraically closed field](../../../../../algebraically-closed-field.md) $\mathbb C$ then gives

$$
\boxed{\operatorname{ht}\mathfrak p=3\Longrightarrow\mathfrak p=(x-a,y-b,z-c)}
$$

for some $a,b,c\in\mathbb C$. This proves both requested generator assertions.

For the [monomial curve with exponents three, four and five](../../../../../monomial-curve-with-exponents-three-four-and-five.md), put

$$
g_1=y^2-xz,\qquad g_2=yz-x^3,\qquad g_3=z^2-x^2y,\qquad J=(g_1,g_2,g_3).
$$

All three map to zero under the given parametrization, so $J\subseteq I=\ker\varphi$. Reduce any [monomial](../../../../../monomial.md) using $y^2\mapsto xz$, $yz\mapsto x^3$ and $z^2\mapsto x^2y$. Each reduction decreases the sum of the exponents of $y,z$, so it terminates. Every polynomial has, modulo $J$, the form

$$
A_0(x)+A_1(x)y+A_2(x)z.
$$

Its image is $A_0(t^3)+t^4A_1(t^3)+t^5A_2(t^3)$. These three terms occupy different exponent classes modulo three, so they cannot cancel. A zero image forces each $A_i=0$. Consequently

$$
\boxed{I=(y^2-xz,\ yz-x^3,\ z^2-x^2y)}.
$$

The quotient is the domain $\mathbb C[t^3,t^4,t^5]$, hence $I$ is a [prime ideal](../../../../../prime-ideal.md). It is finite free over $\mathbb C[t^3]$, with [basis of a module](../../../../../basis-of-a-module.md) $1,t^4,t^5$, by the same normal-form argument. Its dimension is therefore one, using that integral extensions preserve [Krull dimension](../../../../../krull-dimension.md). The [polynomial-ring height and dimension formula](../../../../../polynomial-ring-height-and-dimension-formula.md) gives

$$
\boxed{\operatorname{ht}I=3-\dim(A/I)=2}.
$$

For the generator obstruction, let $\mathfrak m=(x,y,z)$. Since $I\subseteq\mathfrak m^2$, we have $\mathfrak mI\subseteq\mathfrak m^3$. The degree-two initial forms of $g_1,g_2,g_3$ are

$$
y^2-xz,\qquad yz,\qquad z^2.
$$

They are [linearly independent](../../../../../linear-independence.md) over $\mathbb C$ in $\mathfrak m^2/\mathfrak m^3$. Thus no nonzero constant linear combination of the $g_i$ belongs to $\mathfrak mI$, and their classes are independent in $I/\mathfrak mI$. Since the three generators span that quotient,

$$
\boxed{\dim_{\mathbb C}I/\mathfrak mI=3}.
$$

Two global generators would span it by two vectors, which is impossible. This is the [initial-form lower bound for ideal generators](../../../../../initial-form-lower-bound-for-ideal-generators.md); it shows why height two does not force two generators, even though height one and height three behave as above.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
