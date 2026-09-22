<h1 id="5/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Three defensible approaches are:

- Use simultaneous calibration, for example [Bonferroni correction](../../../../../../bonferroni-correction.md): give each of eight hospitals outside [probability](../../../../../../probability.md) at most $0.05/8$. Replace 1.96 by $z_{1-0.05/16}\approx2.7344$ in the normal bands, giving familywise error at most 5% when the marginal tests are calibrated.
- Apply the [Holm step-down procedure](../../../../../../holm-bonferroni-method.md) to valid two-sided binomial p-values. Order them and compare the jth smallest with $0.05/(9-j)$ until the first nonrejection. This controls familywise error while often being less conservative than giving every hospital the same Bonferroni threshold.
- Treat an initial signal as a screen and require prespecified confirmation in independent new data before declaring a persistent deviation, alongside checking case mix and coding. Calibration must include both stages; unrestricted repeated testing until an alarm appears would increase, rather than solve, the problem.

**A control-limit crossing prompts investigation; it is not itself a verdict on a hospital.** Wider or adjusted thresholds also reduce sensitivity, so the false-alarm objective and the cost of missed genuine problems should be made explicit.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [5](../../5.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
