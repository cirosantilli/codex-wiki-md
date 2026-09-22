<h1 id="18j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $K=\mathbb R$, the answer is yes. A root of $\Phi_4(X)=X^2+1$ is $i$ or $-i$, so

$$
\mathbb R(\zeta_4)=\mathbb C=\overline{\mathbb R}.
$$

For $K=\mathbb Q$, the answer is no. Every $\mathbb Q(\zeta_n)/\mathbb Q$ is finite abelian Galois. If $\sqrt[3]{2}$ belonged to $\mathbb Q^{\mathrm{cyc}}$, then it would belong to some $\mathbb Q(\zeta_n)$. The [subextensions of an abelian Galois extension](../../../../../../subextensions-of-an-abelian-galois-extension.md) result would make

$$
\mathbb Q(\sqrt[3]{2})/\mathbb Q
$$

Galois. This is false: $X^3-2$ has two nonreal roots absent from the real field $\mathbb Q(\sqrt[3]{2})$. Hence $\mathbb Q^{\mathrm{cyc}}$ is a proper subfield of $\overline{\mathbb Q}$.

For $K=\mathbb F_p$, the answer is yes. Given $m\geq1$, take

$$
n=p^m-1,
$$

which is coprime to $p$. Every root of $\Phi_n$ in characteristic $p$ has exact multiplicative order $n$. The degree

$$
[\mathbb F_p(\zeta_n):\mathbb F_p]
$$

is the least positive $d$ such that $n\mid p^d-1$. The value $d=m$ works, and no $d<m$ can work because

$$
0<p^d-1<p^m-1=n.
$$

Therefore

$$
\mathbb F_p(\zeta_{p^m-1})=\mathbb F_{p^m}.
$$

Every element algebraic over $\mathbb F_p$ lies in some finite field $\mathbb F_{p^m}$, so

$$
\mathbb F_p^{\mathrm{cyc}}=\overline{\mathbb F}_p.
$$

These are respectively the [maximal cyclotomic extension of the real numbers](../../../../../../maximal-cyclotomic-extension-of-the-real-numbers.md), the [maximal cyclotomic extension of the rational numbers](../../../../../../maximal-cyclotomic-extension-of-the-rational-numbers.md), and the [maximal cyclotomic extension of a finite field](../../../../../../maximal-cyclotomic-extension-of-a-finite-field.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [18J](../../18j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
