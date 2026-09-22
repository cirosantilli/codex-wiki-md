<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

First check the signs directly. For $(x,y)\in M_i$, applying the proposed differential twice gives

$$
d_f^2(x,y)=\left(d_C^2x,\;(-1)^{i-1}f(d_Cx)+(-1)^i d_Df(x)+d_D^2y\right)=(0,0),
$$

because $f$ is a [chain map](../../../../../chain-map.md). Thus $M$ is a [chain complex](../../../../../chain-complex.md).

Let $C'$ be the shifted [chain complex](../../../../../chain-complex.md) with $C'_i=C_{i-1}$ and differential $d_C$; here there is no minus sign in that differential. Inclusion in the second summand and projection onto the first give a [short exact sequence of chain complexes](../../../../../short-exact-sequence-of-chain-complexes.md)

$$
0\longrightarrow D\longrightarrow M\longrightarrow C'\longrightarrow0.
$$

To compute the connecting map in its [long exact sequence in homology](../../../../../long-exact-sequence-in-homology.md), lift a cycle $x\in C_{i-1}$ to $(x,0)\in M_i$. Its boundary is $(0,(-1)^if(x))$. Hence the connecting map $H_i(C')\to H_{i-1}(D)$ is $(-1)^if_*$, and the relevant exact portion is

$$
H_i(C)\xrightarrow{(-1)^{i+1}f_*}H_i(D)\longrightarrow H_i(M)\longrightarrow H_{i-1}(C)\xrightarrow{(-1)^if_*}H_{i-1}(D).
$$

If every $f_*$ is an [isomorphism](../../../../../isomorphism.md), exactness makes $H_i(M)=0$. Conversely, if every $H_i(M)$ is zero, the adjacent exact portions make every $f_*$ both injective and surjective. Therefore

$$
\boxed{H_*(M)=0\quad\Longleftrightarrow\quad f\text{ is a quasi-isomorphism}.}
$$

This is the acyclicity criterion for a [mapping cone](../../../../../mapping-cone-homological-algebra.md), with the degree-dependent signs adjusted to the given convention.

For the assertion about spaces, use the [cellular approximation theorem](../../../../../cellular-approximation-theorem.md) to replace $f$ by a [cellular map](../../../../../cellular-map.md), and take the induced map of the finite free [cellular chain complexes](../../../../../cellular-chain-complex.md). Tensoring these complexes and their cone with $\mathbb F_p$ gives the corresponding mod-$p$ complexes and cone. The same exact-sequence argument works over $\mathbb F_p$, so the assumed [homology](../../../../../homology-split.md) isomorphisms imply

$$
H_i(M\otimes\mathbb F_p)=0\qquad\text{for every }i\text{ and every prime }p.
$$

The [universal coefficient theorem for homology](../../../../../universal-coefficient-theorem-for-homology.md) gives

$$
0\longrightarrow H_i(M)\otimes\mathbb F_p\longrightarrow H_i(M\otimes\mathbb F_p)\longrightarrow\operatorname{Tor}_1^{\mathbb Z}(H_{i-1}(M),\mathbb F_p)\longrightarrow0.
$$

In particular $H_i(M)\otimes\mathbb F_p=0$ for every prime. Each $H_i(M)$ is a [finitely generated abelian group](../../../../../finitely-generated-abelian-group.md). A nonzero free summand would survive tensoring with every $\mathbb F_p$, while a nonzero finite cyclic summand would survive for a prime dividing its order. Thus $H_i(M)=0$ in every degree, by [detection of integral acyclicity modulo primes](../../../../../detection-of-integral-acyclicity-modulo-primes.md). Applying the cone criterion once more proves **the integral homology map is an isomorphism in every degree**. Finite generation is what makes detection by all prime fields sufficient.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
