# Microscope scale calibration

↑ **Parent:** [Optical microscope](optical-microscope.md)

[Microscope scale calibration](microscope-scale-calibration.md) compares an image readout with a known specimen [length](length.md). This documented practical uses an [eyepiece graticule](ocular-micrometer.md), [stage micrometer](stage-micrometer.md) and [Köhler illumination](kohler-illumination.md). Focus the graticule; place the reference on the stage with the objective-appropriate cover glass. Focus both scales with the chosen [microscope objective](microscope-objective.md), then rotate and translate them into parallel alignment. Read widely separated coincidences using consistent line edges. Record the optical configuration and recalibrate for each objective.[Linear Measurements (Micrometry), Stage Micrometers and Eyepiece Reticle Calibration, Fig. 4 and procedure bullets](linear-measurements-micrometry-by-thomas-j-fellers-and-michael-w-davidson.md)

The [stage micrometer](stage-micrometer.md) is the reference; preserve the optical configuration when substituting the specimen. Line width, focus, edge selection and [optical aberrations](optical-aberration.md) limit accuracy. Additional recommended checks are realignment and another known interval: agreement tests repeatability and scale consistency, not absolute reference accuracy.[Linear Measurements (Micrometry), Conclusions, line-edge choice and calibration errors; repeat-after-realignment check is an additional recommendation](linear-measurements-micrometry-by-thomas-j-fellers-and-michael-w-davidson.md)

Here is an original toy calculation, not the source's calibration example or measured data. Suppose a reference span $L=100\,\mathrm{\mu m}$ coincides with $N=40$ eyepiece intervals. Then the calibration factor and the [length](length.md) corresponding to $n=18$ specimen intervals are

$$
c=\frac{L}{N}=2.5\,\mathrm{\mu m}\text{ per interval},\qquad \ell=nc=45\,\mathrm{\mu m}.
$$

This works because both readouts use the same image-to-specimen scale: $\ell/L=n/N$. One must count intervals, not tick marks; forty intervals have forty-one bounding ticks. In an ideal linear scale model, if identifying the calibration endpoints introduces a total readout error of $\pm1$ interval, the inferred factor ranges from $100/41$ to $100/39\,\mathrm{\mu m}$ per interval. Holding $n=18$ exact gives $43.90\leq\ell/\mathrm{\mu m}\leq46.15$. This isolates one contribution to [measurement uncertainty](measurement-uncertainty.md); it is not a complete uncertainty budget or a measured confidence interval.

<a id="image-microscope-scale-calibration-measures-length-empty-magnification-only-enlarges-an-existing-image"></a>
![](microscope-calibration-and-empty-magnification.png)

**[Figure 8](#image-microscope-scale-calibration-measures-length-empty-magnification-only-enlarges-an-existing-image). Microscope scale calibration measures length; empty magnification only enlarges an existing image**. Original upper-panel toy alignment: $100\,\mathrm{\mu m}$ spans forty eyepiece intervals, so eighteen intervals represent $45\,\mathrm{\mu m}$. Lower panels show the same stipulated blurred two-source profile on two display scales; both feature separation and blur expand together. A Gaussian illustration is used for legibility, not as a measured profile or an exact [Airy disk](airy-disk.md).

For a recorded [real image](real-image.md), image a [stage micrometer](stage-micrometer.md) at the same capture settings to calibrate [length](length.md) per [detector pixel](optical-detector-pixel.md). Resizing changes [length](length.md) per [pixel](pixel.md); update the scale bar accordingly. Eye-viewing [angular magnification](angular-magnification.md) alone supplies no digital image scale.[Linear Measurements (Micrometry), Conclusions, digital images acquired at identical pixel resolution](linear-measurements-micrometry-by-thomas-j-fellers-and-michael-w-davidson.md)

**Table of contents**

- [Ocular micrometer](ocular-micrometer.md)
- [Stage micrometer](stage-micrometer.md)

## ↑ Ancestors (6)

1. [Optical microscope](optical-microscope.md)
2. [Optical instrument](optical-instrument-split.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Empty magnification](empty-magnification.md)
- [Microscope scale calibration](microscope-scale-calibration.md)
- [Ocular micrometer](ocular-micrometer.md)
- [Optical microscope](optical-microscope.md)
- [Stage micrometer](stage-micrometer.md)
- [Transmission electron microscopy specimen dose and calibration](transmission-electron-microscopy-specimen-dose-and-calibration.md)
