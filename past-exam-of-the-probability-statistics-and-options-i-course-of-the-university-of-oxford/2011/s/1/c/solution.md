<h1 id="s/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $r=1-\pi/4$ be the rejection probability. The [rejected-proposal distribution](../../../../../rejected-proposal-distribution.md) has density

$$
g_R(v)=\frac{q(v)(1-\sqrt{1-v^2})}{r}
=\frac{1-\sqrt{1-v^2}}{2r},\qquad -1<v<1.
$$

If any of the first $n$ trials accepts, the returned value has target density $f$. If all $n$ reject, which has probability $r^n$, the forced return is the final rejected proposal and has density $g_R$. Thus the capped algorithm has density

$$
\boxed{f_n=(1-r^n)f+r^n g_R.}
$$

It is biased toward the ends of the interval, where rejection is most likely, and has too little mass near the centre. The bias disappears geometrically as the trial cap increases. This is [bias from returning a rejected proposal after a rejection-sampling cap](../../../../../bias-from-returning-a-rejected-proposal-after-a-rejection-sampling-cap.md).

Conditional on acceptance before the $n$th trial, however, **the returned value has exactly the semicircle law**. For each possible first successful trial its value has density $f$, independently of the number of previous failures; a mixture of these identical conditional laws remains $f$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [S](../../../s.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
