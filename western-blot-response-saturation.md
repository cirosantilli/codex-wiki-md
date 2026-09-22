# Western blot response saturation

↑ **Parent:** [Western blot](western-blot.md)

[Western blot response saturation](western-blot-response-saturation.md) means that increasing target amount no longer increases the recorded signal proportionally. It can arise before imaging, through limited binding or reagent availability, as well as through detector limits. Shortening exposure can address a detector limit without repairing an already unresponsive assay. Test the target and normalization readouts with a dilution series under the actual assay conditions; merely seeing a gray band does not establish a proportional response.

In a 2013 methods experiment, a [biological cell](biological-cell-split.md) extract containing added purified [yeast](yeast.md) [protein](protein-split.md) was separated on gels, transferred with a Trans-Blot Turbo to [polymer](polymer-split.md) membranes, and read with an [enzyme](enzyme-split.md)-linked [secondary antibody](secondary-antibody.md). A ChemiDoc MP imager and film recorded the same dilution-series blots. The target and an abundant reference [protein](protein-split.md) had different usable response ranges; transferred total-[protein](protein-split.md) imaging and the reference bands did not track loading equally well. This demonstrates the need for assay-specific response checks, rather than a universal conversion from darkness to amount. [Taylor, Berkelman, Yadav and Hammond, Materials and Methods; Figures 2–4 and 5–7: transfer apparatus, film/imager comparison and loading normalization](a-defined-methodology-for-reliable-quantification-of-western-blot-data-by-sean-c-taylor-and-others.md)

An illustrative response model separates background $b$, target amount $T$, retained fraction $q$, response scale $S$ and characteristic amount $K$:

$$
I(T)=b+S\frac{qT}{K+qT},\qquad S,K>0,\quad 0<q\leq1.
$$

This is an assumed model, not a fitted [Western blot](western-blot.md) calibration. When $qT\ll K$, $I-b\approx(Sq/K)T$. When $qT\gg K$, $I-b$ approaches $S$. For two otherwise identical lanes, doubling $T$ gives the background-corrected [ratio](ratio.md)

$$
\frac{I(2T)-b}{I(T)-b}=\frac{2(K+qT)}{K+2qT}.
$$

At $qT=K$ the [ratio](ratio.md) is $4/3$, despite a true twofold amount change. Thus [Western blot normalization](western-blot-normalization.md) cannot recover a lost amount difference merely by dividing two saturated readouts.

## ↑ Ancestors (4)

1. [Western blot](western-blot.md)
2. [Protein](protein-split.md)
3. [Biology](biology-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Antibody equilibrium occupancy](antibody-equilibrium-occupancy.md)
- [Receptor phosphorylation assay](receptor-phosphorylation-assay.md)
- [Western blot response saturation](western-blot-response-saturation.md)
