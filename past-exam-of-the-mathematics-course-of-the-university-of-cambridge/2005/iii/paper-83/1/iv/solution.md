<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For a straight unit-winding [quantum vortex](../../../../../../quantum-vortex.md), the real radial amplitude satisfies

$$
R''+\frac1sR'-\frac R{s^2}+(1-R^2)R=0,
\qquad R(0)=0,\quad R(\infty)=1.
$$

In the frame translating with the ring, put $Z=z-ut$ and $\Phi=e^{i\theta}(R+\phi)$, where $\phi$ is independent of the angular coordinate. The cylindrical [Laplacian](../../../../../../laplacian.md) has the exact identity

$$
\nabla^2[e^{i\theta}(R+\phi)]
=e^{i\theta}\left[\frac1s\partial_s(s\partial_s(R+\phi))+\partial_Z^2\phi-\frac{R+\phi}{s^2}\right].
$$

After inserting this into the translating [Gross–Pitaevskii equation](../../../../../../gross-pitaevskii-equation.md), subtract the straight-vortex equation. Because $R$ is real,

$$
|R+\phi|^2=R^2+R(\phi+\phi^*)+|\phi|^2,
$$

and direct expansion of the nonlinear difference gives

$$
(1-|R+\phi|^2)(R+\phi)-(1-R^2)R
=(1-2R^2)\phi-R^2\phi^*-R\phi^2-2R|\phi|^2-|\phi|^2\phi.
$$

Thus the exact ring-on-line perturbation equation, including its quadratic and cubic terms, is

$$
\boxed{2iu\phi_Z=\frac1s\partial_s(s\phi_s)+\phi_{ZZ}-\frac\phi{s^2}
+\bigl[1-2R^2-R(\phi+2\phi^*)-|\phi|^2\bigr]\phi-R^2\phi^*.}
$$

The two appearances of $R|\phi|^2$ are responsible for the coefficient $2$ multiplying $\phi^*$ inside the bracket. No small-amplitude approximation is needed for this identity.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 83](../../../paper-83-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
