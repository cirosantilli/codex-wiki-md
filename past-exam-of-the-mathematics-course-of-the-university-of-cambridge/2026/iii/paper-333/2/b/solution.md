<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The eastern wall has no normal flow, so the [quasi-geostrophic streamfunction](../../../../../../quasi-geostrophic-streamfunction.md) is constant there. Choose $\psi(L,y)=0$. Integrating the Sverdrup relation gives

$$
\boxed{
\psi_{\rm int}(x,y)
=\frac{f_0\tau'(y)}{\beta\rho H_0^2}(L-x)}.
$$

Since [geostrophic balance](../../../../../../geostrophic-balance.md) gives $\psi=g\eta/f_0$,

$$
\boxed{
\eta_{\rm int}(x,y)
=\frac{f_0^2\tau'(y)}
{g\beta\rho H_0^2}(L-x)}.
$$

If this interior solution were extended to both walls, the west-minus-east height difference would be

$$
\boxed{
\eta_{\rm int}(0,y)-\eta_{\rm int}(L,y)
=\frac{f_0^2L}{g\beta\rho H_0^2}\tau'(y)}.
$$

The northward volume transport per unit meridional distance is

$$
T=H_0\int_0^L v\,dx
=H_0\int_0^L\psi_x\,dx
=\frac{gH_0}{f_0}\,[\eta(L,y)-\eta(0,y)].
$$

Thus

$$
\boxed{
T=-\frac{f_0L}{\beta\rho H_0}\tau'(y)}.
$$

This is the basin-integrated form of [Sverdrup balance](../../../../../../sverdrup-balance.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 333](../../../paper-333-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
