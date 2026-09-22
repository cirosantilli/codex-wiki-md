<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Conversely, the same induction-norm formula shows that $I_G(\varphi)=N$ for every nonprincipal $\varphi\in\operatorname{Irr}(N)$. Conjugation by each $g\notin N$ fixes only $1_N$, so [Brauer's permutation lemma](../../../../../../../brauer-s-permutation-lemma.md) says that it fixes only the identity [conjugacy class](../../../../../../../conjugacy-class.md) of $N$. A nonidentity element centralizing $g$ would provide another fixed class. Therefore $C_N(g)=1$ for every $g\notin N$.

We first prove that $|N|$ and $[G:N]$ are coprime. If a prime $p$ divided both, a [Sylow p-subgroup](../../../../../../../sylow-subgroup.md) $S$ of $G$ would have $1<S\cap N<S$. The nontrivial [normal subgroup](../../../../../../../normal-subgroup.md) $S\cap N$ meets $Z(S)$ nontrivially: the class equation for the conjugation action of the [p-group](../../../../../../../p-group.md) $S$ on $S\cap N$ makes the number of fixed elements divisible by $p$, and one of them is the identity. Choose $1\ne z\in N\cap Z(S)$ and $s\in S\setminus N$. Then $z\in C_N(s)$, contradicting the previous conclusion.

Thus $N$ is a [normal subgroup](../../../../../../../normal-subgroup.md) that is also a [Hall subgroup](../../../../../../../hall-subgroup.md). The [Schur-Zassenhaus theorem](../../../../../../../schur-zassenhaus-theorem.md) supplies a [group complement](../../../../../../../complement-of-a-normal-subgroup.md) $H$, meaning $G=NH$ and $N\cap H=1$. The theorem's existence assertion requires only normality and coprimality of order and index. Here $H$ is nontrivial and proper by the assumptions on $N$.

For $n\in N\setminus\{1\}$, suppose $1\ne h\in H\cap nHn^{-1}$. Write $h=nh'n^{-1}$ with $h'\in H$. Projection to $G/N$ gives $hN=h'N$, hence $h=h'$ because $H\to G/N$ is injective. This makes $n$ centralize $h\notin N$, which is impossible. Hence $H\cap nHn^{-1}=1$. Writing an arbitrary element outside $H$ as $nh_0$ reduces its conjugate intersection to this case. It follows that $H$ is a [Frobenius complement](../../../../../../../frobenius-complement.md) and $G$ is a [Frobenius group](../../../../../../../frobenius-group.md).

Moreover, for each $1\ne h\in H$, the map $v\mapsto vhv^{-1}$ from $N$ into the coset $Nh$ is injective, since $C_N(h)=1$, and hence bijective. Thus every element outside $N$ belongs to a conjugate of $H$, while no nonidentity element of $N$ does. **The [Frobenius kernel](../../../../../../../frobenius-kernel.md) is exactly $N$.** This completes both directions of the [Frobenius kernel criterion by irreducible induction](../../../../../../../frobenius-kernel-criterion-by-irreducible-induction.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Iii](../../../../split.md)
6. [2002](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
