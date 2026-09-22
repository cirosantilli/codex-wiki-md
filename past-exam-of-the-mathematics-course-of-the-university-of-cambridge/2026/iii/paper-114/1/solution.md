<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Because every $C_i$ is free abelian, reduction modulo $n$ gives a short exact sequence of [chain complexes](../../../../../chain-complex.md)

$$
0\longrightarrow C_\bullet\xrightarrow{\ n\ }C_\bullet\xrightarrow{\rho}C_\bullet\otimes\mathbb Z/n\longrightarrow0.
$$

Its [long exact sequence in homology](../../../../../long-exact-sequence-in-homology.md) is

$$
\cdots\to H_i(C)\xrightarrow{n}H_i(C)\xrightarrow{\rho_*}H_i(C\otimes\mathbb Z/n)\xrightarrow{\widehat\beta}H_{i-1}(C)\to\cdots.
$$

If $\bar z$ is a cycle modulo $n$, choose a lift $z\in C_i$. Then $dz=nw$ for some $w\in C_{i-1}$, and the [connecting homomorphism](../../../../../connecting-homomorphism.md) is $\widehat\beta[\bar z]=[w]$.

The coefficient sequence

$$
0\longrightarrow\mathbb Z/n\xrightarrow{[a]\mapsto[na]}\mathbb Z/n^2\xrightarrow{[b]\mapsto[b]\bmod n}\mathbb Z/n\longrightarrow0
$$

similarly gives

$$
\cdots\to H_i(C\otimes\mathbb Z/n)\to H_i(C\otimes\mathbb Z/n^2)\to H_i(C\otimes\mathbb Z/n)\xrightarrow{\beta}H_{i-1}(C\otimes\mathbb Z/n)\to\cdots.
$$

At chain level, if $z$ lifts a mod-$n$ cycle and $dz=nw$ modulo $n^2$, then the [Bockstein homomorphism](../../../../../bockstein-homomorphism.md) is $\beta[\bar z]=[\bar w]$.

There is a morphism from the first short exact sequence to the second whose three vertical maps are reduction modulo $n$, reduction modulo $n^2$, and the identity on $C\otimes\mathbb Z/n$. Naturality of connecting homomorphisms gives

$$
\beta=\rho_*\widehat\beta.
$$

Exactness of the first long exact sequence says $\widehat\beta\rho_*=0$, and hence

$$
\beta^2=\rho_*\widehat\beta\rho_*\widehat\beta=0.
$$

For the standard cellular chain complex of [Real projective space](../../../../../real-projective-space.md) $\mathbb{RP}^3$, there is one copy of $\mathbb Z$ in degrees $0,1,2,3$, with $d_2=2$ and $d_1=d_3=0$. Modulo two all cellular differentials vanish, while the Bockstein is the identity from degree two to degree one and zero elsewhere. Therefore

$$
\beta H_i(C_*(\mathbb{RP}^3);2)\cong
\begin{cases}
\mathbb Z/2,&i=0,3,\\
0,&i=1,2.
\end{cases}
$$

Finally, Smith normal form decomposes a bounded chain complex of finitely generated free abelian groups, up to chain isomorphism and contractible summands, into one-term complexes $\mathbb Z[i]$ and two-term complexes

$$
0\longrightarrow\mathbb Z\xrightarrow{m}\mathbb Z\longrightarrow0
$$

in degrees $i+1$ and $i$. The former represents a free homology summand, and the latter represents $\mathbb Z/m$ in degree $i$. The two requested conclusions now follow from the next two parts.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 114](../../paper-114-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
