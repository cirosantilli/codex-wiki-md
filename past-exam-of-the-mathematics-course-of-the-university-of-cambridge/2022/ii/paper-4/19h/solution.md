<h1 id="19h/solution">Solution</h1>

↑ **Parent:** [19H](../19h.md)

The [Mackey restriction formula](../../../../../mackey-restriction-formula.md) says, for an $H$-representation $V$,

$$
\operatorname{Res}_H^G\operatorname{Ind}_H^GV
\cong
\bigoplus_{x\in H\backslash G/H}
\operatorname{Ind}_{H\cap xHx^{-1}}^H
\operatorname{Res}_{H\cap xHx^{-1}}^{xHx^{-1}}({}^xV).
$$

[Frobenius reciprocity](../../../../../frobenius-reciprocity.md) says

$$
\langle\operatorname{Ind}_H^G\alpha,\beta\rangle_G
=
\langle\alpha,\operatorname{Res}_H^G\beta\rangle_H.
$$

Applying both with an irreducible character $\chi$ gives

$$
\left\langle
\operatorname{Ind}_H^G\chi,
\operatorname{Ind}_H^G\chi
\right\rangle_G
=
\sum_{x\in H\backslash G/H}
\left\langle
\operatorname{Res}_{H\cap xHx^{-1}}\chi,
\operatorname{Res}_{H\cap xHx^{-1}}({}^x\chi)
\right\rangle.
$$

The identity double coset contributes one, and all terms are nonnegative integers. Therefore [Mackey irreducibility criterion](../../../../../mackey-irreducibility-criterion.md) says that $\operatorname{Ind}_H^G\chi$ is irreducible exactly when every term belonging to a nonidentity double coset is zero.

Now take $G=SL_2(k)$. Write

$$
U=\left\{
\begin{pmatrix}1&b\\0&1\end{pmatrix}:b\in k
\right\},
\qquad
T=\left\{
\begin{pmatrix}a&0\\0&a^{-1}\end{pmatrix}:a\in k^\times
\right\},
$$

so $B=T\ltimes U$. For $q\geq4$, commutators of $T$ with $U$ generate $U$, because conjugation sends $u(b)$ to $u(a^2b)$ and one can choose $a^2\ne1$. Every degree-one character of $B$ is therefore trivial on $U$ and has the form

$$
\boxed{
\chi_\theta
\begin{pmatrix}a&b\\0&a^{-1}\end{pmatrix}
=\theta(a)
},
$$

where $\theta:k^\times\to\mathbb C^\times$ is a multiplicative character.

The [Bruhat decomposition of SL2 over a finite field](../../../../../bruhat-decomposition-of-sl2-over-a-finite-field.md) has two double cosets,

$$
G=B\sqcup BwB,
\qquad
w=\begin{pmatrix}0&-1\\1&0\end{pmatrix},
$$

and $B\cap wBw^{-1}=T$. Conjugation by $w$ inverts $T$, so

$$
\chi_\theta^w|_T=\chi_{\theta^{-1}}|_T.
$$

The only nonidentity Mackey term vanishes exactly when these two one-dimensional characters differ. Consequently

$$
\boxed{
\operatorname{Ind}_B^G\chi_\theta
\text{ is irreducible}
\quad\Longleftrightarrow\quad
\theta\ne\theta^{-1}
\quad\Longleftrightarrow\quad
\theta^2\ne1
}.
$$

Thus the trivial character is excluded, as is the unique quadratic character when $q$ is odd. All other degree-one characters of $B$ induce irreducibly; the induced representations have degree $[G:B]=q+1$. This is the [irreducible principal series of finite SL2](../../../../../irreducible-principal-series-of-finite-sl2.md).

## ↑ Ancestors (10)

1. [19H](../19h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
