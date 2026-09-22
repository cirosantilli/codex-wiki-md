# Binary cross-entropy

↑ **Parent:** [Cross-entropy](cross-entropy.md)

Let $Y$ follow a [Bernoulli distribution](bernoulli-distribution.md) with true event [probability](probability.md) $r$, and let the model report event [probability](probability.md) $q$. The [binary cross-entropy](binary-cross-entropy.md) is its expected [logarithmic loss](logarithmic-loss.md):

$$
H(r,q)=-r\log_2q-(1-r)\log_2(1-q).
$$

For $0<r<1$, it is minimized at $q=r$, where the value is [binary entropy](binary-entropy.md) $h_2(r)$. An individual outcome has loss $-\log_2q$ when $Y=1$ and $-\log_2(1-q)$ when $Y=0$; the [binary cross-entropy](binary-cross-entropy.md) averages those two cases using the true [probabilities](probability.md).

For $r=1/4$, truthful reporting gives $h_2(1/4)\approx0.811278$ [bits](bit.md). Reporting $q=1/2$ gives one [bit](bit.md). Reporting $q=0.01$ gives

$$
H(1/4,0.01)=\tfrac14\log_2 100-\tfrac34\log_2 0.99\approx1.671839\text{ bits}.
$$

Both $q=1/4$ and $q=0.01$ select zero if one predicts only the more likely binary outcome. Their predicted [probabilities](probability.md) are very different, however, and [cross-entropy](cross-entropy.md) reveals the cost of underestimating the event that occurs a quarter of the time. Endpoint losses are computed using the realized outcome rather than multiplying zero by an undefined [logarithm](logarithm.md).

<a id="image-the-expected-logarithmic-loss-is-minimized-by-reporting-the-true-event-probability"></a>
![](binary-cross-entropy-forecast-loss.png)

**[Figure 2](#image-the-expected-logarithmic-loss-is-minimized-by-reporting-the-true-event-probability). The expected logarithmic loss is minimized by reporting the true event probability**. The true [Bernoulli distribution](bernoulli-distribution.md) has parameter $r=1/4$. The blue curve averages the orange event loss and gray nonevent loss with weights $1/4$ and $3/4$. Its minimum is at $q=r$, while both endpoint limits diverge because both outcomes have positive [probability](probability.md). These are calculated expectations, rather than measurements.

## ↑ Ancestors (7)

1. [Cross-entropy](cross-entropy.md)
2. [Information entropy](information-entropy-split.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Binary cross-entropy](binary-cross-entropy.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/15/c/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-3/section-f/47/b/solution.md)
