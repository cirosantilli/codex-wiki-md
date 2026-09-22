<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Work inside $V_{m+1}$, and take the [orthogonal complement for a bilinear form](../../../../../orthogonal-complement-for-a-bilinear-form.md) of $U=V_m$ relative to this ambient space. If $z\in U\cap U^\perp$, then $\varphi(z,z)=0$, so positive definiteness on $U$ forces $z=0$.

Part (a)(iv) therefore gives $V_{m+1}=U\oplus U^\perp$, with $\dim U^\perp=1$. Choose $w\ne0$ spanning that complement and use the basis $e_1,\ldots,e_m,w$. Symmetry and orthogonality make its [Gram matrix](../../../../../gram-matrix.md)

$$
B=\begin{pmatrix}A_m&0\\0&d\end{pmatrix},\qquad d=\varphi(w,w).
$$

By part (b)(i), $\det B=(\det P)^2\det A_{m+1}>0$. Part (ii) applied to the already positive definite restriction gives $\det A_m>0$. Therefore

$$
d\det A_m=\det B>0,\qquad d>0.
$$

For a nonzero vector $u+tw$ with $u\in U$,

$$
\varphi(u+tw,u+tw)=\varphi(u,u)+t^2d>0.
$$

This proves **positive definiteness on $V_{m+1}$**.

Finally $\det A_1>0$ says $\varphi(e_1,e_1)>0$, so the restriction to $V_1$ is positive definite. Induction using all successive positive leading [principal minors](../../../../../principal-minor.md) reaches $V_n=V$. Combined with part (ii), this proves **[Sylvester's criterion](../../../../../sylvester-s-criterion.md)** in both directions.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the algebra 1 and differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Algebra 1 and differential equations 1 course of the University of Oxford](../../../../../algebra-1-and-differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
