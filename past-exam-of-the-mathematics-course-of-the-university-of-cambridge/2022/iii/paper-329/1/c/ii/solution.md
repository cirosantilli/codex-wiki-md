<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $\boldsymbol\Omega=\mathbf G_1/(8\pi\mu a^3)$. The incident [rotlet](../../../../../../../rotlet.md) of sphere 1 at sphere 2 is

$$
\mathbf u_\infty(\mathbf R)=a^3\frac{\boldsymbol\Omega\times\mathbf R}{R^3},
$$

and it is harmonic away from sphere 1. Since sphere 2 is [force-free](../../../../../../../force-free.md), [Faxén's first law](../../../../../../../faxen-s-first-law.md) therefore gives

$$
\boxed{\mathbf U_2=a^3\frac{\boldsymbol\Omega\times\mathbf R}{R^3}.}
$$

The [vorticity](../../../../../../../vorticity.md) of the rotlet is

$$
\boldsymbol\omega_\infty(\mathbf R)
=\frac{a^3}{R^3}\left[
3\frac{(\boldsymbol\Omega\cdot\mathbf R)\mathbf R}{R^2}
-\boldsymbol\Omega
\right].
$$

Because $\mathbf G_2=0$, [Faxén's rotational law](../../../../../../../faxen-s-rotational-law.md) gives

$$
\boxed{\boldsymbol\Omega_2
=\frac{a^3}{2R^3}\left[
3\frac{(\boldsymbol\Omega\cdot\mathbf R)\mathbf R}{R^2}
-\boldsymbol\Omega
\right].}
$$

The symmetric [rate-of-strain tensor](../../../../../../../strain-rate-tensor.md) of the incident rotlet at sphere 2 is

$$
\mathbf E=-\frac{3a^3}{2R^5}\left[
(\boldsymbol\Omega\times\mathbf R)\mathbf R
+\mathbf R(\boldsymbol\Omega\times\mathbf R)
\right].
$$

After translation and rotation have matched the uniform and antisymmetric parts of the incident flow, the leading perturbation from sphere 2 is the [stresslet](../../../../../../../force-dipole-flow.md) part of the supplied straining-sphere solution:

$$
\boxed{\mathbf u_2'(\mathbf x)
\sim-\frac{5a^3}{2}\frac{(\mathbf x\cdot\mathbf E\cdot\mathbf x)\mathbf x}{r^5}.}
$$

Part b gives its vorticity as

$$
\boldsymbol\omega_2'=5a^3\frac{\mathbf x\times(\mathbf E\cdot\mathbf x)}{r^5}.
$$

At the centre of sphere 1, $\mathbf x=-\mathbf R$, so

$$
\boldsymbol\omega_2'(-\mathbf R)
=-\frac{15a^6}{2R^6}\left[
\boldsymbol\Omega-\frac{(\boldsymbol\Omega\cdot\mathbf R)\mathbf R}{R^2}
\right].
$$

Applying [Faxén's rotational law](../../../../../../../faxen-s-rotational-law.md) to sphere 1 produces half this ambient vorticity and proves

$$
\boxed{
\boldsymbol\Omega_1-\boldsymbol\Omega
=-\frac{15a^6}{4R^6}\left[
\boldsymbol\Omega-\frac{(\boldsymbol\Omega\cdot\mathbf R)\mathbf R}{R^2}
\right].}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 329](../../../../paper-329-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
