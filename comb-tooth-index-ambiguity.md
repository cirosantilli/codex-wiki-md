# Comb tooth index ambiguity

↑ **Parent:** [Optical frequency measurement with a comb](optical-frequency-measurement-with-a-comb.md)

One [beat](beat.md) magnitude does not tell us the [integer](integer-split.md) $n$. In the example, every proposed optical [frequency](frequency.md) $n(250\,\mathrm{MHz})+50\,\mathrm{MHz}$ produces the same signed [beat](beat.md) with its corresponding tooth. A coarse independent optical measurement can select the [integer](integer-split.md): once the [beat](beat.md) sign is known, an error bound below $f_r/2$ suffices if the candidate is selected by nearest distance.

There is also a useful two-spacing check. Keep the unknown [laser](laser-split.md) and $f_0$ fixed, track the same tooth continuously, and increase $f_r$ by a stipulated $5\,\mathrm{Hz}$. Its [frequency](frequency.md) rises by $10\,\mathrm{MHz}$, so the signed [beat](beat.md) falls from $30$ to $20\,\mathrm{MHz}$. Hence

$$
n=-\frac{\Delta b}{\Delta f_r}=\frac{10{,}000{,}000}{5}=2{,}000{,}000.
$$

This inference fails if the unknown drifts appreciably, the offset changes unnoticed, the [beat](beat.md) sign is lost, or the tracker jumps to another tooth. The assumed tooth motion stays well below half the spacing in this example. If $f_0$ also changes by a measured amount, use $n=-(\Delta b+\Delta f_0)/\Delta f_r$.

For a fixed verified tooth number, the first-order [frequency](frequency.md) error is $\delta f_L=n\delta f_r+\delta f_0+\delta b$. Errors in these readings can be correlated because they share a reference. A small [beat](beat.md) uncertainty therefore does not imply the same absolute optical accuracy: the reference's calibration and the factor $n$ remain in the error budget. A wrong tooth number is a separate discrete error, not a small correction. The beauty of the comb is that two controlled parameters organize millions of optical reference points, while the unknown's position is read electronically.

## ↑ Ancestors (7)

1. [Optical frequency measurement with a comb](optical-frequency-measurement-with-a-comb.md)
2. [Optical frequency comb](optical-frequency-comb.md)
3. [Laser](laser-split.md)
4. [Optics](optics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
