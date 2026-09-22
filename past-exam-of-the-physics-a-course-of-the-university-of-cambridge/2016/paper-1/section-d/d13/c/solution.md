<h1 id="section-d/d13/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Uniform [signal sampling](../../../../../../signal-sampling.md) at rate $f_s$ multiplies a continuous signal by a time-domain [Dirac comb](../../../../../../dirac-comb.md), giving frequency-domain replicas spaced by $f_s$:

$$
X_s(f)=f_s\sum_{k=-\infty}^{\infty}X(f-kf_s).
$$

If a baseband signal is restricted to $|f|\leq B$ and **$f_s>2B$**, these replicas can be separated by an ideal reconstruction filter. Frequencies differing by integer multiples of $f_s$ have the same sampled phase progression; for real signals they fold into the interval from zero to $f_s/2$. This ambiguity is **[aliasing](../../../../../../aliasing.md)**.

<a id="section-d/d13/c/image-two-different-continuous-cosine-frequencies-produce-the-same-samples-when-one-lies-above-nyquist"></a>
![](../../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2016/paper-1-sampling-alias.png)

**[Figure 8](#section-d/d13/c/image-two-different-continuous-cosine-frequencies-produce-the-same-samples-when-one-lies-above-nyquist). Two different continuous cosine frequencies produce the same samples when one lies above Nyquist**. [Source](paper-1-sampling-alias.py).

For example, $0.8f_s$ and $0.2f_s$ cosines produce identical sample values. Apply an analogue [Anti-aliasing filter](../../../../../../anti-aliasing-filter.md) before digitization and choose enough sample-rate margin for its finite transition band. A digital filter applied afterward cannot distinguish components already folded onto one another. Out-of-band noise also aliases unless filtered. The sample rate sets temporal/spectral coverage; [quantization](../../../../../../quantization-signal-processing.md) resolution sets amplitude precision and is a separate limitation. Bandpass [Signal sampling](../../../../../../signal-sampling.md) has additional conditions beyond the simple baseband rule.[MT-002: spectral replicas, aliases and practical filtering](../../../../../../what-the-nyquist-criterion-means-to-your-sampled-data-system-design-by-walt-kester.md)

## ↑ Ancestors (15)

1. [C](../c.md)
2. [D13](../../d13.md)
3. [Section D](../../../section-d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2016](../../../../split.md)
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
