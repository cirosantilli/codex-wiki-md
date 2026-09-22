<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [channel capacity](../../../../../channel-capacity.md) is the supremum of reliable communication rates: a rate $R$ bits per use is achievable if block encoders and decoders using $n$ channel uses can transmit $M_n$ messages with error [probability](../../../../../probability.md) tending to zero and $\liminf n^{-1}\log_2M_n\ge R$.

A [discrete memoryless channel](../../../../../discrete-memoryless-channel.md) has fixed transition [probabilities](../../../../../probability.md) $W(y|x)$ on finite input and output alphabets, and

$$
W(y_1,\ldots,y_n|x_1,\ldots,x_n)=\prod_{j=1}^nW(y_j|x_j).
$$

Its single-letter capacity formula is

$$
\boxed{C=\max_{P_X}I(X;Y)=\max_{P_X}\bigl(H(Y)-H(Y|X)\bigr),}
$$

with [logarithms](../../../../../logarithm.md) to base two. The [Shannon second coding theorem](../../../../../noisy-channel-coding-theorem.md) identifies this maximum with the operational reliable rate.

For the [binary erasure channel](../../../../../binary-erasure-channel.md), use output symbols $0,1,e$, where $e$ is a recognizable erasure flag. Given input $x$, the output is $x$ with [probability](../../../../../probability.md) $1-p$ and $e$ with [probability](../../../../../probability.md) $p$. If $\Pr(X=1)=a$, the output [probabilities](../../../../../probability.md) are $(1-p)(1-a),(1-p)a,p$. Thus, writing $h_2$ for [binary entropy](../../../../../binary-entropy.md),

$$
H(Y)=h_2(p)+(1-p)h_2(a),\qquad H(Y|X)=h_2(p),
$$

and $I(X;Y)=(1-p)h_2(a)$. Its maximum is attained by the uniform input $a=1/2$, giving

$$
\boxed{C=1-p\text{ bits per channel use},\qquad0\le p\le1.}
$$

In particular the noiseless and complete-erasure endpoints have capacities one and zero. The erasure flag reveals which positions were lost; it does not reveal the erased input values.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
