<h1 id="b4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $m_i\in\{0,1\}$ for the true [DNA methylation](../../../../../dna-methylation.md) status and $o_i$ for its observation. The observation [likelihood function](../../../../../likelihood-function.md) is a [binary symmetric channel](../../../../../binary-symmetric-channel.md), so

$$
\log p(o\mid m)=\sum_{i=0}^{99}\begin{cases}\log(0.8),&o_i=m_i,\\\log(0.2),&o_i\ne m_i.\end{cases}
$$

For the loop suggested in the practical, set $p_i=(0.1,0.5,0.9)_{m_{i-1}+m_{i+1}}$ and add $\log p_i$ when $m_i=1$, or $\log(1-p_i)$ otherwise. The following independent implementation combines these terms without multiplying many small numbers:

```
import numpy as np

def methylation_score(pattern, observed):
    """Conditional-product score used by the practical's natural loop filling."""
    pattern=np.asarray(pattern,dtype=int);observed=np.asarray(observed,dtype=int)
    if pattern[0]!=1 or pattern[-1]!=1:return -np.inf
    neighbour_sum=pattern[:-2]+pattern[2:]
    p=np.array([.1,.5,.9])[neighbour_sum]
    prior_terms=np.where(pattern[1:-1]==1,p,1-p)
    observation_terms=np.where(pattern==observed,.8,.2)
    return float(np.log(prior_terms).sum()+np.log(observation_terms).sum())

log_likelihood = methylation_score
print(f"{log_likelihood(obs, obs):.2f}")
```

**The conditional-product log score at the observed pattern is $-102.14$.** The endpoint observations are included once each, while the endpoint statuses are fixed rather than assigned an additional prior probability.

There is a modeling qualification: multiplying the specified neighbour [conditional probabilities](../../../../../conditional-probability.md) gives a [pseudolikelihood](../../../../../pseudolikelihood.md), not generally the [joint probability distribution](../../../../../joint-probability-distribution.md) having those [conditional probabilities](../../../../../conditional-probability.md). Thus the function above defines the practical's conditional-product target; the pure observation [log-likelihood](../../../../../log-likelihood.md) at $m=o$ would instead be $100\log(0.8)=-22.3144$.

If the neighbour probabilities are intended literally as full conditionals of a [Markov random field](../../../../../markov-random-field.md), a coherent alternative has edge weights $T_{aa}=3/4$ and $T_{ab}=1/4$ for $a\ne b$, with both endpoints fixed. Given two equal neighbours, the matching centre has conditional odds $(3/4)^2:(1/4)^2=9:1$; mixed neighbours give equal weights. Consequently its unnormalized [posterior probability](../../../../../posterior-probability.md) has log score

$$
\ell_J(m;o)=\sum_{i=0}^{98}\log T_{m_i m_{i+1}}+\log p(o\mid m).
$$

For this alternative, $\ell_J(o;o)=-94.7394$ before the constant associated with conditioning the endpoints. It can be implemented as follows, but its numerical results must not be mixed with the conditional-product results in the remaining parts:

```
def joint_methylation_score(pattern,observed):
    """Coherent nearest-neighbour model with the specified full conditionals."""
    pattern=np.asarray(pattern,dtype=int);observed=np.asarray(observed,dtype=int)
    if pattern[0]!=1 or pattern[-1]!=1:return -np.inf
    edges=np.where(pattern[1:]==pattern[:-1],.75,.25)
    emissions=np.where(pattern==observed,.8,.2)
    return float(np.log(edges).sum()+np.log(emissions).sum())
```

## ↑ Ancestors (13)

1. [A](../a.md)
2. [B4](../../b4.md)
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
