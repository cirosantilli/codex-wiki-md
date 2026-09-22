# Seidel coma pupil mapping

↑ **Parent:** [Coma (optics)](coma-optics.md)

Consider an original, explicitly normalized model of primary [coma](coma-optics.md), rather than a prescription for a particular [optical lens](lens-optics.md). Let $(u,v)$ be [Cartesian coordinates](cartesian-coordinate-system.md) in a circular [optical pupil](optical-pupil.md) divided by its radius $a$, with $u^2+v^2\leq1$. Let $h=\alpha/\alpha_0$ be a signed small field [angle](angle.md) divided by an arbitrary positive reference [angle](angle.md). With [polar coordinates](polar-coordinates.md) $u=\rho\cos\theta$, $v=\rho\sin\theta$, prescribe the [wavefront error](wavefront-error.md)

$$
W(u,v)=W_0w(u,v),\qquad
w(u,v)=h\rho^3\cos\theta=h\,u(u^2+v^2).
$$

Here $W_0$ is an arbitrary positive [optical path difference](optical-path-difference.md) scale, not a measured error. The cubic [optical pupil](optical-pupil.md) dependence and linear field dependence are the classical Seidel form.[Amateur Telescope Optics, §4.2, classical coma formula after equation 15 and equation 13: pupil-cubic and field-linear dependence](amateur-telescope-optics-by-vladimir-sacek/coma-aberration.md)

In the [paraxial approximation](paraxial-approximation.md), [light ray](light-ray.md) direction errors follow the transverse [gradient](gradient.md) of [wavefront error](wavefront-error.md). For a reference sphere a distance $L$ from the exit [optical pupil](optical-pupil.md) in a uniform image medium of [refractive index](refractive-index.md) $n$, the corresponding image-error scale is $s=LW_0/(na)$. Choose image-error coordinate signs so the normalized displacement is $\nabla w$; reversing the convention reverses the plotted orientation. Image coordinates below are errors relative to the ideal image of this particular object point, rather than positions of different objects:

$$
X=\frac{\partial w}{\partial u}=h(3u^2+v^2),\qquad
Y=\frac{\partial w}{\partial v}=2huv.
$$

The [partial derivatives](partial-derivative.md) explain the asymmetry: opposite [optical pupil](optical-pupil.md) points $(u,v)$ and $(-u,-v)$ land together, rather than on opposite sides of the ideal image. For $h>0$, every $X$ is nonnegative, while $Y$ can have either sign. The figures stipulate this single [wavefront error](wavefront-error.md), omit other [optical aberrations](optical-aberration.md) and [diffraction](diffraction.md), and assign no instrument dimensions.

For a ring of fixed [optical pupil](optical-pupil.md) radius $\rho$, the double-angle formulas for [trigonometric functions](trigonometric-function.md) give

$$
X=h\rho^2(2+\cos2\theta),\qquad
Y=h\rho^2\sin2\theta,\qquad
(X-2h\rho^2)^2+Y^2=h^2\rho^4.
$$

Thus each ring maps into a [circle](circle.md) of radius $|h|\rho^2$ whose centre is displaced by $2h\rho^2$. Doubling $\rho$ quadruples both sizes; for $h=1$, the edge ring has centre $(2,0)$ and radius $1$, while the half-radius ring has centre $(1/2,0)$ and radius $1/4$. Superposing these displaced [circles](circle.md) produces the comet-like envelope.

<a id="seidel-coma-pupil-ring-mapping"></a>
![](seidel-coma-pupil-ring-mapping.png)

**[Figure 10](#seidel-coma-pupil-ring-mapping). Primary coma: optical pupil rings map into displaced image circles**. Original normalized [Seidel coma pupil mapping](seidel-coma-pupil-mapping.md) at $h=1$. Colours identify equal-radius [optical pupil](optical-pupil.md) rings and their image [circles](circle.md); crosses mark circle centres. The opposite points A and B have the same image position. These are [light ray](light-ray.md) intersections, with no instrument dimensions or [diffraction](diffraction.md) calculation.

For uniform [irradiance](irradiance.md) over the circular [optical pupil](optical-pupil.md), equal [area](surface-area.md) samples give an equal-weight geometrical image. Its [centroid](centroid.md) is $(h,0)$ because $\langle u^2\rangle=\langle v^2\rangle=1/4$ and $\langle uv\rangle=0$. Moving the coordinate origin to that [centroid](centroid.md) translates the image; it does not remove its asymmetric shape. Adding a linear term to $w$ likewise translates all [light rays](light-ray.md) equally. These origin choices must be distinguished from changing the [optical aberration](optical-aberration.md) itself.

<a id="seidel-coma-off-axis-point-image"></a>
![](seidel-coma-off-axis-point-image.png)

**[Figure 11](#seidel-coma-off-axis-point-image). The normalized geometrical point image grows and reverses with field angle**. Original equal-[area](surface-area.md) sampling of the same circular [optical pupil](optical-pupil.md), mapped at $h=0,1/2,1,-1$ with one image scale. The orange cross is the geometrical [centroid](centroid.md). Each blue point represents one equal-weight [light ray](light-ray.md); point density is not a calibrated [light intensity](light-intensity.md) display or a measured [point spread function](point-spread-function-split.md). At $h=0$ all model [light rays](light-ray.md) coincide, while a real finite [aperture](aperture.md) still gives [diffraction](diffraction.md).

The model's full transverse extent is $3|h|$ along $X$ and $2|h|$ along $Y$. Halving the field [angle](angle.md) halves the blur, and reversing it reverses the pattern about the ideal image. This isolates why [coma](coma-optics.md) matters for an [optical camera](optical-camera.md)'s usable [field of view](field-of-view.md): collecting more [light](light.md) does not ensure that off-axis points remain compact. Near [diffraction-limited resolution](diffraction-limited-resolution.md), a [physical optics](physical-optics-split.md) calculation of the [point spread function](point-spread-function-split.md) is needed instead of interpreting the geometrical tip as an infinitely sharp image.[Amateur Telescope Optics, §4.2, Figure 41: geometrical spots versus diffraction images](amateur-telescope-optics-by-vladimir-sacek/coma-aberration.md)

## ↑ Ancestors (8)

1. [Coma (optics)](coma-optics.md)
2. [Seidel aberration](seidel-aberration.md)
3. [Optical aberration](optical-aberration.md)
4. [Geometrical optics](geometrical-optics-split.md)
5. [Optics](optics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Off-axis pinhole test for coma](off-axis-pinhole-test-for-coma.md)
- [Seidel coma pupil mapping](seidel-coma-pupil-mapping.md)
