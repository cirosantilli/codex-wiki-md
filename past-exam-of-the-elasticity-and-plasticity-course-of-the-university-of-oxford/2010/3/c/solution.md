<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the same [first variation](../../../../first-variation.md) on the half-plane, with no restrictions on the edge [traces](../../../../matrix-trace.md) of $\eta$. Write $M=w_{xx}+\nu w_{yy}$. Two $x$ integrations of the $M\eta_{xx}$ term produce the boundary term $-M\eta_x+M_x\eta$ at $x=0$. The mixed term, after one integration in $x$ and one along the edge in $y$, contributes $2(1-\nu)w_{xyy}\eta$. All other boundary terms vanish at infinity. Hence

$$
\delta\mathcal U=D\iint_{x>0}\eta\nabla^4w\,dx\,dy
-D\int_{-\infty}^{\infty}
\{\eta_x(w_{xx}+\nu w_{yy})-\eta[w_{xxx}+(2-\nu)w_{xyy}]\}_{x=0}\,dy.
$$

The bulk equation makes its area term zero. Stationarity therefore gives exactly

$$
\boxed{\int_{-\infty}^{\infty}
\{\eta_x(w_{xx}+\nu w_{yy})-\eta[w_{xxx}+(2-\nu)w_{xyy}]\}_{x=0}\,dy=0.}
$$

The two edge [traces](../../../../matrix-trace.md) can be prescribed independently: use $\eta(x,y)=\chi(x)[f(y)+xg(y)]$ with $\chi=1$ near zero and compactly supported smooth $f,g$. The fundamental lemma on the edge then gives

$$
\boxed{w_{xx}+\nu w_{yy}=0,\qquad
w_{xxx}+(2-\nu)w_{xyy}=0\quad(x=0).}
$$

They are zero [bending moment](../../../../bending-moment.md) and zero effective transverse shear at a free straight edge. The second includes the edge derivative of the twisting moment; omitting the mixed contribution would give the wrong coefficient.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../split.md)
5. [Elasticity and plasticity course of the University of Oxford](../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
