<h1 id="n/n2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

During phase A every item is inspected, while during phase B inspection has probability $1/r$, independently of item quality. The long-run inspected fraction is therefore the stationary reward

$$
I=\sum_{i<K}\pi_i+\frac{\pi_K}{r}=1-\left(1-\frac1r\right)\pi_K.
$$

This can be justified by the [Markov chain ergodic theorem](../../../../../../markov-chain-ergodic-theorem.md) for state occupation and the strong law for the independent inspection coins (or the corresponding bounded martingale differences).

For the printed cumulative count this gives

$$
\boxed{I_{\rm cumulative}=\frac{Kp+q}{Kp+rq}}.
$$

It does not equal the claimed expression in general. For instance $K=2$, $p=1/2$, $r=2$ gives $I=3/4$, whereas the printed expression gives $4/5$.

For the consecutive-clearance rule, substituting $\pi_K=rq^K/D$ instead gives

$$
I_{\rm consecutive}=1-\frac{(r-1)q^K}{D}
=\boxed{\frac1{1+(r-1)(1-p)^K}}.
$$

Thus **the claimed formula is valid for consecutive clearance, and false for the literal cumulative count**. For $p=0$ the limiting inspected fraction is $1/r$ in either model; for $p=1$ it is 1 because phase A never clears.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [N2](../../../n2.md)
4. [N](../../../../n.md)
5. [2004](../../../../../2004-split.md)
6. [Past exam of the options II course of the University of Oxford](../../../../../split.md)
7. [Options II course of the University of Oxford](../../../../../../options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
