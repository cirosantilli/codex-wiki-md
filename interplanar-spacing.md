# Interplanar spacing

↑ **Parent:** [Lattice plane](lattice-plane.md)

The [interplanar spacing](interplanar-spacing.md) $d$ is the perpendicular [distance between parallel planes](distance-between-parallel-planes.md) in a specified family. Measuring along an oblique line gives a larger distance, so the direction of measurement matters.

There is a short [reciprocal lattice](reciprocal-lattice.md) derivation. With the angular convention $a_i\cdot b_j=2\pi\delta_{ij}$, put $G=hb_1+kb_2+lb_3$. Then $G\cdot r=2\pi m$ is the same [plane equation](cartesian-equation-of-a-plane.md) as $hx+ky+lz=m$. Thus $G$ is a [normal vector](normal-vector.md). Moving between consecutive sheets along this normal changes the [dot product](dot-product.md) by $2\pi$, giving

$$
|G|d=2\pi,\qquad d=\frac{2\pi}{|G|}.
$$

For perpendicular cubic axes of length $a$, this becomes

$$
G=\frac{2\pi}{a}(h,k,l),\qquad d_{hkl}=\frac{a}{\sqrt{h^2+k^2+l^2}}.
$$

For example, choose a [primitive cubic lattice](primitive-cubic-lattice.md) with $a=0.600\,\mathrm{nm}$. Its $(210)$ [lattice planes](lattice-plane.md) have $d_{210}=0.600/\sqrt5\simeq0.268328\,\mathrm{nm}$. This is a chosen geometry, not an experimental value. The [distance from a point to a plane](distance-from-a-point-to-a-plane.md) gives the same result: the planes $2X+Y=0$ and $2X+Y=a$ in ordinary Cartesian length coordinates are separated by $a/\sqrt5$.

Specify whether $d_{hkl}$ denotes spacing between successive occupied [lattice planes](lattice-plane.md) or the formal spacing assigned to a reflection label. In a [primitive cubic lattice](primitive-cubic-lattice.md), $(200)$ has formal spacing $a/2$ but every other sheet contains no [lattice points](lattice-point.md); its reflection is the second [diffraction order](diffraction-order.md) of $(100)$. In a [face-centered cubic lattice](face-centered-cubic-lattice.md) with conventional cubic axes, the $(200)$ sheets at half-integer $X/a$ do contain [lattice points](lattice-point.md). Here $a/2$ is the actual spacing of the complete family perpendicular to that cube edge. The [Primitive cubic Bragg peak positions](primitive-cubic-bragg-peak-positions.md) example explains how to avoid counting a reflection twice.

## ↑ Ancestors (5)

1. [Lattice plane](lattice-plane.md)
2. [Crystal structure](crystal-structure.md)
3. [Physical chemistry](physical-chemistry-split.md)
4. [Chemistry](chemistry-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (13)

- [Bragg angle](bragg-angle.md)
- [Bragg crystal reflection experiment of 1913](bragg-crystal-reflection-experiment-of-1913.md)
- [Bragg's law](bragg-s-law.md)
- [Crystal structure](crystal-structure.md)
- [Crystal X-ray spectrometer](crystal-x-ray-spectrometer.md)
- [Gaussian spectral doublet resolution](gaussian-spectral-doublet-resolution.md)
- [Interplanar spacing](interplanar-spacing.md)
- [Lattice constant from two indexed reflections](lattice-constant-from-two-indexed-reflections.md)
- [Neutron diffraction](neutron-diffraction.md)
- [Primitive cubic Bragg peak positions](primitive-cubic-bragg-peak-positions.md)
- [Relative X-ray wavelength calibration](relative-x-ray-wavelength-calibration.md)
- [Two-atom neutron diffraction selection](two-atom-neutron-diffraction-selection.md)
- [X-ray crystallographic structure inference](x-ray-crystallographic-structure-inference.md)
