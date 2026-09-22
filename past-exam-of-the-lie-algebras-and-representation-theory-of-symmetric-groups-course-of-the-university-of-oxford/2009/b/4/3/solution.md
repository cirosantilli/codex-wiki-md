<h1 id="b/4/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The final condition makes $\lambda=(k,k-1,\ldots,1)$. Its column lengths are the same staircase, so

$$
h(i,j)=2k-2i-2j+3,
$$

which is odd. This proves (3) implies (1) and completes the equivalence. Such a partition exists exactly at the triangular numbers

$$
\boxed{n=k(k+1)/2\quad(k\geq1),\qquad\lambda=(k,k-1,\ldots,1).}
$$

The hook formula gives $v_2(f^\lambda)=v_2(n!)=a$, since its denominator is odd. Thus $2^a$ divides $f^\lambda$. Conversely $2^a\mid f^\gamma$ implies $v_2(\prod h_\gamma)=a-v_2(f^\gamma)\leq0$. The product is an integer, so its valuation is zero and all its hooks are odd. By the equivalence $\gamma$ is a staircase; its size uniquely determines its length, so **$\gamma=\lambda$**.

For the [character](../../../../../character-of-a-representation.md) assertion, every removable [rim hook](../../../../../rim-hook.md) has length equal to some [hook length](../../../../../hook-length.md) of the diagram. Here is a direct justification. If a [border strip](../../../../../rim-hook.md) $\lambda/\mu$ occupies rows $i$ through $j$, connectedness and absence of a two-by-two block make adjacent strips of boxes overlap in exactly one column. Hence $\mu_l=\lambda_{l+1}-1$ for $i\leq l<j$, so its size is $\lambda_i-\mu_j+j-i$. The column $c=\mu_j+1$ has height $j$, giving exactly $h_\lambda(i,c)=\lambda_i-\mu_j+j-i$. Therefore every removable [rim hook](../../../../../rim-hook.md) of the staircase has odd length.

A fixed-point-free permutation of power-of-two order has only even cycles. Apply the [Murnaghan–Nakayama rule](../../../../../murnaghan-nakayama-rule.md) starting with any cycle. It would require removal of a [rim hook](../../../../../rim-hook.md) of that even length, but none exists. The sum is empty, so

$$
\boxed{\chi^\lambda(g)=0.}
$$

Finally suppose $\gamma$ has distinct parts and is not $\lambda$. It cannot be another staircase of the same size. Thus some gap between successive rows is at least two, or the last row has length at least two; in either case a horizontal rim domino is removable. No vertical rim domino is removable, since that would require two equal adjacent row lengths. Murnaghan-Nakayama on a [transposition](../../../../../transposition-permutation.md) consequently gives a nonempty sum

$$
\chi^\gamma(\tau)=\sum_{\text{removable horizontal dominoes}}f^{\gamma\setminus\text{domino}}>0,
$$

all signs being positive and all tableau counts positive. Thus **the [character](../../../../../character-of-a-representation.md) is nonzero at every [transposition](../../../../../transposition-permutation.md)**, proving the requested existence.

## ↑ Ancestors (13)

1. [3](../3.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../split.md)
6. [Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../../lie-algebras-and-representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
