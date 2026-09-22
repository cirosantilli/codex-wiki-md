<h1 id="a/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

We prove the common-zero-vector form of [Engel's theorem](../../../../../engel-s-theorem.md) by strong [induction](../../../../../mathematical-induction.md) on the dimension of the acting [Lie algebra](../../../../../lie-algebra-split.md) of operators, allowing its action on a nonzero finite-dimensional space to have a kernel. The zero-dimensional case is immediate.

First, every proper [Lie subalgebra](../../../../../lie-subalgebra.md) $H<L$ has a strictly larger [normalizer of a Lie subalgebra](../../../../../normalizer-of-a-lie-subalgebra.md). The action of $H$ on $L/H$ by $h\cdot(x+H)=[h,x]+H$ consists of nilpotent operators by part (a). Its image has dimension at most $\dim H<\dim L$. By [induction](../../../../../mathematical-induction.md) it has a nonzero common-zero [vector](../../../../../vector.md) $x+H$, giving $[H,x]\subseteq H$ with $x\notin H$. Hence $N_L(H)>H$.

Choose a maximal proper [Lie subalgebra](../../../../../lie-subalgebra.md) $H$. The preceding paragraph forces $N_L(H)=L$, so $H$ is an [ideal of a Lie algebra](../../../../../ideal-of-a-lie-algebra.md). Moreover $L/H$ has dimension one: otherwise any nonzero one-dimensional subspace of $L/H$, which is a [Lie subalgebra](../../../../../lie-subalgebra.md), would lift to an intermediate proper subalgebra. By [induction](../../../../../mathematical-induction.md) the common kernel

$$
W=\{v\in V:Hv=0\}
$$

is nonzero. It is $L$-invariant, since $h(xv)=x(hv)+[h,x]v=0$ for $v\in W$, $h\in H$, $x\in L$. Take $x\notin H$. Its restriction to $W$ is nilpotent and so has a nonzero [vector](../../../../../vector.md) $v$ in its kernel. As $L=H+Kx$, this [vector](../../../../../vector.md) is killed by every element of $L$:

$$
\boxed{Lv=0\quad\text{for some }v\ne0.}
$$

This completes the [induction](../../../../../mathematical-induction.md). The underlying space is understood to be nonzero, as required for the asserted [vector](../../../../../vector.md) to exist.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../split.md)
6. [Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../../lie-algebras-and-representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
