# Right censoring

↑ **Parent:** [Censoring (statistics)](censoring-statistics.md)

An unobserved [survival time](survival-time.md) is [right-censored](right-censoring.md) when it is known to exceed the last event-free follow-up time. For a potential [survival time](survival-time.md) $T$ and potential observation-ending time $C$, record

$$
Y=\min(T,C),\qquad \delta=\mathbf1_{\{T\leq C\}}.
$$

When $\delta=1$, the occurrence was observed at $Y$; when $\delta=0$, only $T>Y=C$ is known. An intact machine at the study's closing date and an event-free subject who stops attending follow-up can both yield [right censoring](right-censoring.md), but the reasons for stopping matter for [independent censoring](independent-censoring.md). A subject [right-censored](right-censoring.md) at year two has contributed two years to [person-time at risk](person-time-at-risk.md) and belongs to earlier [risk sets](risk-set.md). Neither recording a failure at year two nor discarding that subject preserves this information.

Under [independent censoring](independent-censoring.md) and separate parameters for the observation mechanism, the part of the [survival likelihood](survival-likelihood.md) involving an [absolutely continuous probability distribution](absolutely-continuous-probability-distribution.md) for $T$ is $f(Y)^\delta S(Y)^{1-\delta}$. Thus a [right-censored](right-censoring.md) observation contributes the [survival function](survival-function.md) $S(Y)$, rather than the event [probability density function](probability-density-function.md) $f(Y)$. See [Lu Tian's Stanford notes, Section 2.1, equations (2.1)–(2.2)](https://web.stanford.edu/~lutian/coursepdf/unit2.pdf). The [Kaplan–Meier six-subject cohort](kaplan-meier-six-subject-cohort.md) shows exactly how this distinction changes the calculation.

## ↑ Ancestors (6)

1. [Censoring (statistics)](censoring-statistics.md)
2. [Survival analysis](survival-analysis-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (43)

- [Aalen–Johansen estimator](aalen-johansen-estimator.md)
- [EM algorithm for a censored lognormal competing-risks mixture](em-algorithm-for-a-censored-lognormal-competing-risks-mixture.md)
- [Events divided by exposure estimator](events-divided-by-exposure-estimator.md)
- [Kaplan–Meier estimator](kaplan-meier-estimator.md)
- [Kaplan–Meier six-subject cohort](kaplan-meier-six-subject-cohort.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-37/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-38/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-44/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-44/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-46/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-46/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-41/5/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-41/5/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-37/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-37/5/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-32/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-32/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-32/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-32/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-32/7/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-33/5/b/i/solution.md)
- [4](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-207/4.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-207/3/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-207/4/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-207/4/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-207/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-207/4/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-207/4/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-207/4/c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-207/4/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-207/5/b/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-207/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-207/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-207/5/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-207/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-207/6/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-207/5/a/solution.md)
- [Potential right-censoring time](potential-right-censoring-time.md)
- [Right censoring](right-censoring.md)
- [Risk set](risk-set.md)
- [Survival analysis](survival-analysis-split.md)
- [Survival data](survival-data.md)
- [Survival time](survival-time.md)
