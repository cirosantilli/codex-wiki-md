<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Specific intensity is defined by $dE=I_\nu\cos\theta\,dA\,d\Omega\,d\nu\,dt$. A ray bundle in free space expands in area while its solid angle contracts by the same factor, so

$$
\boxed{\frac{dI_\nu}{ds}=0}.
$$

Thus [specific intensity](../../../../../../specific-intensity.md) does not obey an inverse-square law; the flux of an unresolved source does because its apparent solid angle scales as distance${}^{-2}$.

For a cold medium with coherent, isotropic, conservative scattering, the source function is the [mean intensity](../../../../../../mean-intensity.md) $J_\nu$. With scattering optical depth increasing along the ray,

$$
\frac{dI_\nu}{d\tau_\nu}=-I_\nu+J_\nu,
$$

and

$$
\boxed{
I_\nu(\tau)=I_\nu(0)e^{-\tau}
+\int_0^\tau J_\nu(t)e^{-(\tau-t)}dt}.
$$

The unscattered pencil beam is attenuated by $e^{-\tau}$ and reappears as a diffuse halo in other directions. Coherent scattering preserves frequency, and conservative scattering preserves total luminosity when all outgoing directions are collected.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 315](../../../paper-315-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
