<h1 id="algebra/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First suppose $E=E^*$. For $u\in U=\operatorname{im}E$, choose $v$ with $Ev=u$. For $w\in W=\ker E$,

$$
\langle u,w\rangle=\langle Ev,w\rangle=\langle v,Ew\rangle=0.
$$

Thus $U\subseteq W^\perp$. The [direct sum of vector spaces](../../../../../direct-sum.md) gives $\dim U=\dim V-\dim W$, while the [orthogonal complement](../../../../../orthogonal-complement.md) has $\dim W^\perp=\dim V-\dim W$. Equal finite dimensions imply $U=W^\perp$.

Conversely, suppose $U=W^\perp$. Decompose arbitrary vectors as $v=u+w$ and $v'=u'+w'$, with $u,u'\in U$ and $w,w'\in W$. Since $E$ is the indicated [projection](../../../../../projection-linear-algebra.md), $Ev=u$ and $Ev'=u'$. Orthogonality makes the cross terms vanish, so

$$
\langle Ev,v'\rangle=\langle u,u'\rangle=\langle v,Ev'\rangle.
$$

Therefore $E$ satisfies the defining identity of its own [adjoint operator](../../../../../adjoint-operator.md). By uniqueness from part (a), $E=E^*$. Hence

$$
\boxed{E=E^*\quad\Longleftrightarrow\quad U=W^\perp.}
$$

This is the characterization of an [orthogonal projection](../../../../../orthogonal-projection.md) among projections along a complementary subspace.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [Algebra](../../../algebra.md)
4. [2013](../../../../2013-split.md)
5. [Past exam of the algebra and analysis I for mathematics and philosophy course of the University of Oxford](../../../../split.md)
6. [Algebra and analysis I for mathematics and philosophy course of the University of Oxford](../../../../../algebra-and-analysis-i-for-mathematics-and-philosophy-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and philosophy course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-philosophy-course-of-the-university-of-oxford.md)
8. [Mathematics and philosophy course of the University of Oxford](../../../../../mathematics-and-philosophy-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
