<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Remove the common Grassmann parameter and write the [BRST transformation](../../../../../../brst-symmetry.md) as the odd derivation $s$:

$$
sA_\mu^a=(D_\mu c)^a,
\qquad
sc^a=-\frac g2\epsilon^{abc}c^bc^c,
\qquad
s\bar c^a=B^a,
\qquad
sB^a=0.
$$

The last two equations immediately give $s^2\bar c^a=s^2B^a=0$. Applying $s$ to the ghost and using the graded product rule gives

$$
s^2c^a=\frac{g^2}{4}\epsilon^{abc}
\left(\epsilon^{bde}c^dc^ec^c-\epsilon^{cde}c^bc^dc^e\right)=0.
$$

The cancellation is the [Jacobi identity](../../../../../../jacobi-identity.md) for the $SU(2)$ structure constants together with anticommutation of the ghost fields. For the gauge field, the component calculation is

$$
s^2A_\mu^a=(D_\mu sc)^a
+g\epsilon^{abc}(D_\mu c)^bc^c.
$$

The graded product rule gives

$$
(D_\mu sc)^a=-\frac g2\epsilon^{abc}
\left[(D_\mu c)^bc^c+c^b(D_\mu c)^c\right]
=-g\epsilon^{abc}(D_\mu c)^bc^c,
$$

so the two terms cancel. Thus $s^2$ vanishes on every elementary field.

For two independent Grassmann parameters, $\delta_1=\eta_1s$ and $\delta_2=\eta_2s$ satisfy $\delta_1\delta_2O=\eta_1\eta_2s^2O=0$. Since $s$ obeys the graded Leibniz rule, induction extends $s^2O=0$ from the generators $A,c,\bar c,B$ to every polynomial $O(A,c,\bar c,B)$. Hence the BRST transformations are nilpotent.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 304](../../../paper-304-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
