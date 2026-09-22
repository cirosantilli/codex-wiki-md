<h1 id="c9/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take $\mu$ to be the total instantaneous [mutation rate](../../../../../mutation-rate.md) away from a base, so each specified alternative has rate $\mu/3$. Under the [Jukes-Cantor model](../../../../../jukes-cantor-model.md), the uniform component is stationary and the three contrast components decay as $e^{-4\mu t/3}$, giving

$$
P_{ab}(t)=\begin{cases}
\frac14+\frac34e^{-4\mu t/3},&a=b,\\
\frac14(1-e^{-4\mu t/3}),&a\ne b.
\end{cases}
$$

An implementation is:

```
def jukes(a, b, t, mu):
    decay = np.exp(-4*mu*t/3)
    return .25 + .75*decay if a == b else .25*(1-decay)

print(f"{jukes(2,2,1,.5):.3f} {jukes(2,3,1,.5):.3f}")
```

**The two probabilities are $0.635$ and $0.122$.** The probabilities in any row sum to one, at $t=0$ the [transition matrix](../../../../../stochastic-matrix.md) is the identity, and at long times every entry tends to $1/4$.

The [Jukes-Cantor model](../../../../../jukes-cantor-model.md) is also parameterized by a rate $q$ for each specified replacement, in which case the exponential is $e^{-4qt}$ and $\mu=3q$. The total-rate convention is used consistently below; it yields an optimum within the stated search interval, whereas the corresponding per-replacement rate is about $0.0522$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [C9](../../c9.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
