<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Immediately before measuring $Q_{b0}=i\gamma_b\gamma_0$, the state has definite parity for a bilinear such as $Q_{a0}$ or the restored reference $Q_{N0}$ that anticommutes with $Q_{b0}$. If $Q|\psi\rangle=s|\psi\rangle$ and $\{Q,Q_{b0}\}=0$, then

$$
\langle\psi|Q_{b0}|\psi\rangle
=\langle\psi|Q Q_{b0}Q|\psi\rangle
=-\langle\psi|Q_{b0}|\psi\rangle=0.
$$

Hence

$$
\boxed{\Pr(s_b=\pm1)
=\langle\psi|\Pi_\pm^{(b0)}|\psi\rangle
=\frac12.}
$$

If the undesired value of $s_b$ occurs, perform a reference measurement that projects the ancillary pair back toward its previous parity sector, then measure $Q_{b0}$ again. Alternating these anticommuting parity measurements gives a fresh probability $1/2$ of the desired result on each attempt. This [Forced Majorana parity measurement](../../../../../../forced-majorana-parity-measurement.md) has a geometric waiting time, succeeds almost surely, and does not measure the encoded parity $i\gamma_a\gamma_b$ directly. Apply the same repeat-until-success procedure to each required outcome in $\Pi_+^{(N0)}\Pi_{s_a}^{(a0)}\Pi_{s_b}^{(b0)}$; alternatively, keep arbitrary outcomes and track the known inverse-braid or Pauli-frame correction determined by their signs.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 342](../../../paper-342-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
