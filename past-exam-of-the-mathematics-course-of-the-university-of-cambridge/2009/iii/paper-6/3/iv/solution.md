<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Use the ordered alphabet

$$
\mathcal A=(1,2,\ldots,n,\bar n,\overline{n-1},\ldots,\bar1),
$$

with [weights](../../../../../../weight-representation-theory.md) $\operatorname{wt}(i)=\varepsilon_i$ and $\operatorname{wt}(\bar i)=-\varepsilon_i$. The [crystal of the defining symplectic representation](../../../../../../crystal-of-the-defining-symplectic-representation.md) is the chain

$$
1\xrightarrow{1}2\xrightarrow{2}\cdots\xrightarrow{n-1}n\xrightarrow{n}\bar n\xrightarrow{n-1}\cdots\xrightarrow{2}\bar2\xrightarrow{1}\bar1.
$$

The label of an arrow is its [simple root](../../../../../../simple-root.md) color; a [Kashiwara operator](../../../../../../kashiwara-operator.md) $\widetilde f_i$ follows an arrow of color $i$ and lowers the [weight](../../../../../../weight-representation-theory.md) by $\alpha_i$.

Here is a grid description of the entire [tensor product of crystals](../../../../../../tensor-product-of-crystals.md), valid for every $n$. Put one vertex $a\otimes b$ at row $a$ and column $b$, in the alphabet order above. Let $P_i$ be the set of chain positions with outgoing color $i$, and $Q_i$ the positions with incoming color $i$:

$$
P_i=\{i,2n-i\},\quad Q_i=\{i+1,2n-i+1\}\quad(i<n),\qquad P_n=\{n\},\quad Q_n=\{n+1\}.
$$

Their indicators are $\varphi_i$ and $\varepsilon_i$. Use the [crystal tensor-product rule](../../../../../../crystal-tensor-product-rule.md)

$$
\widetilde f_i(a\otimes b)=\begin{cases}
\widetilde f_i(a)\otimes b,&\varphi_i(a)>\varepsilon_i(b),\\
a\otimes\widetilde f_i(b),&\varphi_i(a)\le\varepsilon_i(b).
\end{cases}
$$

An arrow is omitted if the selected factor has no outgoing arrow of that color. Thus the complete grid has a downward color-$i$ arrow when $a\in P_i$ and $b\notin Q_i$, and a rightward color-$i$ arrow when $b\in P_i$ and $a\notin P_i$. There are no other arrows. These two coordinate rules specify every vertex and every edge of the requested general-rank drawing. The following figure displays the full grid at $n=3$, including all components, together with the standard chain; increasing $n$ uses exactly the same grid construction.

<a id="3/iv/image-defining-c3-crystal-and-its-complete-tensor-square-crystal-with-all-colored-arrows-and-the-three-highest-weight-components"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-6-crystals.png)

**[Figure 2](#3/iv/image-defining-c3-crystal-and-its-complete-tensor-square-crystal-with-all-colored-arrows-and-the-three-highest-weight-components). Defining C3 crystal and its complete tensor-square crystal with all colored arrows and the three highest-weight components**.

For completeness, highest vertices can be read from the raising rule, which selects the first factor when $\varphi_i(a)\ge\varepsilon_i(b)$. If $a$ has an incoming edge of color $i$, then $\varphi_i(a)=0$; either the raising operator acts nontrivially on $a$, or $\varepsilon_i(b)=1$ and it acts nontrivially on $b$. Thus a highest vertex must have $a=1$. At $a=1$, all $\varphi_i(a)$ vanish except $\varphi_1(a)=1$. To be highest, the incoming color of $b$, if any, must consequently be $1$. For $n\ge2$, the possibilities are exactly

$$
1\otimes1,\qquad 1\otimes2,\qquad 1\otimes\bar1.
$$

Their [weights](../../../../../../weight-representation-theory.md) are $2\varepsilon_1=2\omega_1$, $\varepsilon_1+\varepsilon_2=\omega_2$, and zero. Each occurs once. Connected highest-weight components of the [crystal basis](../../../../../../crystal-basis.md) describe the [irreducible representations](../../../../../../irreducible-representation.md) in the [tensor product of Lie algebra representations](../../../../../../tensor-product-of-lie-algebra-representations.md), so

$$
\boxed{V\otimes V\cong L(2\omega_1)\oplus L(\omega_2)\oplus L(0)\qquad(n\ge2).}
$$

This is the [tensor-square decomposition of the defining symplectic representation](../../../../../../tensor-square-decomposition-of-the-defining-symplectic-representation.md). The [symmetric square](../../../../../../symmetric-square.md) is $L(2\omega_1)$; the [exterior square](../../../../../../exterior-square.md) is the [direct sum](../../../../../../direct-sum.md) of its invariant inverse-form line and the [primitive exterior square](../../../../../../primitive-exterior-square.md) $L(\omega_2)$. Their [dimensions](../../../../../../dimension-vector-space.md) are respectively $n(2n+1)$, $n(2n-1)-1$, and one, summing to $4n^2=\dim(V\otimes V)$. At $n=1$, the chain has two vertices and the highest tensor vertices are only $1\otimes1$ and $1\otimes\bar1$: the decomposition is $L(2\omega_1)\oplus L(0)$, of [dimensions](../../../../../../dimension-vector-space.md) three and one.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
