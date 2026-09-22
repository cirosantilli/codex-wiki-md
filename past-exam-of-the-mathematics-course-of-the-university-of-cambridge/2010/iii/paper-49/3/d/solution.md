<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use [phase-flip protection by Hadamard conjugation](../../../../../../phase-flip-protection-by-hadamard-conjugation.md). Insert a [Hadamard gate](../../../../../../hadamard-gate.md) on each of the three data wires immediately after the two encoding CNOTs and before the physical error. Insert another Hadamard on each data wire immediately after the error and before syndrome detection. Leave the two syndrome ancillas and every detection, recovery and decoding gate unchanged.

The first layer changes the encoded state to $\alpha|+++\rangle+\beta|---\rangle$, the three-qubit [phase-flip repetition code](../../../../../../phase-flip-repetition-code.md). The two layers surrounding the error turn the effective error seen by the old circuit into

$$
E'=H^{\otimes3}EH^{\otimes3}.
$$

Since $H^2=I$ and $HZH=X$, the four physical cases become respectively $I,X_1,X_2,X_3$. The original coherent syndrome and recovery circuit corrects all four, as its syndrome table shows. Thus **two Hadamard layers on the three data wires, straddling the error, give the required phase-flip protection**. The final top wire is the original $|\psi\rangle$, not $H|\psi\rangle$, because the second layer returns the data to the original coding basis before recovery and decoding.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 49](../../../paper-49-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
