<h1 id="a/3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $T$ be the first completion time of the word. A fresh gambler arrives before every throw with capital one, betting it all on the successive symbols $1,2,1,2$. Each correct bet multiplies capital by six and each wrong bet loses it, so every bet is fair. A gambler who completes the word keeps the winnings.

At time $T$, the gambler who bet on all four final throws has capital $6^4$. The gambler who bet on the final two throws has correctly matched the suffix $12$ and has capital $6^2$. There are no other survivors: the only nonempty suffixes of $1212$ that are also prefixes are $12$ and $1212$. Thus the total surviving capital is $6^4+6^2$.

To justify the expectation identity, independent blocks of four throws each have probability $6^{-4}$ of equalling the pattern, so $\mathbb P(T>4k)\leq(1-6^{-4})^k$ and $\mathbb ET<\infty$. Total gambling capital minus the number of arriving unit stakes is a martingale with bounded increments before $T$. [Optional stopping](../../../../../optional-sampling-theorem-for-a-supermartingale.md) therefore equates expected terminal capital with expected total stakes:

$$
\boxed{\mathbb ET=6^4+6^2=1332.}
$$

This is the [waiting time for a word in independent uniform symbols](../../../../../waiting-time-for-a-word-in-independent-uniform-symbols.md). The extra $6^2$ reflects the overlapping occurrence of the prefix $12$ at the word's end.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
