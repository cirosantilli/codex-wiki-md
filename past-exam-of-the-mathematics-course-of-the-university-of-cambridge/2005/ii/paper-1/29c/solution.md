<h1 id="29c/solution">Solution</h1>

↑ **Parent:** [29C](../29c.md)

For a regular defining function $\phi$, the hypersurface is [non-characteristic](../../../../../non-characteristic-hypersurface.md) when the characteristic [vector](../../../../../vector.md) has nonzero normal component:

$$
\boxed{x_2\phi_{x_1}-x_1\phi_{x_2}+a\phi_{x_3}\ne0\quad\text{on }S_\phi.}
$$

For $\phi=x_3$ this is precisely $a\ne0$. The defining function must also have nonzero gradient so that it actually defines a hypersurface.

The [method of characteristics](../../../../../method-of-characteristics.md) gives $\dot x_1=x_2$, $\dot x_2=-x_1$, $\dot x_3=a$, $\dot u=u$. Starting at $(\xi_1,\xi_2,0)$, the first two coordinates rotate clockwise through characteristic time $s$ and $x_3=as$. Solving back for the initial point gives

$$
\boxed{u(x_1,x_2,x_3)=e^{x_3/a}f\left(x_1\cos\frac{x_3}a-x_2\sin\frac{x_3}a,\ x_1\sin\frac{x_3}a+x_2\cos\frac{x_3}a\right).}
$$

It meets the data and is $C^1$ when $f$ is $C^1$.

For the rotationally invariant data, $u=(x_1^2+x_2^2)e^{x_3/a}$. As $a\to0^+$ it tends to zero for fixed $x_3<0$, diverges to positive infinity for fixed $x_3>0$ and nonzero radius, and retains the initial value on $x_3=0$. It is identically zero on the vertical axis. **There is no regular limit across the initial plane.** At $a=0$ that plane is characteristic and the data would need to satisfy $x_2f_{x_1}-x_1f_{x_2}=f$; the chosen radial data violate this except at the origin, explaining the singular limit.

## ↑ Ancestors (10)

1. [29C](../29c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
