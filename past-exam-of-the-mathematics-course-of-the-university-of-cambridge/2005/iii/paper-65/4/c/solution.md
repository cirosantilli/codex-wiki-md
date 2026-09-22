<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The displayed orbit has the normalization **$\alpha=1$**. To verify it put $z=\tanh(\tau/\sqrt2)$ and $f=1-z^2=\operatorname{sech}^2(\tau/\sqrt2)$. Then $z'=f/\sqrt2$, $f'=-\sqrt2 fz$, so

$$
u'=3\sqrt2 fz=v,\qquad
v'=3f(1-3z^2).
$$

Also $u=-2+3z^2$, and $(u^2-1)=3(1-z^2)(1-3z^2)$, exactly the same expression as $v'$. Therefore the conservative equations hold. As $\tau\to\pm\infty$, $(u,v)\to(1,0)$; at $\tau=0$ the orbit reaches $(-2,0)$. Its conserved energy is $2/3$, so this is the required [homoclinic orbit](../../../../../../homoclinic-orbit.md).

For a general positive $\alpha$ set $s=\sqrt\alpha$. Rescaling the verified solution gives

$$
\boxed{u=s\left[1-3\operatorname{sech}^2\left(\frac{\sqrt s\,\tau}{\sqrt2}\right)\right],\quad
v=3\sqrt2\,s^{3/2}\operatorname{sech}^2\left(\frac{\sqrt s\,\tau}{\sqrt2}\right)
\tanh\left(\frac{\sqrt s\,\tau}{\sqrt2}\right).}
$$

Direct differentiation gives $u'=v$ and $v'=u^2-\alpha$, and the endpoints are $(s,0)$. This restores the parameter dependence implicit in the normalized printed orbit.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
