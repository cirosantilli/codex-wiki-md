# Western blot normalization

↑ **Parent:** [Western blot](western-blot.md)

Total-[protein](protein.md) [Western blot normalization](western-blot-normalization.md) compares a target-band signal with a signal representing many transferred [proteins](protein.md) in that lane. It is distinct from measuring one reference [protein](protein.md), and from measuring the target itself. Its denominator is a loading proxy: normalization estimates target abundance relative to detected total [protein](protein.md), rather than target amount per [biological cell](biological-cell.md). Different sample compositions, selective [Western blot transfer](western-blot-transfer.md) losses or unequal stain responses can still matter.

For an original calculation, suppose background-corrected target signals $I_A=12$, $I_B=24$ and total-[protein](protein.md) signals $P_A=30$, $P_B=60$ are in their respective proportional response ranges. Then

$$
\frac{I_B/P_B}{I_A/P_A}=\frac{24/60}{12/30}=1.
$$

The invented signals double together, so this calculation supplies no evidence for a higher target fraction. With $I_B=24$ but $P_B=30$, the same calculation gives $2$. These examples assume a common target response and a common total-[protein](protein.md) response between lanes, negligible remaining background, and comparable target recovery; they do not equate total-[protein](protein.md) staining with target abundance. Multiplying both signals in a lane by the same loading factor cancels in their [ratio](ratio.md); a selective target loss does not cancel.

## ↑ Ancestors (4)

1. [Western blot](western-blot.md)
2. [Protein](protein.md)
3. [Biology](biology-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Receptor phosphorylation assay](receptor-phosphorylation-assay.md)
- [Western blot normalization](western-blot-normalization.md)
- [Western blot response saturation](western-blot-response-saturation.md)
