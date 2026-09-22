<h1 id="6/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

At any division step $u=qv+r$, an [integer](../../../../../../../integer-split.md) divides both $u,v$ exactly when it divides both $v,r$: one direction uses $r=u-qv$, and the other uses $u=qv+r$. Hence

$$
\gcd(u,v)=\gcd(v,r).
$$

Starting with $r_0=a$, $r_1=b$, the [Euclidean division](../../../../../../../euclidean-division.md) produces

$$
r_{j-1}=q_jr_j+r_{j+1},\qquad 0\le r_{j+1}<r_j.
$$

The nonzero [remainders](../../../../../../../remainder.md) form a strictly decreasing sequence of positive [integers](../../../../../../../integer-split.md). Such a sequence must terminate, since there are only finitely many positive [integers](../../../../../../../integer-split.md) below $b$. Suppose $r_N$ is the last nonzero [remainder](../../../../../../../remainder.md), so $r_{N+1}=0$. The unchanged [greatest common divisor](../../../../../../../greatest-common-divisor.md) at each step gives

$$
\boxed{\gcd(a,b)=\gcd(r_1,r_2)=\cdots=\gcd(r_N,0)=r_N.}
$$

The final equality holds because the positive common [divisors](../../../../../../../divisor.md) of $r_N$ and $0$ are precisely the positive [divisors](../../../../../../../divisor.md) of $r_N$. This proves both termination and correctness of the [Euclidean algorithm](../../../../../../../euclidean-algorithm.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [Mathematics IV](../../../../mathematics-iv-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
