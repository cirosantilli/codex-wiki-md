<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $A(y)=y^{-1/2}+\lambda$ and $F(y,y')=A(y)\sqrt{1+y'^2}$. Since there is no explicit $x$ dependence, the [Beltrami identity](../../../../beltrami-identity.md) says $F-y'F_{y'}$ is constant along a stationary curve. One can verify it directly:

$$
\frac d{dx}(F-y'F_{y'})=y'\left(F_y-\frac d{dx}F_{y'}\right)=0
$$

by the [Euler-Lagrange equation](../../../../euler-lagrange-equation.md). Here $F_{y'}=A(y)y'/\sqrt{1+y'^2}$, so

$$
\boxed{H=F-y'F_{y'}=\frac{y^{-1/2}+\lambda}{\sqrt{1+y'^2}}\quad\text{is constant}.}
$$

This identity applies on the open arch where $y>0$. The constant is finite by evaluating at any interior point. Near an endpoint $A(y)>0$, hence $H>0$ everywhere on such an arch. Thus also $A(y)>0$ throughout it.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the short options course of the University of Oxford](../../../split.md)
5. [Short options course of the University of Oxford](../../../../short-options-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
