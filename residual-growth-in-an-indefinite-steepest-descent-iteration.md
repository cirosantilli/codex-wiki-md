# Residual growth in an indefinite steepest-descent iteration

↑ **Parent:** [Gradient descent](gradient-descent-split.md)

For this nonsymmetric [matrix](matrix.md), consider the formal residual update $r^+=r-(r^Tr)/(r^TAr)Ar$, with nonzero $r=(x,y)^T$. Put $D=2x^2-2xy-2y^2$ and $B=5x^2+4xy+3y^2$. Algebra gives $r^+=(B/D)(-y,x)^T$ when $D\ne0$. But $B+D=7(x+y/7)^2+6y^2/7>0$ and $B-D=3(x+y)^2+2y^2>0$. Hence $B>|D|$ and $\|r^+\|>\|r\|$ for every defined nonzero step. At $D=0$, the quotient is undefined. Thus the iteration cannot converge to zero [linear-system residual](linear-system-residual.md) from any nonzero initial residual. This concrete divergence proof distinguishes failure of an algorithm from mere failure to meet a sufficient theorem's hypotheses.

## ↑ Ancestors (6)

1. [Gradient descent](gradient-descent-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/digital-systems-linear-algebra-introduction-to-formal-proof/6/c/ii/solution.md)
