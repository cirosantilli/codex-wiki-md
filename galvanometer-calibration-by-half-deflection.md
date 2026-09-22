# Galvanometer calibration by half deflection

↑ **Parent:** [Moving-coil galvanometer](moving-coil-galvanometer.md)

NCERT's teaching experiment uses a [moving-coil galvanometer](moving-coil-galvanometer.md), a 0–6 V supply, a 0–10 kΩ series [electrical resistance](electrical-resistance.md) box $R$, a 0–200 Ω parallel [electrical resistance](electrical-resistance.md) box $S$, two switches and a [voltmeter](voltmeter.md). With the parallel path open, close the supply switch and record the pointer deflection. Keep $R$ fixed, close the parallel path, and adjust $S$ until the deflection halves. The guide requests repeated settings, clean tight contacts and constant supply [electromotive force](electromotive-force.md); it introduces high $R$ before energizing to protect the winding. [Experiment 6, printed pp. 53–58: Figure E 6.1, Procedure 1–5, Precautions and Sources of Errors](laboratory-manual-physics-class-xii/experiment-6-resistance-and-figure-of-merit-of-a-galvanometer.md)

Write the winding [electrical resistance](electrical-resistance.md) as $R_g$, the supply [electromotive force](electromotive-force.md) as $E$, and assume negligible supply internal [electrical resistance](electrical-resistance.md). [Ohm's law](ohm-s-law.md) gives the two winding [electric currents](electric-current.md)

$$
I_1=\frac{E}{R+R_g},\qquad I_2=\frac{ES}{R(R_g+S)+R_gS}.
$$

If proportional deflection gives $I_2=I_1/2$, solving yields $R_g=RS/(R-S)$, requiring $R>S$. The shortcut $R_g\simeq S$ requires $R\gg R_g$; closing the parallel path generally changes the total supply [electric current](electric-current.md). For chosen values $R=9900\,\Omega$ and $S=99.0\,\Omega$, the exact result is $R_g=100\,\Omega$, rather than $99\,\Omega$. The manual gives this exact relation and asks how finite supply internal [electrical resistance](electrical-resistance.md) affects it. [Experiment 6, printed pp. 54–55, equations (E 6.2), (E 6.8) and (E 6.9); p. 58, Self Assessment 4](laboratory-manual-physics-class-xii/experiment-6-resistance-and-figure-of-merit-of-a-galvanometer.md)

As an additional calibration control, record the supply-off zero, apply several small positive and negative [electric currents](electric-current.md), and recheck zero after each sequence. With $R_g$ known, calculate each [electric current](electric-current.md) from the measured supply [electric potential difference](electric-potential-difference.md) and the total series [electrical resistance](electrical-resistance.md); plot settled deflection against that [electric current](electric-current.md). Equal-magnitude reversed readings should lie equally far from a stable zero. A fitted relation $\theta_{\mathrm{read}}=\theta_0+S_I I$ separates zero offset from [galvanometer current sensitivity](galvanometer-current-sensitivity.md). The manual's “figure of merit” is [electric current](electric-current.md) per scale division, not the mechanical [torsional spring constant](torsion-constant.md) $k$ used above. These reversal and zero checks extend the documented procedure; they are proposed controls, not reported measurements.

## ↑ Ancestors (8)

1. [Moving-coil galvanometer](moving-coil-galvanometer.md)
2. [Galvanometer](galvanometer.md)
3. [Electric current](electric-current.md)
4. [Electric charge](electric-charge-split.md)
5. [Electromagnetism](electromagnetism-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
