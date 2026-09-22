<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Maintain the latest five [temperature](../../../../../temperature-split.md) readings in a [circular buffer](../../../../../circular-buffer.md), together with their running [sum](../../../../../sum.md). The following [C programming language](../../../../../c-programming-language.md) code spells out the [message passing](../../../../../message-passing.md) interface rather than assuming a particular library: `send(dst,&m)` is a blocking [synchronous message passing](../../../../../synchronous-message-passing.md) send; `receive(src,&m)` receives from the specified sender or `ANY` and returns the sender's identity; `sendrec(dst,&m)` atomically sends the request and waits for that sender's reply in the same message object. Successful, reliable operations are assumed. Message contents are copied by the interface.

```
enum { ANY = -1, TIMER = 1, TEMP = 2 };
enum { PULSE, PING, REQUEST, REPLY };
typedef struct {
    int type;
    int period_ms;
    double value;
} Message;

extern void send(int dst, const Message *m);
extern int receive(int src, Message *m);
extern void sendrec(int dst, Message *m);

void smooth(void) {
    double history[5] = {0};
    double sum = 0;
    int count = 0, next = 0;
    Message m = { .type = PULSE, .period_ms = 1000 };
    send(TIMER, &m);                 /* subscribe once */

    for (;;) {
        int sender = receive(count < 5 ? TIMER : ANY, &m);
        if (sender == TIMER && m.type == PING) {
            Message t = { .type = REQUEST };
            sendrec(TEMP, &t);       /* matching REPLY contains t.value */
            if (count == 5)
                sum -= history[next];
            else
                ++count;
            history[next] = t.value;
            sum += t.value;
            next = (next + 1) % 5;
        } else if (count == 5 && m.type == REQUEST) {
            Message answer = { .type = REPLY, .value = sum / 5.0 };
            send(sender, &answer);
        }
    }
}
```

Before the fifth reading, selective reception from `TIMER` prevents premature client requests from being accepted. Such clients wait at their synchronous sends; they are not given a partial [arithmetic mean](../../../../../arithmetic-mean.md). Thereafter the [operating-system process](../../../../../process-computing.md) receives both timer messages and client requests. Each accepted `PING` initiates one measurement; each accepted client request returns the [arithmetic mean](../../../../../arithmetic-mean.md) of the five most recently completed measurements, without initiating another measurement or changing the [circular buffer](../../../../../circular-buffer.md).

The [loop invariant](../../../../../loop-invariant.md) is that `count` is the number of valid readings, capped at five, `sum` is their [sum](../../../../../sum.md), and `next` is the next unused slot during startup or the oldest slot afterwards. Removing the overwritten reading and adding the new one preserves this [loop invariant](../../../../../loop-invariant.md). Each update and reply uses $O(1)$ [time complexity](../../../../../time-complexity.md) and $O(1)$ storage, since the window length is fixed. Under timely sensor replies, timer delivery and [process scheduling](../../../../../process-scheduling.md), measurements are initiated once per second. The next parts explain failures of these timing assumptions; the code does not promise one-second sampling when the [sensor](../../../../../sensor.md) itself cannot sustain it.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
