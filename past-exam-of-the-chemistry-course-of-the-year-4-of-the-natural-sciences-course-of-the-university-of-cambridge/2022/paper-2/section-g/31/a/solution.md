<h1 id="section-g/31/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**Use symmetric single-bead displacements with the Metropolis acceptance rule, discard equilibration, and record the end-to-end distance after complete sweeps, including sweeps with rejected moves.** One sweep is $N$ attempted bead moves; it is a sampling index, not physical time.

```
INITIALIZE(N, sigma):
    for i = 1,...,N:
        r[i] = ((i-1)*sigma, 0, 0)
    return r

ENERGY(r):
    for each pair i < j:
        if norm(r[i]-r[j]) < sigma:
            return infinity
    U = 0
    for i = 1,...,N-1:
        U += k/2 * (norm(r[i+1]-r[i])-sigma)^2
    return U

TRIAL(r):
    choose i uniformly from 1,...,N
    choose delta uniformly from [-a,a]^3
    r_trial = copy(r)
    r_trial[i] += delta
    return r_trial

ACCEPT(U, U_trial, beta):
    if U_trial == infinity:
        return false
    return log(uniform(0,1)) < min(0, -beta*(U_trial-U))

MAIN:
    r = INITIALIZE(N, sigma)
    U = ENERGY(r)
    for sweep = 1,...,n_equilibrate+n_produce:
        repeat N times:
            r_trial = TRIAL(r)
            U_trial = ENERGY(r_trial)
            if ACCEPT(U, U_trial, 1/(k_B*T)):
                r = r_trial
                U = U_trial
        if sweep > n_equilibrate:
            d_ETE = norm(r[N]-r[1])
            store d_ETE and update its histogram
    estimate autocorrelation and block uncertainties
```

The straight initial chain is nonoverlapping and has zero bond-stretching energy, but is not presumed to be an equilibrium configuration. Check relaxation from contrasting initial configurations and stationarity before production. The displacement scale may be tuned during equilibration and then held fixed. Every sweep may be recorded; correlations are handled in uncertainty estimates rather than pretending adjacent records are independent. If thinning is used, choose its spacing with reference to the measured [autocorrelation time](../../../../../../autocorrelation-time.md). Rejected states must still be sampled to retain their correct equilibrium residence weight.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [31](../../31.md)
3. [Section G](../../../section-g.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../../chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
