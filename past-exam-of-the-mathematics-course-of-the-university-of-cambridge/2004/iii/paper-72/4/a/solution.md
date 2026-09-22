<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the finite crack use the branch

$$
\chi(z)=\sqrt{z^2-a^2},\qquad \chi(z)\sim z\text{ at infinity},
$$

cut on $[-a,a]$. For $-a<t<a$, its limiting values are $\chi^+(t)=i\sqrt{a^2-t^2}$ and $\chi^-(t)=-i\sqrt{a^2-t^2}$. Consequently $H=\chi G$ converts the sum condition of the [Hilbert problem for an antiplane crack](../../../../../../hilbert-problem-for-an-antiplane-crack.md) into an additive jump:

$$
H^+-H^-=\chi^+(G^++G^-)=-2i\sqrt{a^2-t^2}\,p(t).
$$

By the [Sokhotski–Plemelj theorem](../../../../../../sokhotski-plemelj-theorem.md), the [Cauchy integral](../../../../../../cauchy-transform.md) with this jump is

$$
H(z)=\frac1{2\pi i}\int_{-a}^a\frac{-2i\sqrt{a^2-t^2}\,p(t)}{t-z}\,dt
=\frac1\pi\int_{-a}^a\frac{\sqrt{a^2-t^2}\,p(t)}{z-t}\,dt.
$$

Thus the [finite antiplane crack Cauchy solution](../../../../../../finite-antiplane-crack-cauchy-solution.md) is $G=H/\chi$. For regular integrable loading, $H=O(z^{-1})$ and $G=O(z^{-2})$. A homogeneous term $C/\chi$ would instead produce a logarithmic potential. In the reflected real-loading class $C$ is real, and its $1/z$ term gives a nonzero displacement period around the crack. It is excluded for the induced, dislocation-free correction. A nonvanishing constant stress term would change the remote applied field and is likewise excluded.

For $x=x_1>a$, $\chi(x)=\sqrt{x^2-a^2}>0$, so

$$
\boxed{\sigma_{23}(x,0)+i\sigma_{13}(x,0)=\frac1{\pi\sqrt{x^2-a^2}}\int_{-a}^a\frac{\sqrt{a^2-t^2}\,\sigma_{23}^A(t,0)}{x-t}\,dt.}
$$

This is the additional stress, not the total stress; the applied field must still be added. The integral is real at these intact-axis points, so $\sigma_{13}(x,0)=0$. On the crack itself, the upper [Cauchy principal value](../../../../../../cauchy-principal-value.md) formula gives $H^+=\pi^{-1}\operatorname{PV}\int\sqrt{a^2-t^2}p(t)/(x-t)\,dt-i\sqrt{a^2-x^2}p(x)$. Division by $i\sqrt{a^2-x^2}$ verifies $\operatorname{Re}G^+=-p$, checking the sign of the face traction cancellation.

For example, constant applied shear $p_0$ gives $H(z)=p_0(z-\chi(z))$ and $G(z)=p_0(z/\chi(z)-1)$. The total shear ahead of the crack is then $p_0x/\sqrt{x^2-a^2}$, providing a direct check of the normalization and the crack-tip singularity.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
