# Gamma function recurrence

↑ **Parent:** [Gamma function](gamma-function.md)

The [Gamma function](gamma-function.md) obeys the [recurrence relation](recurrence-relation.md)

$$
\Gamma(z+1)=z\Gamma(z).
$$

Initially, for $\operatorname{Re}z>0$, [integration by parts](integration-by-parts.md) in the [Gamma integral](gamma-integral.md) gives the short proof

$$
\Gamma(z+1)=\int_0^\infty t^ze^{-t}\,dt=\left[-t^ze^{-t}\right]_0^\infty+z\int_0^\infty t^{z-1}e^{-t}\,dt=z\Gamma(z).
$$

The boundary term vanishes at zero because $|t^z|=t^{\operatorname{Re}z}\to0$, and at infinity because of exponential decay. Together with $\Gamma(1)=\int_0^\infty e^{-t}\,dt=1$, the [Gamma function recurrence](gamma-function-recurrence.md) immediately gives $\Gamma(n+1)=n!$ for every nonnegative [integer](integer.md) $n$.[NIST DLMF, equation 5.5.1: Gamma recurrence](https://dlmf.nist.gov/5.5#E1)

Read backwards, the [Gamma function recurrence](gamma-function-recurrence.md) defines

$$
\Gamma(z)=\frac{\Gamma(z+m)}{z(z+1)\cdots(z+m-1)},\qquad \operatorname{Re}(z+m)>0,
$$

where $m$ is a positive [integer](integer.md). These overlapping formulas agree by the [Gamma function recurrence](gamma-function-recurrence.md), giving the [meromorphic continuation](meromorphic-continuation.md). Since $\Gamma(1)=1$, they give a [simple pole](simple-pole.md) at zero and then at every negative [integer](integer.md); [Gamma function residue at a nonpositive integer](gamma-function-residue-at-a-nonpositive-integer.md) records the [residues](residue.md). The [recurrence relation](recurrence-relation.md) therefore holds throughout the continuation as an identity of [meromorphic functions](meromorphic-function.md).

## ↑ Ancestors (6)

1. [Gamma function](gamma-function.md)
2. [Complex analysis](complex-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (29)

- [Beta distribution](beta-distribution.md)
- [Beta-function recurrence](beta-function-recurrence.md)
- [Bohr-Mollerup theorem](bohr-mollerup-theorem.md)
- [Gamma function](gamma-function.md)
- [Gamma function has no zeros](gamma-function-has-no-zeros.md)
- [Gamma function recurrence](gamma-function-recurrence.md)
- [Gamma function residue at a nonpositive integer](gamma-function-residue-at-a-nonpositive-integer.md)
- [Global partial-fraction expansion of the zeta logarithmic derivative](global-partial-fraction-expansion-of-the-zeta-logarithmic-derivative.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-40/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-48/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-50/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-4/14e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-4/8e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-30/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-51/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-1/8e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-29/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-46/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-34/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-49/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-304/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-137/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-306/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/7a/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1/7e/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-3/17b/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-320/3/a/solution.md)
- [Power-law spherical projection kernel](power-law-spherical-projection-kernel.md)
- [Residues of the Gamma function](residues-of-the-gamma-function.md)
