<h1 id="27j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The terminal [European put option](../../../../../../european-put-option.md) payoffs are zero at forty-five, thirty-six and sixteen, and five at ten. At the good first node its value is zero. At the bad node its continuation value is $(4/5)[(5/6)0+(1/6)5]=2/3$, below the exercise payoff three, so optimal exercise occurs there. At time zero the continuation value is $(4/5)[(3/8)0+(5/8)3]=\boxed{3/2}$, exceeding the immediate payoff zero.

To hedge one sold [American put option](../../../../../../american-put-option.md), short $1/6$ of a share and put four in the bank at time zero. The portfolio costs $-15/6+4=3/2$, exactly the premium. At time one the bank holds five. After a good move the short position costs five to close, exhausting the portfolio and liability. After a bad move it costs two to close, leaving three for the exercised put. Thus after two bad periods the rational buyer already exercised at time one, and **the hedge pays three and closes then; there is no remaining time-two obligation**. Physical delivery gives the same accounting by immediately selling the stock received on exercise.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [27J](../../27j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
