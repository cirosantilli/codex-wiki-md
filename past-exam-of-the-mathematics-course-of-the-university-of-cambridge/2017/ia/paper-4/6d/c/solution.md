<h1 id="6d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For each positive [integer](../../../../../../integer.md) $n$, the positive elements of $A_n$ form an infinite [set](../../../../../../set-split.md), and the preceding increasing enumeration gives a [bijection](../../../../../../bijection.md) $f_n:\mathbb N\to A_n$ on these positive elements. The positive [integers](../../../../../../integer.md) have a unique decomposition $10^{n-1}q$ with $10\nmid q$, so these [sets](../../../../../../set-split.md) are disjoint and exhaust the positive [integers](../../../../../../integer.md).

The printed [natural numbers](../../../../../../natural-number.md) include $0$. The trailing-zero count of the representation of $0$ is not needed: shift the positive partition down by one and put

$$
\boxed{g(i,j)=f_{i+1}(j)-1,\qquad i,j\in\mathbb N.}
$$

Uniqueness of the trailing-zero count proves the [injective function](../../../../../../injective-function.md) property, and the decomposition of $N+1$ proves the [surjective function](../../../../../../surjective-function.md) property. An explicit [decimal trailing-zero pairing function](../../../../../../decimal-trailing-zero-pairing-function.md), using the increasing enumeration from the previous part, is

$$
\boxed{g(i,j)=10^i\left(j+1+\left\lfloor\frac j9\right\rfloor\right)-1.}
$$

Indeed, the bracket enumerates $1,2,\ldots,9,11,12,\ldots$, exactly the positive [integers](../../../../../../integer.md) not divisible by $10$. This handles both the positive index $n$ and the element $0$ without silently changing the PDF's convention.

To enumerate the [rational numbers](../../../../../../rational-number.md), first enumerate the [integers](../../../../../../integer.md) by $e(0)=0$, $e(2r-1)=r$, $e(2r)=-r$ for $r\ge1$. The [function](../../../../../../function-split.md) $(i,j)\mapsto e(i)/(j+1)$ maps $\mathbb N^2$ onto $\mathbb Q$, and composing with $g^{-1}$ gives a [surjective function](../../../../../../surjective-function.md) from $\mathbb N$. Choosing the first index representing each [rational number](../../../../../../rational-number.md) gives an [injective function](../../../../../../injective-function.md) $\mathbb Q\to\mathbb N$. Thus **$\mathbb Q$ is countably infinite**; its infinitude follows because it contains all [integers](../../../../../../integer.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6D](../../6d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
