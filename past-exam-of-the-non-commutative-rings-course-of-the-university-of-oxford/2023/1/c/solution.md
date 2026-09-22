<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $B=R/I$. By the definition of a [left-primitive ideal](../../../../primitive-ideal.md), there is a [faithful module](../../../../faithful-module.md) $V$ that is a [simple module](../../../../irreducible-module.md) on the left over $B$. The assumed relation passes to the [quotient ring](../../../../quotient-ring.md) $B$, since any pair of elements of $B$ can be lifted to $R$.

By [Schur's lemma](../../../../schur-s-lemma.md), the [endomorphism ring](../../../../endomorphism-ring.md) $\operatorname{End}_B(V)$ is a [division ring](../../../../division-ring.md): the [kernel](../../../../kernel-of-a-linear-map-split.md) and [image](../../../../image-of-a-function.md) of a nonzero [module endomorphism](../../../../module-endomorphism.md) are [submodules](../../../../submodule.md), so simplicity makes that [module endomorphism](../../../../module-endomorphism.md) both [injective](../../../../injective-function.md) and [surjective](../../../../surjective-function.md). Set

$$
\Delta=\operatorname{End}_B(V)^{\mathrm{op}}.
$$

Evaluation makes $V$ a right [vector space over a division ring](../../../../vector-space-over-a-division-ring.md) $\Delta$, and the $B$-action is $\Delta$-linear. The [opposite ring](../../../../opposite-ring.md) in the definition ensures the correct order for this right action.

The [Jacobson density theorem](../../../../jacobson-density-theorem.md) says that, for any finite $\Delta$-[linearly independent](../../../../linear-independence.md) family $v_1,\ldots,v_m$ and any $w_1,\ldots,w_m\in V$, some $b\in B$ satisfies $bv_i=w_i$ for every $i$.

Suppose that $V$ contains two $\Delta$-[linearly independent](../../../../linear-independence.md) vectors $v,w$. Applying the [Jacobson density theorem](../../../../jacobson-density-theorem.md) twice, choose $a,b\in B$ satisfying

$$
av=0,\qquad aw=v,\qquad bv=w,\qquad bw=0.
$$

The inherited relation gives

$$
ba=\sum_{k=1}^n c_ka^kb
$$

with integers $c_k$. Acting on $w$, the left side gives $baw=bv=w$, but every term on the right gives $a^kbw=0$. This contradicts $w\ne0$. Thus $\dim_\Delta V=1$.

The [ring homomorphism](../../../../ring-homomorphism.md)

$$
B\longrightarrow\operatorname{End}_\Delta(V)
$$

given by the action is [injective](../../../../injective-function.md) because $V$ is a [faithful module](../../../../faithful-module.md). It is [surjective](../../../../surjective-function.md) because the [Jacobson density theorem](../../../../jacobson-density-theorem.md), applied to a single nonzero [basis vector](../../../../basis-vector.md), realizes every $\Delta$-linear [endomorphism](../../../../endomorphism.md) of this one-dimensional [vector space over a division ring](../../../../vector-space-over-a-division-ring.md). Every nonzero such [endomorphism](../../../../endomorphism.md) is invertible. Hence

$$
\boxed{R/I\cong\operatorname{End}_\Delta(V)\text{ is a division ring}.}
$$

The use of the [Jacobson density theorem](../../../../jacobson-density-theorem.md) here only prescribes actions on finitely many vectors; it does not assume that an arbitrary [primitive ring](../../../../primitive-ring.md) is already a full [endomorphism ring](../../../../endomorphism-ring.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the non-commutative rings course of the University of Oxford](../../../split.md)
5. [Non-commutative rings course of the University of Oxford](../../../../non-commutative-rings-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
