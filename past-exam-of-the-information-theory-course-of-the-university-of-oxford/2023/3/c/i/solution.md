<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $0\leq q<1$, use [repeat-until-success coding over an erasure channel](../../../../../repeat-until-success-coding-over-an-erasure-channel.md): **delete every erasure symbol from the received sequence and retain the non-erased bits in order**. Each message [bit](../../../../../bit.md) contributes a string of erasures followed by exactly one correct non-erased copy. The [channel encoder](../../../../../channel-encoder.md) advances to the next [bit](../../../../../bit.md) only after this successful copy, so the retained [bits](../../../../../bit.md) are precisely $W_1,\ldots,W_n$. Hence

$$
\boxed{d(Y)=W,\qquad\Pr(d(Y)\ne W)=0.}
$$

Indeed, $\Pr(M_j>k)=q^k\to0$, so each stage and the finite collection of $n$ stages terminate [almost surely](../../../../../almost-sure-convergence.md). The protocol uses [channel feedback](../../../../../channel-feedback.md): Alice must know whether an erasure occurred before deciding whether to repeat. This feedback is implicit in the stated algorithm and is not counted as a forward [channel](../../../../../communication-channel.md) use.

At $q=1$, no stage ever finishes, so there is **no terminating zero-error decoder for arbitrary messages**. This endpoint is excluded from the operational claim above.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the information theory course of the University of Oxford](../../../../split.md)
6. [Information theory course of the University of Oxford](../../../../../information-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
