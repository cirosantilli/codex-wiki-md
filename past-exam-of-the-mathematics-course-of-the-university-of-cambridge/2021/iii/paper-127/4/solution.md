<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The space $K(\mathbb Z/n,1)$ is a classifying space $B(\mathbb Z/n)$. The periodic resolution of a finite cyclic group gives

$$
H^*(K(\mathbb Z/n,1);\mathbb Z)
\cong\mathbb Z[c]/(nc),
\qquad |c|=2.
$$

Thus positive odd cohomology vanishes and every positive even group is $\mathbb Z/n$.

Let $p$ be odd. If $p\nmid n$, transfer makes multiplication by $n$ both zero and invertible on positive-degree cohomology, so

$$
H^*(K(\mathbb Z/n,1);\mathbb F_p)=\mathbb F_p.
$$

If $p\mid n$, restriction to the cyclic Sylow $p$-subgroup and transfer give

$$
H^*(K(\mathbb Z/n,1);\mathbb F_p)
\cong\Lambda(u)\otimes\mathbb F_p[v],
\qquad |u|=1,\quad |v|=2.
$$

For $n=p$, one may take $v=\beta u$, where $\beta$ is the mod-$p$ [Bockstein homomorphism](../../../../../bockstein-homomorphism.md).

For the second part put $A=\mathbb Z/p$ and $X=K(A,1)\times K(A,1)$. The long exact homotopy sequence of the homotopy fibre of $f:X\to K(A,2)$ gives

$$
1\longrightarrow A\longrightarrow G:=\pi_1(F)
\longrightarrow A^2\longrightarrow1
$$

and $\pi_k(F)=0$ for $k>1$. Therefore $F$ is a $K(G,1)$ and $|G|=p^3$.

Regard it as the fibration

$$
K(A,1)\longrightarrow F\longrightarrow K(A,1)^2.
$$

Write

$$
H^*(K(A,1)^2;\mathbb F_p)
=\Lambda(u_1,u_2)\otimes\mathbb F_p[v_1,v_2]
$$

and write $w,t$ for the degree-one and degree-two generators of the fibre. The fibration is classified by $u_1u_2$, so in its cohomological [Serre spectral sequence](../../../../../serre-spectral-sequence.md)

$$
d_2(w)=u_1u_2.
$$

The [Kudo transgression theorem](../../../../../kudo-transgression-theorem.md) and the mod-$p$ Bockstein give

$$
d_3(t)=\beta(u_1u_2)=v_1u_2-u_1v_2\ne0.
$$

Consequently $H^1(F;\mathbb F_p)$ has basis $u_1,u_2$, while $H^2(F;\mathbb F_p)$ has the four surviving classes represented by

$$
v_1,\quad v_2,\quad u_1w,\quad u_2w.
$$

If $G$ were abelian, an abelian group of order $p^3$ mapping onto $A^2$ would be either $A^3$ or $\mathbb Z/p^2\times A$. The first has three-dimensional $H^1(-;\mathbb F_p)$; the second has two-dimensional $H^1$ but three-dimensional $H^2$. Both contradict the dimensions just calculated. Hence $G$ is nonabelian.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 127](../../paper-127-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
