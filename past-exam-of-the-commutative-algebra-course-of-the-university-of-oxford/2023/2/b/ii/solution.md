<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Consider the [kernel of a ring homomorphism](../../../../../kernel-of-a-ring-homomorphism.md)

$$
K=\ker(R\longrightarrow R_{\mathfrak p})
=\{a\in R:sa=0\text{ for some }s\notin\mathfrak p\}.
$$

Since $R$ is a [Noetherian ring](../../../../../noetherian-ring.md), this [ideal](../../../../../ideal.md) has a finite [generating set of an ideal](../../../../../generating-set-of-an-ideal.md), say $K=(a_1,\ldots,a_t)$. For each $i$, choose $s_i\notin\mathfrak p$ with $s_i a_i=0$, and put

$$
f=\prod_{i=1}^t s_i.
$$

Then $f\notin\mathfrak p$ by the [prime ideal](../../../../../prime-ideal.md) condition, and $fK=0$. If $K=0$, take the empty product $f=1$.

If $a/f^n$ maps to zero under the [ring homomorphism](../../../../../ring-homomorphism.md) $\theta_f$ from [a](../../a.md), then $a/1=0$ in $R_{\mathfrak p}$ because $f/1$ is a [unit](../../../../../unit-in-a-ring.md) there. Hence $a\in K$, so $fa=0$. The [vanishing criterion in a module localization](../../../../../vanishing-criterion-in-a-module-localization.md) now gives $a/f^n=0$ already in $R_f$. Therefore

$$
\boxed{\ker\theta_f=0,\qquad\theta_f:R_f\hookrightarrow R_{\mathfrak p}.}
$$

This is the [finite generation clears localization kernels](../../../../../finite-generation-clears-localization-kernels.md) argument: the finite [generating set of an ideal](../../../../../generating-set-of-an-ideal.md) permits a single element outside $\mathfrak p$ to annihilate the entire [kernel of a ring homomorphism](../../../../../kernel-of-a-ring-homomorphism.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the commutative algebra course of the University of Oxford](../../../../split.md)
6. [Commutative algebra course of the University of Oxford](../../../../../commutative-algebra-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
