# Finite observations do not certify Richardson extrapolation accuracy

↑ **Parent:** [Richardson extrapolation](richardson-extrapolation.md)

[Richardson extrapolation](richardson-extrapolation.md) cancels a specified leading term in an [asymptotic expansion](asymptotic-expansion-split.md), but an unquantified remainder does not certify a numerical error at two finite parameter values. For any positive distinct parameters $h_1,h_2$ and prescribed observations $v_1,v_2$, every candidate [limit](limit-of-a-function.md) $L$ can be made consistent with a model $E(h)=L-ch^2-dh^3$: choose $c,d$ to solve $ch_i^2+dh_i^3=L-v_i$ for $i=1,2$. The coefficient [matrix](matrix.md) has nonzero [determinant](determinant.md) $h_1^2h_2^2(h_2-h_1)$. Thus the observations alone cannot identify $L$, even though every model has exactly the advertised $O(h^3)$ remainder in [Big O notation](big-o-notation.md). Quantitative remainder bounds or additional information are needed for an error certificate.

## ↑ Ancestors (6)

1. [Richardson extrapolation](richardson-extrapolation.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-numerical-analysis-course-of-the-university-of-oxford/2015/1/d/solution.md)
