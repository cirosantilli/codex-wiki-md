<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the [quasi-geostrophic approximation](../../../../../../quasi-geostrophic-approximation.md), buoyancy is proportional to $f\psi_z$ and its material equation gives

$$
w=-\frac f{N^2}\frac{D_g\psi_z}{Dt}.
$$

The governing interior and boundary equations are consequently

$$
\boxed{\frac{D_g}{Dt}\left(\nabla_h^2\psi+\frac{f^2}{N^2}\psi_{zz}\right)=0\quad(z>0),}
$$



$$
\boxed{\frac{D_g\psi_z}{Dt}=-\frac{N^2\delta}{2f}\nabla_h^2\psi\quad(z=0).}
$$

After linearization about rest, put $m=Nk/|f|$ and $r=Nk\delta/2$. The initial PV is $-k^2\psi_0\sin kx$, and the decaying homogeneous vertical solution gives

$$
\boxed{psi=\psi_0\left[1-(1-e^{-rt})e^{-mz}\right]\sin kx.}
$$

The boundary current decays on time $r^{-1}=2/(Nk\delta)$, while the original current survives aloft. The boundary influence penetrates only

$$
\boxed{m^{-1}=\frac{|f|}{Nk}.}
$$

Stronger stratification or shorter horizontal scale confines the adjustment more tightly; rotation communicates it farther upward. This is [quasi-geostrophic Ekman spin-down](../../../../../../quasi-geostrophic-ekman-spin-down.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 333](../../../paper-333-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
