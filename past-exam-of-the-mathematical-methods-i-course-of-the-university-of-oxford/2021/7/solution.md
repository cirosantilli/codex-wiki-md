<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

The two affine lines meet at $(a,b)=(2,1)$. Translating their intersection to the origin, $X=x-2$, $Y=y-1$, removes both constant terms and gives the [homogeneous first-order differential equation](../../../homogeneous-first-order-differential-equation.md)

$$
\frac{dY}{dX}=\frac{4X+2Y}{2X-Y}.
$$

On a patch with $X\ne0$, put $Y=uX$. Then $X\,du/dX=(u^2+4)/(2-u)$, and [separation of variables](../../../separation-of-variables.md) gives

$$
\arctan(u/2)-\frac12\ln(u^2+4)=\ln|X|+C.
$$

Thus one local real implicit form is

$$
\boxed{\arctan\!\frac{y-1}{2(x-2)}-\frac12\ln\!\bigl(4(x-2)^2+(y-1)^2\bigr)=C.}
$$

The [arctangent](../../../inverse-tangent.md) branch must be continued on the chosen solution patch. More geometrically, set $r=\sqrt{4X^2+Y^2}$ and take a continuous local argument $\theta=\arg(2X+iY)$; then $\theta-\ln r=C$. This form extends through $X=0$ where the original slope is defined. The intersection itself is excluded because the original right-hand side is $0/0$ there, and points with $2X-Y=0$ do not define a finite derivative. No real constant-$u$ solution was lost, because $u^2+4$ has no real zero. Translating the intersection works precisely because the two affine linear forms then become homogeneous linear forms.

## ↑ Ancestors (11)

1. [7](../7.md)
2. [2021](../../2021-split.md)
3. [Past exam of the mathematical methods I course of the University of Oxford](../../split.md)
4. [Mathematical methods I course of the University of Oxford](../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
