# Parallax localization of a virtual image

↑ **Parent:** [Virtual image](virtual-image.md)

[Parallax localization of a virtual image](parallax-localization-of-a-virtual-image.md) matches the apparent depth of a [virtual image](virtual-image.md) to a directly viewed physical marker. A sideways change of viewpoint changes their relative apparent positions if their depths differ. Adjust the marker until that relative motion vanishes, and use its coordinate to estimate image position. The marker must be viewed directly; viewing it through the same [optical lens](lens-optics.md) compares two images rather than an image and a known physical depth. [Orhan Aytür, Bilkent University, Experiment 2, §2: Pencil parallax test](https://www.ee.bilkent.edu.tr/~ee428/manual/html/node6.html).

For two nearly aligned points at distances $L_i,L_m$ from an eye displaced sideways by $\delta$, the [small-angle approximation](small-angle-approximation.md) gives a change of relative viewing [angle](angle.md) proportional to $\delta(1/L_i-1/L_m)$. It vanishes when $L_i=L_m$, and changes sign across that match. When both distances are large, the difference is small, explaining the poor depth precision near the [thin lens](thin-lens.md) condition $u=f$.

## ↑ Ancestors (6)

1. [Virtual image](virtual-image.md)
2. [Image formation](image-formation.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Parallax localization of a virtual image](parallax-localization-of-a-virtual-image.md)
- [Virtual image](virtual-image.md)
