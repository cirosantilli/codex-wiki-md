<h1 id="15d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The inverse [Lorentz transformation of electromagnetic fields](../../../../../../lorentz-transformation-of-electromagnetic-fields.md), from the primed rest frame to the unprimed frame, gives

$$
\boxed{
E_x=E_x',\qquad E_y=\gamma E_y',\qquad E_z=\gamma E_z'
}
$$

and

$$
\boxed{
B_x=0,\qquad
B_y=-\frac{\gamma v}{c^2}E_z',\qquad
B_z=\frac{\gamma v}{c^2}E_y'
}.
$$

Equivalently, $\mathbf B=\gamma\,\mathbf v\times\mathbf E'/c^2$ for $\mathbf v=v\mathbf e_x$.

Using $1/\mu_0=\epsilon_0c^2$ and $\gamma^2=(1-v^2/c^2)^{-1}$,

$$
\begin{aligned}
w
&=\frac{\epsilon_0}{2}\left[
E_x'^2+\gamma^2(E_y'^2+E_z'^2)
+\gamma^2\frac{v^2}{c^2}(E_y'^2+E_z'^2)
\right]\\
&=\boxed{\frac{\epsilon_0}{2}\left[
E_x'^2+\frac{c^2+v^2}{c^2-v^2}
(E_y'^2+E_z'^2)\right]}.
\end{aligned}
$$

The primed field is static, so $w$ depends on $t,x$ through

$$
x'=\gamma(x-vt)
$$

and has no explicit $t'$ dependence. The [chain rule](../../../../../../chain-rule.md) gives

$$
\partial_tw=-\gamma v\,\partial_{x'}w,
\qquad
\partial_xw=\gamma\,\partial_{x'}w.
$$

Consequently

$$
\boxed{
\frac{\partial w}{\partial t}
+\nabla\mathbin{\cdot}(wv\mathbf e_x)
=\partial_tw+v\partial_xw=0
}.
$$

**Thus the field-energy profile is transported rigidly with velocity $v\mathbf e_x$.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [15D](../../15d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
