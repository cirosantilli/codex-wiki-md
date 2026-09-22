<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The overlap of the two charts is obtained by inverting $c=t^3$. Since $c^2=b^3$, this also inverts $b=t^2$; then $t=c/b$ and $t^{-1}=b/c$. Thus its coordinate [ring](../../../../../../ring.md) is $R[t,t^{-1}]$. The other chart has coordinate $s=t^{-1}$. A [global section](../../../../../../global-section.md) is therefore an element in the intersection

$$
\Gamma(X,\mathcal O_X)=R[\pi t,t^2,t^3]\cap R[t^{-1}]=R
$$

inside $R[t,t^{-1}]$: a [Laurent polynomial](../../../../../../laurent-polynomial.md) with both only nonnegative and only nonpositive exponents is constant.

Let $k=R/(\pi)$. Reducing the presentation of $B$ gives

$$
B_s=k[a,b,c]/(a^2,ab,ac,c^2-b^3).
$$

As a [vector space](../../../../../../vector-space-split.md) and as a [ring](../../../../../../ring.md) extension, this is

$$
B_s=k[b,c]/(c^2-b^3)\oplus ka,
$$

where $a^2=0$ and $a$ is annihilated by $b,c$. In particular $a\ne0$: the free [basis](../../../../../../basis.md) of $B$ in part ii remains a [basis](../../../../../../basis.md) after tensoring with $k$. Although $a$ mapped to $\pi t$ before reduction, reducing the subring is not the same operation as taking its image inside $k[t]$; that distinction is exactly where the extra section arises.

On the overlap, $c$ is invertible and $ac=0$, so $a$ restricts to zero. Therefore the section $a$ on the first chart glues to zero on the second chart and defines a nonzero global nilpotent section $\eta$ on $X_s$. More precisely the reduced first-chart [ring](../../../../../../ring.md) is $k[t^2,t^3]$, and

$$
k[t^2,t^3]\cap k[t^{-1}]=k
$$

in $k[t,t^{-1}]$. The only extra compatible sections are multiples of $a$. Hence

$$
\boxed{\Gamma(X_s,\mathcal O_{X_s})\cong k[\eta]/(\eta^2),\qquad \Gamma(X,\mathcal O_X)=R.}
$$

The map printed in the question reduces $R$ modulo $\pi$ and includes its image as constants. Its kernel is $\pi R$ and its cokernel is $k\eta$. More strongly, even the usual base-change map after tensoring,

$$
\boxed{\Gamma(X,\mathcal O_X)\otimes_Rk=k\longrightarrow k[\eta]/(\eta^2),}
$$

is not surjective. This is [global-section base-change failure in a flat projective family](../../../../../../global-section-base-change-failure-in-a-flat-projective-family.md), despite the properness and flatness proved above.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 89](../../../paper-89-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
