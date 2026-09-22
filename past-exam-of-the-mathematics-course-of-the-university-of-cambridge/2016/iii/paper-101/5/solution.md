<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The [Artin-Rees lemma](../../../../../artin-rees-lemma.md) states that, for a [Noetherian ring](../../../../../noetherian-ring.md) $R$, an [ideal](../../../../../ideal.md) $I$, a [finitely generated module](../../../../../finitely-generated-module.md) $M$, and a [submodule](../../../../../submodule.md) $N\subseteq M$, there is $c\ge0$ such that

$$
\boxed{I^jM\cap N=I^{j-c}(I^cM\cap N)\quad\text{for every }j\ge c.}
$$

Thus the filtration on $N$ induced from the [I-adic filtration](../../../../../i-adic-filtration.md) of $M$ is eventually determined by one of its terms.

For the proof, form the [Rees ring](../../../../../rees-algebra.md) and its [Rees module](../../../../../rees-module.md):

$$
\mathcal R(I)=\bigoplus_{j\ge0}I^jt^j\subseteq R[t],\qquad
\mathcal R_I(M)=\bigoplus_{j\ge0}I^jMt^j.
$$

Since $R$ is a [Noetherian ring](../../../../../noetherian-ring.md), write $I=(a_1,\ldots,a_s)$. Then $\mathcal R(I)=R[a_1t,\ldots,a_st]$, so it is a [Noetherian ring](../../../../../noetherian-ring.md) by the [Hilbert basis theorem](../../../../../hilbert-basis-theorem.md). Generators of $M$ in degree zero generate $\mathcal R_I(M)$ as a [module](../../../../../module-mathematics.md) over $\mathcal R(I)$, so this is a [Noetherian module](../../../../../noetherian-module.md).

The graded [submodule](../../../../../submodule.md)

$$
L=\bigoplus_{j\ge0}(I^jM\cap N)t^j
$$

is therefore finitely generated. Choose homogeneous generators $z_\alpha t^{d_\alpha}$ with $d_\alpha\le c$ for some $c$. For $j\ge c$, taking degree-$j$ components gives

$$
I^jM\cap N=\sum_\alpha I^{j-d_\alpha}z_\alpha
=I^{j-c}\sum_\alpha I^{c-d_\alpha}z_\alpha.
$$

The same generators show that the final sum is exactly $I^cM\cap N$. This proves the [Artin-Rees lemma](../../../../../artin-rees-lemma.md). If $L=0$, one may simply take $c=0$.

Now let

$$
K=\bigcap_{j\ge1}I^jM.
$$

It is a [submodule](../../../../../submodule.md) of the [Noetherian module](../../../../../noetherian-module.md) $M$, hence a [finitely generated module](../../../../../finitely-generated-module.md). Apply the [Artin-Rees lemma](../../../../../artin-rees-lemma.md) with $N=K$ and $j=c+1$. Since $K$ is contained in every $I^jM$ (including $I^0M=M$), its conclusion reduces to

$$
K=IK.
$$

Write generators as $y_1,\ldots,y_h$. There is a matrix $A=(a_{ij})$ with entries in $I$ such that $y_i=\sum_j a_{ij}y_j$. Multiplication by the adjugate of $I_h-A$ shows that

$$
\det(I_h-A)y_i=0\quad\text{for all }i.
$$

The [determinant](../../../../../determinant.md) is congruent to $1$ modulo $I$, so it is $1+r$ for some $r\in I$. This [determinant trick](../../../../../determinant-trick.md) produces a single such element annihilating all of $K$, and in particular annihilating each $m\in K$. If $K=0$, use $r=0$.

Conversely, if $(1+r)m=0$ with $r\in I$, then $m=-rm$. Iterating gives $m=(-r)^jm\in I^jM$ for every $j\ge1$. Hence the exact description is

$$
\boxed{\bigcap_{j\ge1}I^jM=\{m\in M:\text{some }r\in I\text{ satisfies }(1+r)m=0\}.}
$$

In a [local ring](../../../../../local-ring.md) with $I$ contained in the [maximal ideal](../../../../../maximal-ideal.md), every $1+r$ is a [unit](../../../../../unit-in-a-ring.md), so this also yields the usual vanishing form of the [Krull intersection theorem](../../../../../krull-intersection-theorem.md).

For a failure without the [Noetherian ring](../../../../../noetherian-ring.md) hypothesis, let $D=\mathbb Z[1/2]_{\ge0}$ and use the [semigroup algebra](../../../../../semigroup-algebra.md)

$$
R=k[t^q:q\in D]=\bigcup_{h\ge0}k[t^{1/2^h}].
$$

Its elements are finite sums of formal [monomials](../../../../../monomial.md) $t^q$, with multiplication $t^qt^{q'}=t^{q+q'}$. Each ring in the union is a [polynomial ring](../../../../../polynomial-ring.md) and the inclusions are injective, so $R$ is an [integral domain](../../../../../integral-domain.md). It is not a [Noetherian ring](../../../../../noetherian-ring.md), since

$$
(t)\subsetneq(t^{1/2})\subsetneq(t^{1/4})\subsetneq\cdots.
$$

Indeed the generator on the left is the square of the next generator, while division in the opposite direction would require a negative exponent, which is unavailable in $R$.

Let $I$ be the [ideal](../../../../../ideal.md) of elements with zero constant term, equivalently

$$
I=(t^q:q\in D,\ q>0).
$$

It is proper because taking the constant term gives $R/I\cong k$. Every generator $t^q$ is $(t^{q/2})^2$, with $t^{q/2}\in I$, so $I^2=I$. Thus this is a nonzero [idempotent ideal](../../../../../idempotent-ideal.md), with $I^j=I$ for every $j\ge1$. Take

$$
\boxed{m=t\in\bigcap_{j\ge1}I^j.}
$$

For every $r\in I$, the constant term of $1+r$ is $1$, so $1+r\ne0$. Since $R$ is an [integral domain](../../../../../integral-domain.md) and $t\ne0$, we have $(1+r)t\ne0$. This gives all three requested objects and proves that no element of the required form annihilates $m$.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 101](../../paper-101-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
