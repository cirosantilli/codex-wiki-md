<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take the drift propagator with the correct initial normalization, $U_0(t,t_0)=e^{-i(t-t_0)H_0}$, and define the [interaction picture](../../../../../../interaction-picture.md) by $U=U_0U_I$. Differentiate this product and substitute the [Schrödinger equation](../../../../../../schrodinger-equation.md):

$$
i\dot U_0U_I+iU_0\dot U_I=\left(H_0+\sum_m f_mH_m\right)U_0U_I.
$$

Since $i\dot U_0=H_0U_0$, the drift terms cancel. Left multiplication by $U_0^\dagger$ gives

$$
\boxed{i\dot U_I=\sum_m f_m(t)\widetilde H_m(t)U_I,\qquad \widetilde H_m=U_0^\dagger H_mU_0,\qquad U_I(t_0,t_0)=I.}
$$

The printed $e^{-itH_0}$ is this expression with time origin $t_0=0$. Its differential identity remains valid at arbitrary $t_0$, but its interaction-picture initial operator would then be $e^{it_0H_0}$ rather than the identity. Using $t-t_0$ resolves that normalization without changing the derivation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
