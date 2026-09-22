<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The proposed hybrid recording rule updates the event times of students who leave but does not update the follow-up of those who remain. Thus the recorded end of observation depends on the subsequent outcome: this is [outcome-dependent updating of survival follow-up](../../../../../../outcome-dependent-updating-of-survival-follow-up.md).

In the four-student illustration, all four are known to be event-free at month six. Under the proposed coding, the three students without event reports are censored at month six, while the student whose event is subsequently reported remains in the [risk set](../../../../../../risk-set.md) until month seven. The recorded [risk set](../../../../../../risk-set.md) at that event therefore has size one, although the other three may still be studying. The [Kaplan–Meier estimator](../../../../../../kaplan-meier-estimator.md) factor would be $1-1/1=0$ and the [Nelson–Aalen estimator](../../../../../../nelson-aalen-estimator.md) jump would be $1/1=1$. This creates an artificial complete loss of estimated survival at that event.

If event notification is complete through the common eight-month cutoff, the absence of a notification establishes that the other three have not had the event by that cutoff. They should remain in the [risk set](../../../../../../risk-set.md) at month seven. With only these four subjects, the corresponding factors are instead $1-1/4=3/4$ and $1/4$. **Updating only failures while backdating nonfailures' [censoring](../../../../../../censoring-statistics.md) creates a severely biased [risk set](../../../../../../risk-set.md).** If notifications are incomplete, absence of a report does not establish continued study; positive follow-up confirmation is then required.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
