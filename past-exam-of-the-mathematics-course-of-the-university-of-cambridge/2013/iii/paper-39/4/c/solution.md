<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $v_j$ be the optimal [expected value](../../../../../../expected-value.md) before seeing the next offer when $j$ rounds remain. With one round left the offer must be accepted, so $v_1=1/2$. For $j>1$, observing $x$ gives a choice between $x$ now and the continuation value $v_{j-1}$. [Independence](../../../../../../independent-random-variables.md) of future [uniform distributions](../../../../../../continuous-uniform-distribution.md) makes that continuation value independent of past offers. Thus the [uniform-offer stopping recursion](../../../../../../uniform-offer-stopping-recursion.md) is

$$
v_j=\int_0^1\max(x,v_{j-1})\,dx=\frac{1+v_{j-1}^2}{2}.
$$

It gives $v_2=5/8$ and $v_3=89/128$. The [Snell envelope](../../../../../../snell-envelope.md) rule therefore yields the explicit strategy

$$
\boxed{\begin{array}{c|c}
\text{round}&\text{accept when}\\ \hline
1&\xi_1\ge89/128\\
2&\xi_2\ge5/8\\
3&\xi_3\ge1/2\\
4&\text{always}
\end{array}}
$$

Only rounds actually reached are played. At a threshold the two actions have identical continuation [expected value](../../../../../../expected-value.md); either convention is optimal, and exact equality has probability zero. The optimal expected payout before the first offer is

$$
\boxed{v_4=\frac{1+(89/128)^2}{2}=\frac{24305}{32768}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
