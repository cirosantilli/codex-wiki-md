# Rotational spectral line assignment

↑ **Parent:** [Rotational spectroscopy](rotational-spectroscopy.md)

A [rotational spectral line assignment](rotational-spectral-line-assignment.md) associates a measured [spectral line](spectral-line.md) with a [molecule](molecule-split.md), an internal [quantum state](quantum-state.md), and an initial and final set of [quantum numbers](quantum-number.md). For the spin-free [linear rigid rotor](linear-rigid-rotor.md), absorption is labelled $J\to J+1$. A regularly spaced group suggests a candidate [rotational constant](rotational-constant.md), but the lowest line inside a scanned band need not be $0\to1$. Several [molecules](molecule-split.md) can contribute to the same spectrum, and an apparent missing member can lie outside the band or below the detection threshold.

First determine line centers and their uncertainties from the instrument's readout, accounting for resolved [Doppler shifts](doppler-effect.md) or [hyperfine structure](hyperfine-structure.md) rather than treating every peak as a separate rotational transition. Then propose integer assignments, fit a rotational [Hamiltonian](hamiltonian.md), and predict additional [spectral lines](spectral-line.md). For a weakly distorted [linear molecule](linear-molecule.md) within one vibrational [quantum state](quantum-state.md), the [centrifugal distortion](centrifugal-distortion.md) model gives the useful diagnostic

$$
\nu_m=2Bm-4Dm^3,\qquad
\frac{\nu_m}{2m}=B-2Dm^2,\qquad m=J+1.
$$

Here $B,D,\nu_m$ are all [frequencies](frequency.md) in $\mathrm{Hz}$. Correct assignments make the second expression a [straight line](straight-line.md) against $m^2$, with intercept $B$ and slope $-2D$. This follows by division of the transition formula; no additional model of [molecular geometry](molecular-geometry.md) is required. A direct [weighted least squares](weighted-least-squares.md) fit of $\nu_m$ to $2Bm-4Dm^3$ uses the measured uncertainties. If instead the transformed values are fitted, their uncertainties must also be divided by $2m$.[§2a, equation (7): rotational transition frequencies with centrifugal distortion](diatomic-spectral-database-by-national-institute-of-standards-and-technology/1-sigma-ground-state-molecules.md)

For an original example, stipulate $B=5.000000\,\mathrm{GHz}$ and $D=2.000\,\mathrm{kHz}$, and suppose a scan covers $38$–$72\,\mathrm{GHz}$. The model places four consecutive transitions at $39.999488$, $49.999000$, $59.998272$, and $69.997256\,\mathrm{GHz}$. Their assignments are $m=4,5,6,7$, hence $J=3,4,5,6$. An extra stipulated line at $53.2\,\mathrm{GHz}$ is unrelated to this series. All these [frequencies](frequency.md) are calculated example inputs, not measured OCS data.

At $m=4$ and $m=7$, the transformed values are $4999.936$ and $4999.804\,\mathrm{MHz}$. Their [straight line](straight-line.md) has slope $(4999.804-4999.936)/(49-16)=-0.004\,\mathrm{MHz}$, recovering $D=0.002\,\mathrm{MHz}$ and $B=5000\,\mathrm{MHz}$. Both intermediate transitions satisfy the same line exactly. Merely relabelling the first visible transition $0\to1$ fails this diagnostic. The model predicts a withheld $7\to8$ transition at $79.995904\,\mathrm{GHz}$: an additional measurement there would test the assignment rather than merely refit the original four lines.

<a id="image-rotational-line-assignment-and-thermal-response"></a>
![](rotational-line-assignment-and-thermal-response.png)

**[Figure 5](#image-rotational-line-assignment-and-thermal-response). Original synthetic rotational spectral line assignment, fit diagnostic, and rotational state populations**. Stipulated values, not measured data. Upper panels use $B=5\,\mathrm{GHz}$ and $D=2\,\mathrm{kHz}$; stick heights show positions only. Lower panels independently use the [linear rigid rotor](linear-rigid-rotor.md) with the same $B$, $D=0$, and [temperatures](temperature-split.md) $3$ and $30\,\mathrm K$. [Rotational state populations](rotational-state-populations.md) and ideal integrated absorption areas are different quantities; each absorption curve is normalized separately. Neither is a predicted pulsed [FTMW spectroscopy](fourier-transform-microwave-spectroscopy.md) peak amplitude.

An assignment earns confidence when several independently observed [spectral lines](spectral-line.md), including lines outside the fitted interval, agree within uncertainty and expected strong accessible lines are present. Inspect the [residual of an inverse problem](residual-of-an-inverse-problem.md) for each line against $J$: systematic curvature can signal inadequate [centrifugal distortion](centrifugal-distortion.md), whereas isolated discrepancies suggest a blend or wrong assignment. Comparing a known sample, a blank, and an [isotope shift of a linear rotor](isotope-shift-of-a-linear-rotor.md) supplies different checks. These are general inference controls; the actual reported controls of the [NIST trace-gas FTMW validation experiment](nist-trace-gas-ftmw-validation-experiment.md) are described separately. One isolated match or one fitted [rotational constant](rotational-constant.md) alone cannot certify molecular identity.

## ↑ Ancestors (5)

1. [Rotational spectroscopy](rotational-spectroscopy.md)
2. [Molecular rotation](molecular-rotation.md)
3. [Molecule](molecule-split.md)
4. [Chemistry](chemistry-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [NIST trace-gas FTMW validation experiment](nist-trace-gas-ftmw-validation-experiment.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2021/paper-1/a3/b/iv/solution.md)
- [Rotational spectral line assignment](rotational-spectral-line-assignment.md)
- [Rotational spectroscopy](rotational-spectroscopy.md)
