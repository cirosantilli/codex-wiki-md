<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $[a,b]=[1,2]$, $z(0)=-3$ and $\cosh\theta=3$ gives $e^\theta=3+2\sqrt2$. The normalization factors cancel, so

$$
\boxed{\|x-y^{(k)}\|_2\leq\frac{2}{(3+2\sqrt2)^k+(3-2\sqrt2)^k}\|x-x^{(0)}\|_2
\leq2(3-2\sqrt2)^k\|x-x^{(0)}\|_2.}
$$

If the [eigenvalues](../../../../eigenvalue.md) are known to be exactly $1,3/2,2$, use the more targeted [annihilating polynomial](../../../../annihilating-polynomial.md)

$$
\boxed{p_3(r)=(1-r)(1-2r/3)(1-r/2).}
$$

It equals one at zero and vanishes on the entire spectrum, so the [spectral theorem](../../../../spectral-theorem.md) gives $p_3(A)=0$. Thus $y^{(3)}=x$ in exact arithmetic. Degree three is the least degree that can vanish at all three distinct [eigenvalues](../../../../eigenvalue.md); a particular initial error supported on fewer eigenspaces can terminate earlier.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the numerical linear algebra and approximation course of the University of Oxford](../../../split.md)
5. [Numerical linear algebra and approximation course of the University of Oxford](../../../../numerical-linear-algebra-and-approximation-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
