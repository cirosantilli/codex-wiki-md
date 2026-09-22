# Gas electron diffraction

↑ **Parent:** [Molecular geometry](molecular-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gas_electron_diffraction)

[Gas electron diffraction](gas-electron-diffraction.md) infers [molecular geometry](molecular-geometry.md) from the [diffraction](diffraction.md) of [electrons](electron.md) by a gaseous sample. It makes a useful experimental test of shape: distances between both bonded and nonbonded [atomic nuclei](atomic-nucleus-split.md) affect the signal, so a proposed straight arrangement and a bent arrangement can be distinguished through their pair separations.

A concrete modern apparatus is the Bielefeld instrument described by [Reuter, Vishnevskiy, Blomeyer and Mitzel (2016), Gas electron diffraction of increased performance, §§1, 3 and 12](https://doi.org/10.1515/znb-2015-0186). A hot cathode supplies [electrons](electron.md); apertures and magnetic lenses shape the beam. A temperature-controlled nozzle injects sample vapour across it inside a [vacuum](vacuum.md) chamber. Pumps and a cold trap reduce unwanted residual gas. A central beam stop catches the strong unscattered beam; off-axis scattered [electrons](electron.md) expose imaging plates. A rotating sector can attenuate the intense small-angle region to accommodate detector range. The authors checked both the spatial scale of the plate scanner and its response to electron dose. These checks matter because an error in detector position or intensity calibration can masquerade as a structural difference.

<a id="image-molecular-geometry-electron-diffraction"></a>
![](molecular-geometry-electron-diffraction.png)

**[Figure 12](#image-molecular-geometry-electron-diffraction). Gas electron diffraction: apparatus, pair-distance inference, and a bond angle**. Original schematic, not an engineering drawing or a recorded [diffraction](diffraction.md) pattern. Rays identify possible incident and scattered paths; the detector is deliberately shown without invented rings or intensity traces. The lower [triangle](triangle.md) is a normalized rigid-model construction using $104.4776^\circ$; it illustrates a geometric inference, not distances measured in this apparatus.

What is measured is detector signal as a function of position, converted to scattering [angle](angle.md) using the sample-to-detector distance. Randomly oriented [molecules](molecule-split.md) give radial information. After extracting the molecular intensity, compare it with predictions from a candidate arrangement and adjust the [bond lengths](bond-length.md) and [bond angles](bond-angle.md) to improve the fit. The [Wann Electron Diffraction Group's account of time-averaged GED, experiment and theory](https://www.york.ac.uk/chemistry/people/dwann/wanngroup/time-averagedged/) describes radial averaging and this refinement. The apparatus does not photograph one [molecule](molecule-split.md) with labelled [atomic nuclei](atomic-nucleus-split.md).

Why can distances survive random orientation? In a simplified rigid pair model with separation $r$, write $s$ for the magnitude of the difference between incident and scattered [wave vectors](wavevector.md). Averaging the interference factor over uniformly distributed directions gives

$$
\frac12\int_{-1}^{1}\cos(srt)\,dt=\frac{\sin(sr)}{sr},
$$

with limiting value one at $sr=0$. This follows by integrating the [cosine](cosine.md); $t$ is the [cosine](cosine.md) of the angle between the pair and the scattering direction. The [oscillations](oscillation.md) depend on $r$, although the orientation has disappeared. A real calculation weights many pairs by their [scattering amplitudes](scattering-amplitude.md) and includes nuclear motion. The [wave interference](interference-wave-propagation.md) explanation and superposed pair-distance contributions are discussed in the same [Wann group theory account](https://www.york.ac.uk/chemistry/people/dwann/wanngroup/time-averagedged/).

Once a consistent structural model supplies two equal [bond lengths](bond-length.md) $b$ and an outer-atom separation $d$, the [law of cosines](law-of-cosines.md) converts these to a [bond angle](bond-angle.md). For example, the illustrative $d/b=1.5811$ corresponds to approximately $104.5^\circ$, while $d/b=2$ is straight. This geometric step explains what a shape measurement is trying to establish; it is not a new [water](water.md) measurement.

There are two essential limits. First, recovering labelled three-dimensional positions from a summed radial signal is an [inverse problem](inverse-problem-split.md): composition, candidate connectivity, and other structural information can be needed to distinguish competing fits. Karle's authored review [Structure determination of gaseous and amorphous substances by diffraction methods (1977), abstract](https://pmc.ncbi.nlm.nih.gov/articles/PMC432024/?page=-1) explains why too few independent observations make supplementary structural information indispensable. A good fit alone does not prove that the proposed arrangement is unique. Second, [atomic nuclei](atomic-nucleus-split.md) are moving. Distances inferred by [gas electron diffraction](gas-electron-diffraction.md) are motion-dependent averages; corrections are required before identifying them with a minimum-[potential energy](potential-energy.md) arrangement. For experimental distance conventions, see the [IUPAC Gold Book: bond length](https://goldbook.iupac.org/terms/view/BT07003). These limitations explain why model assumptions and the averaging convention must accompany a precise [bond angle](bond-angle.md).

## ↑ Ancestors (4)

1. [Molecular geometry](molecular-geometry.md)
2. [Molecule](molecule-split.md)
3. [Chemistry](chemistry-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Bond angle](bond-angle.md)
- [Gas electron diffraction](gas-electron-diffraction.md)
- [Molecular geometry](molecular-geometry.md)
