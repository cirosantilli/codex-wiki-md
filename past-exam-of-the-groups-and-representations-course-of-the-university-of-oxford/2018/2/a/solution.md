<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $s=g_1$ and $r=g_2$. Direct [matrix multiplication](../../../../matrix-multiplication.md) gives

$$
r^4=s^2=I_3,\qquad srs=r^{-1}.
$$

Every product reduces to $r^ks^\ell$, with $0\leq k<4$ and $0\leq\ell<2$. These eight [matrices](../../../../matrix.md) are distinct and are precisely the listed elements:

$$
g_3=r^2,\quad g_4=sr=r^{-1}s,\quad g_5=rs,\quad
 g_6=srs=r^{-1},\quad g_7=r^2s.
$$

This is the [dihedral group](../../../../dihedral-group.md) of [group order](../../../../order-of-a-finite-group.md) eight. Its element $r^2$ commutes with both generators. Conjugation by $s$ interchanges $r$ and $r^{-1}$, while conjugation by $r$ sends $s$ to $r^2s$. It also interchanges $rs$ and $r^{-1}s$. The resulting [conjugacy classes](../../../../conjugacy-class.md) are

$$
\boxed{\{e\},\quad\{r^2\},\quad\{s,r^2s\},\quad
\{r,r^{-1}\},\quad\{sr,rs\}.}
$$

These are the stated $C_0,\ldots,C_4$ in order. To see that the last two reflection classes do not merge, conjugation changes the exponent in $r^ks$ by an even integer or changes its sign, preserving its parity. The five sets exhaust all eight elements.

Both generators are real [orthogonal matrices](../../../../orthogonal-matrix.md) with [determinant](../../../../determinant.md) $+1$. Hence every element obeys $g^\dagger g=I_3$ and $\det g=1$. The normal-form calculation establishes closure and inverses, so

$$
\boxed{G\leq SO(3)\leq SU(3).}
$$

In particular the embedding in the [special unitary group](../../../../special-unitary-group.md) uses the given real [matrices](../../../../matrix.md) viewed as complex ones.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
