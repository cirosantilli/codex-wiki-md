<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the four conventional [face-centered cubic lattice](../../../../face-centered-cubic-lattice.md) sites $000$, $0\frac12\frac12$, $\frac120\frac12$ and $\frac12\frac120$, their centering factor is

$$
F_{\rm fcc}=1+(-1)^{k+l}+(-1)^{h+l}+(-1)^{h+k}
=\begin{cases}4,&h,k,l\text{ all even or all odd},\\0,&\text{mixed parity}.\end{cases}
$$

This is the [face-centred cubic selection rule](../../../../face-centred-cubic-selection-rule.md). Enumerating the nonzero representatives with $h^2+k^2+l^2\le16$ gives

$$
\begin{array}{c|rrrrrr}
(hkl)&111&200&220&311&222&400\\\hline
h^2+k^2+l^2&3&4&8&11&12&16
\end{array}
$$

Symmetry-related permutations and signs belong to the same powder ring, not additional rings. For Al, the basis contains one atom, $S=F_{\rm fcc}f_{\rm Al}$. Thus

$$
\boxed{\mathrm{Al}:\quad111,\ 200,\ 220,\ 311,\ 222,\ 400}.
$$

For the stated KCl basis,

$$
S_{\rm KCl}=F_{\rm fcc}[f_K+(-1)^hf_{\rm Cl}].
$$

The all-even reflections add the two atomic factors; all-odd reflections subtract them. Ionic $K^+$ and $Cl^-$ each have 18 [electrons](../../../../electron.md), giving similar X-ray amplitudes. Their difference is much smaller than their sum, so the 111 and 311 rings are weak. Consequently the four strong rings are

$$
\boxed{\mathrm{KCl}:\quad200,\ 220,\ 222,\ 400}.
$$

This is an [accidental diffraction extinction from equal atomic scattering factors](../../../../accidental-diffraction-extinction-from-equal-atomic-scattering-factors.md) in the equal-factor limit, not an extra exact fcc selection rule. Isoelectronic ions can have different radial [electron](../../../../electron.md) distributions, so real odd reflections need not vanish exactly. Even the cruder neutral-atom estimate $f_K\simeq19$, $f_{\rm Cl}\simeq17$ makes the odd/even basis-intensity ratio only $(2/36)^2\simeq0.0031$, before other ring-intensity factors.

For Si's displaced identical basis atoms,

$$
S_{\rm Si}=F_{\rm fcc}f_{\rm Si}\left[1+e^{i\pi(h+k+l)/2}\right].
$$

For all-odd indices, the bracket is $1\pm i$, with squared magnitude 2. For all-even indices it vanishes when $h+k+l=2\pmod4$, and has squared magnitude 4 when the sum is a multiple of four. Thus 200 and 222 vanish, whereas 111, 220, 311 and 400 survive:

$$
\boxed{\mathrm{Si}:\quad111,\ 220,\ 311,\ 400}.
$$

These are the basis extinctions of the ideal [diamond cubic structure](../../../../diamond-cubic-structure.md). Intensity strengths within each surviving set can still differ because of atomic factors, multiplicity and geometry.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
