<h1 id="section-f/47/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

A [multilayer perceptron](../../../../../../multilayer-perceptron.md) usually connects every input unit of a layer to every output unit. For $n$ inputs and $m$ outputs its dense affine layer has **$nm+m$ parameters**, including biases. A convolutional layer instead applies small local filters with [weight sharing](../../../../../../weight-sharing.md) across positions. A two-dimensional filter of size $k_h\times k_w$, with $C_{\rm in}$ input channels and $C_{\rm out}$ output channels, has **$k_hk_wC_{\rm in}C_{\rm out}+C_{\rm out}$ parameters**. The count does not increase with spatial height and width, although the activation storage and arithmetic do.

Local [receptive fields](../../../../../../receptive-field.md) and repeated layers capture increasingly extended patterns. [translation equivariance](../../../../../../translation-equivariance.md) follows from shared filters under compatible boundary conventions; pooling or global aggregation can help build invariance but a convolution alone is not generally translation-invariant. Flattening a large convolutional output into a dense head can reintroduce many parameters. For an unordered descriptor vector, a convolutional locality assumption must be justified rather than imposed merely because convolutional layers have fewer weights.

## ↑ Ancestors (14)

1. [E](../e.md)
2. [47](../../47.md)
3. [Section F](../../../section-f.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../../chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
