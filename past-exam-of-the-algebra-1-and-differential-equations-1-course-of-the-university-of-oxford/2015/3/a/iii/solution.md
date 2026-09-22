<h1 id="3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Writing $u=\sum_i u_ie_i$ and $v=\sum_i v_ie_i$, evaluation against the [dual basis](../../../../../dual-basis.md) gives

$$
\boxed{\phi(u,v)=\sum_i u_i\overline{v_i}.}
$$

**This has codomain $\mathbb C$, not the printed $\mathbb R$.** For a nonzero [vector space](../../../../../vector-space-split.md), take $u=ie_1$ and $v=e_1$ to obtain $\phi(u,v)=i$. Only the diagonal values $\phi(v,v)$ must be real. The displayed formula defines the intended [complex inner product](../../../../../hermitian-inner-product.md).

It is linear in the first argument and conjugate-linear in the second:

$$
\phi(au+bw,v)=a\phi(u,v)+b\phi(w,v),\qquad
\phi(u,av+bw)=\overline a\phi(u,v)+\overline b\phi(u,w).
$$

It has [conjugate symmetry](../../../../../conjugate-symmetry.md), since $\phi(v,u)=\overline{\phi(u,v)}$. Finally,

$$
\phi(v,v)=\sum_i|v_i|^2\geq0,
$$

with equality exactly when every coordinate vanishes, equivalently $v=0$. This proves [positive definiteness](../../../../../positive-definiteness.md). Since $\phi(e_i,e_j)=\delta_{ij}$, the original [basis](../../../../../basis.md) is [orthonormal](../../../../../orthonormal-set.md). This is the [inner product determined by a basis](../../../../../inner-product-determined-by-a-basis.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the algebra 1 and differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Algebra 1 and differential equations 1 course of the University of Oxford](../../../../../algebra-1-and-differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
