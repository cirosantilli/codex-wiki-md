# Binary symmetric channel

↑ **Parent:** [Coding theory](coding-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Binary_symmetric_channel)

A [binary symmetric channel](binary-symmetric-channel.md) is a [discrete memoryless channel](discrete-memoryless-channel.md) that flips each transmitted [bit](bit.md) with fixed crossover [probability](probability.md) $p$. For one use, write $Y=X\oplus Z$, where $\oplus$ is [exclusive or](exclusive-or.md) and $Z$ is a [Bernoulli random variable](bernoulli-distribution.md) with parameter $p$, [independent](independent-random-variables.md) of the input $X$. Thus $Z=0$ preserves the [bit](bit.md) and $Z=1$ flips it. Different uses have independent noise under this model.

With row labels $X=0,1$ and column labels $Y=0,1$, its [transition matrix](stochastic-matrix.md) is

$$
\begin{pmatrix}1-p&p\\p&1-p\end{pmatrix}.
$$

Each row sums to one, and exchanging both binary labels leaves the rule unchanged, explaining symmetric. For $p=0.1$, a prescribed three-[bit](bit.md) input $010$ produces $010$ with [probability](probability.md) $0.9^3=0.729$ and $011$ with [probability](probability.md) $0.9^2(0.1)=0.081$. The received $011$ does not itself announce the changed position: it could also arise from input $011$ with no flips.

The [binary symmetric channel capacity](binary-symmetric-channel-capacity.md) quantifies how well a [block code](block-code.md) can overcome this uncertainty, and [input distribution optimization for a binary symmetric channel](input-distribution-optimization-for-a-binary-symmetric-channel.md) shows why a fair input attains the best information rate. A [completely noisy binary symmetric channel](completely-noisy-binary-symmetric-channel.md) has $p=1/2$ and carries no input information; a known flip on every use, $p=1$, is instead reversible.

**Table of contents**

- [Undetected error](undetected-error.md)
- [Completely noisy binary symmetric channel](completely-noisy-binary-symmetric-channel.md)
- [Positive-rate coding bound below one-quarter crossover](positive-rate-coding-bound-below-one-quarter-crossover.md)

## ↑ Ancestors (5)

1. [Coding theory](coding-theory-split.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (28)

- [Binary rate-distortion function](binary-rate-distortion-function.md)
- [Binary symmetric channel](binary-symmetric-channel.md)
- [Binary symmetric channel capacity](binary-symmetric-channel-capacity.md)
- [Channel capacity](channel-capacity.md)
- [Completely noisy binary symmetric channel](completely-noisy-binary-symmetric-channel.md)
- [Data processing inequality](data-processing-inequality.md)
- [Discrete memoryless channel](discrete-memoryless-channel.md)
- [Flips versus erasures in a binary channel](flips-versus-erasures-in-a-binary-channel.md)
- [Input distribution optimization for a binary symmetric channel](input-distribution-optimization-for-a-binary-symmetric-channel.md)
- [Mutual information](mutual-information.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4/4j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-30/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-30/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-73/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-1/12g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-1/12h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-48/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1/3g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2/3h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3/3g/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1/3k/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-2/3k/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/11i/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-1/11k/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-2/3k/solution.md)
- [Repetition code](repetition-code.md)
- [Worst-case correction guarantee from the Gilbert–Varshamov bound](worst-case-correction-guarantee-from-the-gilbert-varshamov-bound.md)
- [Z-channel](z-channel.md)
