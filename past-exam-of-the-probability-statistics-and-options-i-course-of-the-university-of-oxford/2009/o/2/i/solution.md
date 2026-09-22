<h1 id="o/2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

With immediate replacement and uniform mixing, each capture is a Bernoulli trial with tagged probability $p=k/N$. Counting failures before the $r$th tagged capture gives the stated [negative binomial distribution](../../../../../negative-binomial-distribution.md). Independent runs on the successive days give the sample model.

Writing $S=\sum_i x_i$, the log-[likelihood](../../../../../likelihood-function.md) is $\ell(p)=nr\log p+S\log(1-p)+\text{constant}$. Its derivative vanishes at

$$
\boxed{\widehat p=\frac{nr}{nr+S}=\frac r{r+\overline x}.}
$$

The second derivative is negative. If $S=0$, this formula gives the boundary maximum $p=1$; on the strict physical parameter space $p<1$, it is a supremum rather than an attained interior maximum.

Using the supplied negative-binomial [mean](../../../../../expected-value-split.md), $\mathbb ES=nr(1-p)/p$. Thus total [Fisher information](../../../../../fisher-information-matrix.md) for the sample is

$$
\boxed{I_n(p)=-\mathbb E\ell''(p)=\frac{nr}{p^2}+\frac{nr}{p(1-p)}=\frac{nr}{p^2(1-p)}.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [2](../../2.md)
3. [O](../../../o.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
