<h1 id="3/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Apply the product from right to left, choosing every [Givens rotation](../../../../../givens-rotation.md) from the current first column. First $J(1,2)$ replaces $(a_1,a_2)$ by $(\sqrt{a_1^2+a_2^2},0)$. Next $J(1,3)$ combines that retained entry with $a_3$ and sets the third entry to zero. Inductively, after eliminating coordinates $2,\ldots,k$, the first coordinate is

$$
\sqrt{a_1^2+\cdots+a_k^2},
$$

and coordinates $2,\ldots,k$ are zero. Later [Givens rotations](../../../../../givens-rotation.md) involve only coordinate one and a new coordinate, so those zeros remain zero. Therefore

$$
\boxed{Q_1a=(\|a\|_2,0,\ldots,0)^T=\|a\|_2e_1,}
$$

where $e_1$ is the first [standard basis](../../../../../standard-basis.md) [vector](../../../../../vector.md). The zero [vector](../../../../../vector.md) is included by choosing the [identity matrix](../../../../../identity-matrix.md) for every zero pair. The nonnegative sign follows from the convention fixed in part (c)(ii). This is the first-column stage of [QR decomposition by Givens rotations](../../../../../qr-decomposition-by-givens-rotations.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the numerical analysis course of the University of Oxford](../../../../split.md)
6. [Numerical analysis course of the University of Oxford](../../../../../numerical-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
