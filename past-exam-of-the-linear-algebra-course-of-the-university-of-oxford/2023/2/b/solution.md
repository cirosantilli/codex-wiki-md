<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [b](../b.md)

The increments $\Delta_i=d_i-d_{i-1}$ are positive integers by part (a)(i), are nonincreasing by part (a)(ii), and sum to $d_m=4$. Thus they form an [integer partition](../../../../integer-partition.md) of $4$. The complete list is $(4)$, $(3,1)$, $(2,2)$, $(2,1,1)$, and $(1,1,1,1)$.

To prove all five occur over every [field](../../../../field.md), let $J_s(0)$ be a [Nilpotent Jordan block](../../../../nilpotent-jordan-block.md) of size $s$. It sends each [standard basis](../../../../standard-basis.md) vector to its predecessor, with the first sent to zero, so

$$
\dim\ker J_s(0)^i=\min(i,s).
$$

For a [block diagonal matrix](../../../../block-diagonal-matrix.md), the [nullities](../../../../nullity-of-a-linear-map.md) add. The following explicit [nilpotent matrices](../../../../nilpotent-matrix.md) therefore realize every possible sequence:

$$
\boxed{\begin{array}{c|c|c}
m&(d_1,\ldots,d_m)&\text{realizing matrix}\\\hline
1&(4)&0_{4\times4}\\
2&(3,4)&J_2(0)\oplus J_1(0)\oplus J_1(0)\\
2&(2,4)&J_2(0)\oplus J_2(0)\\
3&(2,3,4)&J_3(0)\oplus J_1(0)\\
4&(1,2,3,4)&J_4(0)
\end{array}}.
$$

In each row the largest [Jordan block](../../../../jordan-block.md) size is exactly the [nilpotency index](../../../../nilpotency-index.md) $m$, so the displayed sequence stops at the correct place.

## ↑ Ancestors (12)

1. [b](../b.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the linear algebra course of the University of Oxford](../../../split.md)
5. [Linear algebra course of the University of Oxford](../../../../linear-algebra-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
