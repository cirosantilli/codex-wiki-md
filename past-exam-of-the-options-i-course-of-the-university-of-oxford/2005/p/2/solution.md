<h1 id="p/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Suppose an approximation has an error expansion $A(h)=I+ch^p+O(h^q)$ with $q>p$. With refinement factor $r>1$, combining the two approximations eliminates the leading term:

$$
\boxed{R(h)=\frac{r^pA(h/r)-A(h)}{r^p-1}=I+O(h^q).}
$$

If further expansion terms are known, repeat the elimination at their successive powers. For an even-power trapezium expansion and repeated halving, this gives the Romberg recurrence $R_{k,j}=(4^jR_{k,j-1}-R_{k-1,j-1})/(4^j-1)$, starting from $R_{k,0}=T(2^{-k})$.

For the stated cubic the one-panel trapezium value is $T(1)=[0^3+1^3]/2=1/2$. The two-panel value is

$$
T(1/2)=\frac14\left[0+2\left(\frac12\right)^3+1\right]=\frac5{16}.
$$

The leading power is two, so one extrapolation step gives

$$
\boxed{\frac{4T(1/2)-T(1)}3=\frac{4(5/16)-1/2}3=\frac14.}
$$

This equals the exact integral $[x^4/4]_0^1=1/4$; for a cubic the trapezium error has only the leading $h^2$ term, which this combination removes exactly.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [P](../../p.md)
3. [2005](../../../2005-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
