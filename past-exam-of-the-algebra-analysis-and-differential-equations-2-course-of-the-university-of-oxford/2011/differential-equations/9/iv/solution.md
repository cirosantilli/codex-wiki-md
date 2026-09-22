<h1 id="differential-equations/9/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Differentiating the transform with respect to $p$ gives

$$
\boxed{\mathcal L[ty](p)=-\frac d{dp}\overline y(p).}
$$

Applying this to $\mathcal L[1]=1/p$ also gives $\boxed{\mathcal L[t]=1/p^2}$ for $\operatorname{Re}p>0$.

Now put $Y=\overline y$, $y_0=y(0)$ and $v_0=\dot y(0)$. Transforming each term of the differential equation, and using the [derivative](../../../../../derivative.md) identities, gives

$$
-\frac d{dp}(p^2Y-py_0-v_0)-\frac d{dp}(pY-y_0)+(pY-y_0)+Y=\frac1{p^2}.
$$

The initial-value terms cancel, leaving

$$
-p(p+1)Y'-pY=\frac1{p^2},\qquad
\frac d{dp}\{(p+1)Y\}=-\frac1{p^3}.
$$

Integrating once yields $(p+1)Y=C+1/(2p^2)$. Partial fractions give

$$
Y=\frac C{p+1}+\frac1{2p^2(p+1)}
=\frac{C+1/2}{p+1}-\frac1{2p}+\frac1{2p^2}.
$$

The transform pairs therefore imply, on writing $A=C+1/2$,

$$
\boxed{y(t)=Ae^{-t}+\frac{t-1}{2}.}
$$

For the final parameter count, the differential equation is the [derivative](../../../../../derivative.md) of $t(\dot y+y)$: it says $[t(\dot y+y)]'=t$. Integrating gives $t(\dot y+y)=t^2/2+B$. A regular solution at $t=0$ has finite $y$ and $\dot y$, forcing $B=0$. Thus $\dot y+y=t/2$ is first order and leaves only one constant. Equivalently, the original equation at zero requires $\dot y(0)+y(0)=0$, so the two usual initial values cannot be chosen independently. The displayed solution satisfies this constraint and verifies the original equation directly.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [9](../../9.md)
3. [Differential Equations](../../../differential-equations.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
