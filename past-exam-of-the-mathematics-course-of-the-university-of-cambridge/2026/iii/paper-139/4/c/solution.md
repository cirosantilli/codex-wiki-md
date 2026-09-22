<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $D=\partial_t$. Since

$$
[tD+\lambda,D]=-D,
$$

the assignments $\theta_\lambda(y)=tD+\lambda$ and $\theta_\lambda(x)=D$ respect $[y,x]=-x$ and extend through the [universal enveloping algebra](../../../../../../universal-enveloping-algebra.md).

The operator $y$ has distinct eigenvectors $t^n$ with eigenvalues $\lambda+n$, while $x(t^n)=nt^{n-1}$. Therefore the submodules are exactly

$$
0,\quad k\oplus kt\oplus\cdots\oplus kt^m\ (m\geq0),\quad k[t].
$$

The character $x\mapsto0$, $y\mapsto\lambda$ has kernel $I_\lambda$, so $U(\mathfrak g)/I_\lambda\cong k$ and $I_\lambda$ is maximal.

By part (a), the $S$-torsion in every module is a submodule. On $V=k\oplus kt$, $x(t)=1$ and $y$ has eigenvalues $\lambda,\lambda+1$. If some $s\in S$ vanished on the $(\lambda+1)$-character, then $s(t)\in k$. Since $s(1)$ is the nonzero scalar given by its image modulo $I_\lambda$, subtracting a suitable constant from $t$ would produce an $S$-torsion vector $v$ with $xv=1$. Submodule closure would make $1$ torsion, contradicting $S\subseteq\mathcal C(I_\lambda)$. Thus

$$
S\subseteq\mathcal C(I_\lambda)\cap\mathcal C(I_{\lambda+1}).
$$

Apply the same argument to each adjacent two-dimensional quotient

$$
(k\oplus\cdots\oplus kt^{n+1})/(k\oplus\cdots\oplus kt^{n-1})
$$

where $x(t^{n+1})=(n+1)t^n\ne0$ because $\operatorname{char}k=0$. Induction gives

$$
\boxed{S\subseteq\bigcap_{n\in\mathbb N_0}\mathcal C(I_{\lambda+n}).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 139](../../../paper-139-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
