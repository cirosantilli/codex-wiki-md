<h1 id="b5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Starting with the [identity matrix](../../../../../identity-matrix.md), multiply by $M$ once per iteration and test the resulting power. Using integer objects keeps the calculation exact and avoids fixed-width integer overflow accidentally turning a nonzero power into zero:

```
def kzero(matrix,kmax=100):
    a=np.asarray(matrix,dtype=object)
    if a.ndim!=2 or a.shape[0]!=a.shape[1]:raise ValueError('square matrix required')
    power=np.eye(len(a),dtype=object)
    for k in range(1,kmax+1):
        power=power@a
        if np.equal(power,0).all():return k
    return None

print([kzero(rand_triu(10)) for _ in range(5)])
```

Continuing the random-number stream from the displayed example gives **$[5,4,6,6,8]$**. These are the least positive zero powers, rather than the number of nonzero powers; in particular, a zero matrix has [nilpotency index](../../../../../nilpotency-index.md) one.

For a [strictly upper triangular matrix](../../../../../strictly-upper-triangular-matrix.md), a nonzero entry of $M^k$ can only lie at least $k$ positions above the diagonal. Thus $M^n=0$, and every one of these $10\times10$ examples must return an integer at most ten. The code interprets “up to” as including `kmax`; if the final strict inequality in the question is intended instead, replace `range(1,kmax+1)` by `range(1,kmax)`.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [B5](../../b5.md)
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
