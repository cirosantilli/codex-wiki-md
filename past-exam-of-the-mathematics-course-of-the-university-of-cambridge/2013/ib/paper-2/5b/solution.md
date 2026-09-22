<h1 id="5b/solution">Solution</h1>

↑ **Parent:** [5B](../5b.md)

Parametrize the [characteristics](../../../../../characteristic-of-a-field.md) by $s$, starting from $(x,y,u)=(1,r,r)$. Their [ordinary differential equations](../../../../../ordinary-differential-equation.md) are

$$
\frac{dx}{ds}=x,\qquad \frac{dy}{ds}=x+y,\qquad \frac{du}{ds}=1.
$$

They give $x=e^s$, $y=e^s(r+s)$ and $u=r+s$. Thus $s=\log x$ and $r=y/x-\log x$, so

$$
\boxed{u(x,y)=\frac yx\quad(x>0).}
$$

Indeed, $u_x=-y/x^2$, $u_y=1/x$ give $xu_x+(x+y)u_y=1$, and $u(1,y)=y$. The initial line is noncharacteristic, and its [characteristics](../../../../../characteristic-of-a-field.md) cover the half-plane $x>0$. The data do not determine a solution on $x<0$; a smooth solution through the origin is impossible because the differential equation there would read $0=1$.

## ↑ Ancestors (10)

1. [5B](../5b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
