# Permanganate-iron endpoint and blank model

↑ **Parent:** [Permanganate-iron titration](permanganate-iron-titration.md)

The apparatus and motivating measurement are described in [permanganate-iron titration](permanganate-iron-titration.md); the following is an original account of its possible errors. Assume correct [titrant standardization](titrant-standardization.md), the [acidic permanganate-iron balance](acidic-permanganate-iron-balance.md), quantitative conversion of the sampled $\mathrm{Fe}^{2+}$, and additive contributions expressed as equivalent [titrant](titrant.md) [volumes](volume.md). Write

$$
V=V_{\mathrm{Fe}}+B_s+D_s+A+I,\qquad
V_b=B_b+D_b,\qquad
V_{\mathrm{Fe}}=\frac{n_{\mathrm{Fe}}}{5c}.
$$

Here $V$ is the sample [titre](titre.md), $V_b$ the [titration blank](titration-blank.md), $B_s,B_b$ background reagent consumption, and $D_s,D_b$ signed offsets of the observed [titration endpoints](titration-endpoint.md) from the respective [stoichiometry](stoichiometry.md) conditions after background consumption. The subscripts distinguish sample and blank. $I$ is additional sample-specific [permanganate](permanganate.md) demand, absent from the blank; $A$ is apparent delivery used to fill an initially air-containing [burette](burette.md) tip rather than enter the flask. Assume the blank's tip is already filled; the sample should also have $A=0$ after proper preparation. These terms are a diagnostic model, not measured components of the stipulated $0.10\,\mathrm{mL}$ blank.

<a id="image-burette-delivery-titration-endpoint-and-titration-blank-describe-different-parts-of-the-inference"></a>
![](redox-titration-endpoint-burette-and-blank.png)

**[Figure 10](#image-burette-delivery-titration-endpoint-and-titration-blank-describe-different-parts-of-the-inference). Burette delivery, titration endpoint and titration blank describe different parts of the inference**. Original schematic and additive [volume](volume-thermodynamics.md) model, not a photograph or measured [titration curve](titration-curve.md). The numerical decomposition $12.60=12.50+0.10\,\mathrm{mL}$ assumes matched background and endpoint contributions and no tip-air or sample-specific demand. Boxes are not to scale; the blank's reagent consumption and endpoint offset are not separately specified. The exact [equivalence point](equivalence-point.md) has no guaranteed visible colour flag.

Subtracting the two accounts proves the error relation

$$
\widehat n_{\mathrm{Fe}}=5c(V-V_b)=n_{\mathrm{Fe}}+5c\Delta V,\qquad
\Delta V=(B_s-B_b)+(D_s-D_b)+A+I.
$$

The simple inference is valid when this residual is negligible. Matching [water](water.md) and [sulfuric acid](sulfuric-acid.md) tests the background terms, but does not by itself establish $D_s=D_b$: flask composition and viewing conditions can differ. A coloured sample can mask residual [permanganate](permanganate.md), changing the assigned [titration endpoint](titration-endpoint.md) without a corresponding [redox](redox.md) consumption. A sample-specific [reducing agent](reducing-agent.md) instead contributes positive $I$ by consuming [permanganate](permanganate.md). A reagent [titration blank](titration-blank.md) cannot measure either effect just by omitting the sample.

A transient purple streak before mixing is not the mixed-flask [titration endpoint](titration-endpoint.md). Conversely, the [equivalence point](equivalence-point.md) is the five-to-one inventory match, without a promised visible flag. In the ideal selective model, a persistent excess colour requires some [permanganate](permanganate.md) beyond that match. No particular drop size, waiting time or endpoint offset is stipulated here; the same stated colour criterion must be applied to sample and blank, and its transferability checked.

The model also predicts error direction. If a tip bubble disappears during sample delivery, $A>0$ makes the inferred [amount of substance](amount-of-substance.md) too high because final minus initial [burette](burette.md) reading includes liquid that stayed in the tip. Conditioning the tip before the first reading prevents this particular discrepancy; subtracting a separate [titration blank](titration-blank.md) is not an instrument repair. Repeated [aliquots](aliquot.md) test scatter, a known added $\mathrm{Fe}^{2+}$ inventory tests the five-to-one response, and an independent [titrant standardization](titrant-standardization.md) tests $c$. These are the proposed controls from [permanganate-iron titration](permanganate-iron-titration.md), with distinct diagnostic roles; none alone proves absence of all sample interference.

## ↑ Ancestors (6)

1. [Permanganate-iron titration](permanganate-iron-titration.md)
2. [Redox titration](redox-titration.md)
3. [Redox](redox.md)
4. [Chemical reaction](chemical-reaction-split.md)
5. [Chemistry](chemistry-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Redox titration](redox-titration.md)
