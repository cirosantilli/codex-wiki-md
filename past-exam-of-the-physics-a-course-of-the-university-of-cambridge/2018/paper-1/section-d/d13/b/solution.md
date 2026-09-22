<h1 id="section-d/d13/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [systematic error](../../../../../../systematic-error.md) is a reproducible bias in the measurement model or procedure, such as a zero offset, incorrect gain, background contamination, misalignment, loading or temperature-dependent calibration. Repeating the same biased procedure more often reduces independent random scatter but does not remove the bias. An unknown correction also has a [measurement uncertainty](../../../../../../measurement-uncertainty.md), even when the mechanism is systematic.

A simple instrument model is $y=(1+g)x+a+d(t)+\epsilon$, with gain error $g$, offset $a$, drift $d(t)$ and random [noise](../../../../../../noise-signal-processing.md) $\epsilon$. Comparison with calibrated standards at several input values separates an offset from a scale error and can test nonlinearity. Use standards that cover the operating range, verify units and reference values, and propagate uncertainty in the standards into the corrected result. Calibration changes the model; it does not make the corrected measurement exact.

A blank or source-off measurement estimates additive background. For independent source-plus-background count $K_s$ in time $t_s$ and background count $K_b$ in time $t_b$, the net-rate estimate and its counting [variance](../../../../../../variance-split.md) are

$$
\widehat S=\frac{K_s}{t_s}-\frac{K_b}{t_b},\qquad \operatorname{Var}(\widehat S)\simeq\frac{K_s}{t_s^2}+\frac{K_b}{t_b^2}.
$$

Subtracting a measured background removes its estimated mean, not its fluctuations or its uncertainty. A long background exposure can reduce the latter, while drifting backgrounds require monitoring or a joint model.

Reversal can distinguish a wanted signal from an unchanged offset. For example, $V(+I)=IR+V_{\mathrm{th}}$ and $V(-I)=-IR+V_{\mathrm{th}}$ give $R=[V(+I)-V(-I)]/(2I)$ when the thermoelectric offset is stable between readings. Interchanging sample and reference, reversing field direction or reversing an apparatus orientation can similarly expose sign-dependent biases, but only if the wanted and unwanted contributions transform differently.

Track slow [instrumental drift](../../../../../../instrumental-drift.md) using frequent references, interleaved readings or an [ABBA measurement sequence](../../../../../../abba-measurement-sequence.md). Equal-time readings in the order A, B, B, A cancel a common linear drift in the difference estimator $(y_1+y_2-y_0-y_3)/2$. Nonlinear drift or unequal sample conditions can survive. Randomizing run order helps prevent a time drift from imitating dependence on a controlled experimental variable.

Control physical couplings directly: stabilize [temperature](../../../../../../temperature-split.md), minimize gradients, shield unwanted fields, align geometry, and use high [input impedance](../../../../../../input-impedance.md) when loading is the concern. Differential and bridge measurements suppress common changes when their channels are well matched. Varying an apparatus parameter or using an independent method can reveal an unsuspected bias. Report residual corrections, their uncertainties and correlations; adding more identical readings cannot justify discarding a shared calibration uncertainty.

## ↑ Ancestors (15)

1. [B](../b.md)
2. [D13](../../d13.md)
3. [Section D](../../../section-d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
