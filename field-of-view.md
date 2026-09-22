# Field of view

↑ **Parent:** [Optical instrument](optical-instrument-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Field_of_view)

The [field of view](field-of-view.md) is the region of object directions sampled by an [optical instrument](optical-instrument-split.md) in one pointing. State whether it is horizontal, vertical or diagonal, and whether it is a full [angle](angle.md) or a half-[angle](angle.md). An object-plane width in millimetres also describes a [field of view](field-of-view.md), but requires a specified object distance. Neither that width nor the angular [field of view](field-of-view.md) is the [aperture](aperture.md) [diameter](diameter.md) or the [diffraction-limited resolution](diffraction-limited-resolution.md).

For a centred flat rectangular [photodetector](photodetector.md) of width $w$ in the [focal plane](focal-plane.md), with positive effective [focal length](focal-length.md) $f$, infinity focus and ideal rectilinear imaging without [optical distortion](distortion-optics.md), the full horizontal [field of view](field-of-view.md) is

$$
\Theta_x=2\arctan\left(\frac{w}{2f}\right).
$$

The model maps an object direction $\theta$ to image height of magnitude $|y|=f|\tan\theta|$; set $|y|=w/2$ and use the [inverse tangent](inverse-tangent.md). This retains exact [right triangle](right-triangle.md) geometry within the stipulated imaging model; a paraxial [focal length](focal-length.md) alone does not guarantee that a real wide-field [optical lens](lens-optics.md) obeys it. With detector height $h$, replace $w$ by $h$ for the vertical [field of view](field-of-view.md), and by $\sqrt{w^2+h^2}$ for the diagonal [field of view](field-of-view.md). The [small-angle approximation](small-angle-approximation.md) gives $\Theta_x\simeq w/f$ in radians. [Gregory Hollows and Nicholas James, Edmund Optics, Understanding Focal Length and Field of View](https://www.edmundoptics.com/knowledge-center/application-notes/imaging/understanding-focal-length-and-field-of-view/).

For an original worked example, a $36\,\mathrm{mm}$ detector width gives $\Theta_x\approx39.60^\circ$ at $f=50\,\mathrm{mm}$, and $20.41^\circ$ at $f=100\,\mathrm{mm}$. Keeping $D=25\,\mathrm{mm}$ makes these f/2 and f/4 respectively: the [field of view](field-of-view.md) changes because $f$ changes. By contrast, closing $D$ from $25$ to $12.5\,\mathrm{mm}$ at $f=100\,\mathrm{mm}$ changes f/4 to f/8 while retaining $20.41^\circ$ in this model. The clean separation is useful: [entrance pupil](entrance-pupil.md) [area](surface-area.md) controls collection, [focal ratio](focal-ratio.md) controls the paraxial cone, and $w/f$ controls angular image coverage. Edge clipping, [optical distortion](distortion-optics.md), [field curvature](petzval-field-curvature.md) and [optical aberrations](optical-aberration.md) can restrict the practically usable [field of view](field-of-view.md).

<a id="image-field-of-view-a-fixed-detector-width-subtends-a-smaller-angle-at-longer-focal-length"></a>
![](aperture-focal-ratio-field-view-sensor-geometry.png)

**[Figure 6](#image-field-of-view-a-fixed-detector-width-subtends-a-smaller-angle-at-longer-focal-length). Field of view: a fixed detector width subtends a smaller angle at longer focal length**. Original ideal rectilinear model. Left: central [light rays](light-ray.md) cross the [thin lens](thin-lens.md) centre and reach the two detector edges, with equal coordinate scales in both panels; the opening is $25\,\mathrm{mm}$ in each. Right: calculated full horizontal [field of view](field-of-view.md) for $w=36\,\mathrm{mm}$, with the $50$ and $100\,\mathrm{mm}$ examples marked. The detector lies in the [focal plane](focal-plane.md), the object is at infinity, and [optical distortion](distortion-optics.md) is absent. No plotted quantity is measured data.

A proposed angular readout on an [optical bench](optical-bench.md) illuminates a small asymmetric target at the [optical focus](focus-optics.md) of a [collimator](collimator.md), providing a bundle with a known direction. Rotate the [optical camera](optical-camera.md) about the centre of its [entrance pupil](entrance-pupil.md), reading a graduated rotation stage, and record the target image position on its fixed [photodetector](photodetector.md). Centre the target to establish zero; turn left and right until its centre reaches each detector edge. The difference between stage readings measures the full horizontal [field of view](field-of-view.md). Repeat with a smaller [aperture stop](aperture-stop.md): unchanged edge directions but reduced signal support the distinction between collection and angular coverage. Keep the same active detector width, infinity focus, illumination, integration time and gain; approach each reading from the same direction to check mechanical backlash. A finite target blurs the edge criterion, detector thresholds can imitate lost coverage, and a wide bundle must illuminate the whole [entrance pupil](entrance-pupil.md) at every tested [angle](angle.md). These checks distinguish a geometrical boundary from insufficient signal. The analytical diagram is the prediction for this protocol, not a record of its execution.

## ↑ Ancestors (5)

1. [Optical instrument](optical-instrument-split.md)
2. [Optics](optics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Aperture](aperture.md)
- [Coma (optics)](coma-optics.md)
- [Field of view](field-of-view.md)
- [Point spread function](point-spread-function-split.md)
- [Seidel coma pupil mapping](seidel-coma-pupil-mapping.md)
