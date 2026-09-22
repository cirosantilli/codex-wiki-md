<h1 id="b/6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

At expiry, the difference of a European call and put with matching strike is $(S_T-K)^+-(K-S_T)^+=S_T-K$. Linearity of pricing therefore makes their difference equal the forward-contract value from part (c):

$$
\boxed{C(t,S)-P(t,S)=S+\frac\delta r(1-e^{-r(T-t)})-Ke^{-r(T-t)}.}
$$

A direct [put-call parity](../../../../../put-call-parity.md) replication gives the same result. Buy one unit of the commodity and deposit $\delta\int_t^T e^{-r(u-t)}du$ in the bank. Withdraw the fixed cash storage payments from this reserve; the reserve is exhausted at expiry, leaving one commodity unit. Its initial cost is $S+\delta(1-e^{-r\tau})/r$. Borrow $Ke^{-r\tau}$ as well, leaving terminal value $S_T-K$. The law of one price proves the parity identity. If $r=0$, replace the storage reserve by $\delta\tau$.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
