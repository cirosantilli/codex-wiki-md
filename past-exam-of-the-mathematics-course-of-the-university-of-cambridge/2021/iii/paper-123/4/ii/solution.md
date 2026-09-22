<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $s=\sqrt{-6}$, so $\mathcal O_K=\mathbb Z[s]$ and $\mathcal O_K^\times=\{\pm1\}$. The primes $2$ and $3$ are ramified:

$$
(2)=\mathfrak p_2^2,
\qquad
(3)=\mathfrak p_3^2.
$$

Thus the finite modulus in the question is

$$
\mathfrak m=\mathfrak p_2^2\mathfrak p_3^2=(6).
$$

The [ray class exact sequence](../../../../../../ray-class-exact-sequence.md), with no real component in the modulus, gives

$$
\mathcal O_K^\times\longrightarrow
(\mathcal O_K/(6))^\times\longrightarrow
\operatorname{Cl}_{\mathfrak m}(K)\longrightarrow
\operatorname{Cl}(K)\longrightarrow1.
$$

The [Chinese remainder theorem for unit groups](../../../../../../chinese-remainder-theorem-for-unit-groups.md) and the ramification relations yield

$$
\begin{aligned}
(\mathcal O_K/(6))^\times
&\simeq(\mathcal O_K/(2))^\times\times(\mathcal O_K/(3))^\times\\
&\simeq\bigl(\mathbb F_2[\epsilon]/(\epsilon^2)\bigr)^\times
\times\bigl(\mathbb F_3[\epsilon]/(\epsilon^2)\bigr)^\times\\
&\simeq C_2\times C_6.
\end{aligned}
$$

The image of $-1$ kills the $C_2$ coming from $\mathbb F_3^\times$. Consequently the kernel of the map from the ray class group to the ordinary class group is

$$
(\mathcal O_K/(6))^\times/\{\pm1\}\simeq C_2\times C_3\simeq C_6.
$$

Since the given [class number](../../../../../../class-number.md) is two, $|\operatorname{Cl}_{\mathfrak m}(K)|=12$.

It remains to distinguish $C_{12}$ from $C_6\times C_2$. Let

$$
\mathfrak q=(5,s-2).
$$

The prime $5$ splits in $K$, and $\mathfrak q$ represents the nontrivial ordinary ideal class because no element of $\mathbb Z[s]$ has norm $5$. Direct multiplication, or comparison of norms and valuations at the two primes over $5$, gives

$$
\mathfrak q^2=(1+2s).
$$

Modulo $2$, the element $1+2s$ is $1$. Modulo $3$, its class $1+2\epsilon$ is nontrivial and has order three because $\epsilon^2=0$. Hence the ray class of $\mathfrak q$ has order six: its square is a nontrivial element of order three in the congruence kernel. The remaining order-two factor of that kernel, coming from $(\mathcal O_K/(2))^\times$, is independent of $\langle[\mathfrak q]\rangle$. Therefore

$$
\boxed{\operatorname{Cl}_{\mathfrak m}(\mathbb Q(\sqrt{-6}))\simeq C_6\times C_2.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 123](../../../paper-123-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
