<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**There is a sign error in the printed assertion under the standard [sl2 triple](../../../../../sl2-triple.md) convention.** Work first with the operators exactly as printed. Since the $v_i$ form a [Hamel basis](../../../../../basis.md), their prescribed images extend to [linear maps](../../../../../linear-map.md) on $V$; each vector is a finite [linear combination](../../../../../linear-combination.md) of [basis vectors](../../../../../basis-vector.md).

For $i\geq1$, the [operator commutators](../../../../../operator-commutator.md) with $h$ are

$$
\begin{aligned}
[h,e]v_i&=\bigl(-2(i-1)(i-1)+2i(i-1)\bigr)v_{i-1}=2ev_i,\\
[h,f]v_i&=\bigl(-2(i+1)^2+2i(i+1)\bigr)v_{i+1}=-2fv_i.
\end{aligned}
$$

At $i=0$, the first identity holds because both sides vanish; the second holds because $hf(v_0)=-2v_1$ and $fh(v_0)=0$. On the other hand, for $i\geq1$,

$$
[e,f]v_i=i(i+1)v_i-i(i-1)v_i=2iv_i=-hv_i.
$$

At $i=0$, both $ef(v_0)=e(v_1)=0$ and $fe(v_0)=0$, so this identity also holds. Thus the actual relations are

$$
\boxed{[h,e]=2e,\qquad[h,f]=-2f,\qquad[e,f]=-h.}
$$

In particular, $[e,f]v_1=2v_1\ne-2v_1=hv_1$ in [characteristic zero](../../../../../characteristic-zero.md); the requested equality cannot hold as printed. Setting

$$
\boxed{E=-e,\qquad H=h,\qquad F=f.}
$$

corrects the sign and gives $[H,E]=2E$, $[H,F]=-2F$, $[E,F]=H$. These are the standard [sl2 triple](../../../../../sl2-triple.md) relations, so the standard [basis](../../../../../basis.md) of the [sl2 Lie algebra](../../../../../sl2-lie-algebra.md) acts on $V$ by $E,H,F$, giving a [Lie algebra representation](../../../../../lie-algebra-representation.md).

For completeness, these operators are [linearly independent](../../../../../linear-independence.md): applying $aE+bH+cF=0$ to $v_0$ gives $c=0$; applying it to $v_1$ then gives $b=0$; applying it to $v_2$ gives $a=0$. Hence the printed operators span a [Lie subalgebra](../../../../../lie-subalgebra.md) isomorphic to the [sl2 Lie algebra](../../../../../sl2-lie-algebra.md), even though their printed normalization fails. Replacing the coefficient $i-1$ in the printed definition of $e(v_i)$ by $1-i$ is one equivalent way to repair the statement.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the lie algebras course of Part C of the mathematics course of the University of Oxford](../../../../split.md)
6. [Lie algebras course of Part C of the mathematics course of the University of Oxford](../../../../../lie-algebras-course-of-part-c-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
