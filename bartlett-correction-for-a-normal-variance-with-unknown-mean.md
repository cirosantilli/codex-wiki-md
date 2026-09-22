# Bartlett correction for a normal variance with unknown mean

↑ **Parent:** [Bartlett correction coefficient](bartlett-correction-coefficient.md)

For a sample of size $n\geq2$ from a [normal distribution](normal-distribution.md) with unknown mean, the null variance [likelihood-ratio test statistic](likelihood-ratio-test-statistic.md) is $W=n[-\log(U/n)+U/n-1]$, where $U\sim\chi^2_{n-1}$. With $V=(U-n)/n$, its expected Taylor terms start with $n[\mathbb EV^2/2-\mathbb EV^3/3+\mathbb EV^4/4]$. Here $\mathbb EV^2=(2n-1)/n^2$, $\mathbb EV^3=(2n-3)/n^3$, and $\mathbb EV^4=(12n^2+4n-15)/n^4$. Higher fixed-order terms contribute only $O(n^{-2})$ under valid termwise asymptotic integration. Thus $\mathbb E_0W=1+11/(6n)+O(n^{-2})$ and $W_B=W/[1+11/(6n)]$.

## ↑ Ancestors (11)

1. [Bartlett correction coefficient](bartlett-correction-coefficient.md)
2. [Bartlett correction](bartlett-correction.md)
3. [Likelihood-ratio test statistic](likelihood-ratio-test-statistic.md)
4. [Likelihood-ratio test](likelihood-ratio-test.md)
5. [Statistical hypothesis test](statistical-hypothesis-test.md)
6. [Statistical modelling](statistical-modelling-split.md)
7. [Statistical model](statistical-model-split.md)
8. [Probability and statistics](probability-and-statistics-split.md)
9. [Area of mathematics](area-of-mathematics.md)
10. [Mathematics](mathematics-split.md)
11. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-41/6/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-44/4/solution.md)
