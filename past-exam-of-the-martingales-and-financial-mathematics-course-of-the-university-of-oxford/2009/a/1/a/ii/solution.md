<h1 id="a/1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Fix $\epsilon>0$ and use the [indicator random variables](../../../../../../indicator-random-variable.md) $Y_n=1_{\{|X_n-X|>\epsilon\}}$. [Almost sure convergence](../../../../../../almost-sure-convergence.md) gives $\limsup_nY_n=0$ almost surely, while $0\leq Y_n\leq1$. The [Reverse Fatou lemma](../../../../../../reverse-fatou-lemma.md) states that for random variables bounded above by an integrable random variable,

$$
\limsup_n\mathbb E Y_n\leq\mathbb E(\limsup_nY_n).
$$

It follows that

$$
0\leq\limsup_n\mathbb P(|X_n-X|>\epsilon)\leq0.
$$

Since $\epsilon$ was arbitrary, this proves **convergence in probability**. The integrable upper bound is essential to the application of the [Reverse Fatou lemma](../../../../../../reverse-fatou-lemma.md).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [A](../../../../a.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../../split.md)
7. [Martingales and financial mathematics course of the University of Oxford](../../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
