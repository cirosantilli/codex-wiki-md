<h1 id="section-b/b8/solution">Solution</h1>

↑ **Parent:** [B8](../b8.md)

At screen coordinate $X$, the propagation length from [aperture](../../../../../aperture.md) coordinate $x$ is $[D^2+(X-x)^2]^{1/2}$. Its expansion has a constant term, a term linear in $x$ giving the observation angle, and a quadratic term of order $x^2/(2D)$. For $|x|\leq d/2$, the quadratic [wave phase](../../../../../phase-waves.md) is at most of order $\pi d^2/(4\lambda D)$. Requiring it to be much smaller than one gives the sufficient condition **$D\gg d^2/\lambda$**; higher terms are then smaller in the paraxial geometry. In the [lens](../../../../../lens-optics.md) arrangement, put the source at the first [lens](../../../../../lens-optics.md)'s front focus, illuminate the grating with its collimated output, and put the screen at the second [lens](../../../../../lens-optics.md)'s back [focal plane](../../../../../focal-plane.md). This obtains the angular [Fraunhofer diffraction](../../../../../fraunhofer-diffraction.md) pattern without a physically very distant screen.

<a id="section-b/b8/image-two-lens-arrangement-for-a-grating-diffraction-pattern"></a>
![](../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2011/paper-1-grating-layout.png)

**[Figure 4](#section-b/b8/image-two-lens-arrangement-for-a-grating-diffraction-pattern). Two-lens arrangement for a grating diffraction pattern**. Original schematic ray construction. Equal outgoing ray slopes meet at a common back-focal-plane position; distances and angles are illustrative.

The slit pitch is $p=1/(200\,\mathrm{mm^{-1}})=5.00\,\mathrm{\mu m}$. Normal-incidence maxima satisfy $p\sin\theta=m\lambda$. Thus $\sin\theta_3=0.276$ and, using rectilinear focal-plane geometry,

$$
\boxed{x_3=\pm f\tan\theta_3=\pm86.1\,\mathrm{mm}.}
$$

The paraxial result $x_3\simeq fm\lambda/p=\pm82.8\,\mathrm{mm}$ is a roughly 4% lower approximation; an actual wide-angle [lens](../../../../../lens-optics.md)'s mapping depends on its design. The angular result does not depend on that convention.

For $N$ uniformly illuminated equal slits of width $w$, the diffraction [intensity](../../../../../intensity-physics.md) has the form

$$
I(\theta)=Cw^2\operatorname{sinc}^2\!\left(\frac{\pi w\sin\theta}{\lambda}\right)
\left[\frac{\sin(N\pi p\sin\theta/\lambda)}{\sin(\pi p\sin\theta/\lambda)}\right]^2,\quad \operatorname{sinc}u=\frac{\sin u}u.
$$

Here $C$ is unchanged when the incoming [intensity](../../../../../intensity-physics.md) is fixed. The broad [single-slit diffraction](../../../../../single-slit-diffraction.md) envelope multiplies the narrow grating orders. At a principal maximum,

$$
I_m=CN^2w^2\operatorname{sinc}^2(\pi mw/p).
$$

The [fixed-illumination grating peak change with slit width](../../../../../fixed-illumination-grating-peak-change-with-slit-width.md) gives the changes from $w=1.0$ to $1.5\,\mathrm{\mu m}$ are

$$
\boxed{I_{0,\rm new}/I_{0,\rm old}=2.25},\qquad
\boxed{I_{3,\rm new}/I_{3,\rm old}=\left[\frac{\sin(0.9\pi)}{\sin(0.6\pi)}\right]^2=0.1056.}
$$

The central peak increases by 125%, while the third-order peak decreases by about 89.4%. Separate normalizations to each central peak would hide this effect. The following width-specific solutions and profiles use a common incoming normalization.

## ↑ Ancestors (14)

1. [B8](../b8.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2011](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
