# Distributed Systems

Lecture notes for course [CSE138, Spring 2020](http://composition.al/CSE138-2020-03/index.html) given by [Prof Lindsey Kuper](https://users.soe.ucsc.edu/~lkuper/), Assistant Professor of Computing as UCSC

Due to the Covid-19 lockdown being enforced at the time, these lectures had to be delivered online and are available on [YouTube](https://www.youtube.com/user/lindseykuper/videos) and [Twitch](https://www.twitch.tv/lindseykuper/videos)

This series of lectures also includes a discussion panel with recent grad students and two guest lectures.  Notes have not been created for any of these videos; however, you can watch them here:

* ["Grad Student Discussion Panel"](https://www.youtube.com/watch?v=ArKapXZkJvM) Lindsey Kuper talks with Emma Gomish, Pete Wilcox and Lawrence Lawson. May 15<sup>th</sup>, 2020
* ["Blockchain Consensus"](https://www.youtube.com/watch?v=m6qZY7_ingY) by Chris Colohan, May 27<sup>th</sup>, 2020
* ["Building Peer-to-Peer Applications"](https://www.twitch.tv/videos/640120840) by Karissa McKelvey, June 3<sup>rd</sup>

|  Date | Description | Subjects Recapped |
|---|---|---|
| Lecture 1 | There are no notes for this lecture as it was concerned with course administration and logistics  |
| [Lecture 2](./Lecture%202.md)<br>April&nbsp;1<sup>st</sup>,&nbsp;2020 | Distributed Systems: What and why?<br>Time and clocks |
| [Lecture 3](./Lecture%203.md)<br>April&nbsp;3<sup>rd</sup>,&nbsp;2020| Lamport diagrams<br>Causality and happens-before<br>Network models<br>State and events<br>Partial orders
| [Lecture 4](./Lecture%204.md)<br>April&nbsp;6<sup>th</sup>,&nbsp;2020 | Total orders and Lamport clocks | Partial orders<br>Happens-before
| [Lecture 5](./Lecture%205.md)<br>April&nbsp;8<sup>th</sup>,&nbsp;2020 | Vector clocks<br>Protocol runs and anomalies<br>Delivery vs. Receiving<br>FIFO delivery | Lamport Clocks
| [Lecture 6](./Lecture%206.md)<br>April&nbsp;10<sup>th</sup>,&nbsp;2020 | Causal delivery<br>Totally-ordered delivery<br>Implementing FIFO delivery<br>Preview of implementing causal broadcast | Delivery vs. receiving<br>FIFO delivery
| [Lecture 7](./Lecture%207.md)<br>April&nbsp;13<sup>th</sup>,&nbsp;2020 | Implementing causal broadcast<br>Uses of causality in distributed systems<br>Consistent snapshots<br>Preview of Chandy-Lamport snapshot algorithm | Causal anomalies and vector clocks
| [Lecture 8](./Lecture%208.md)<br>April&nbsp;15<sup>th</sup>,&nbsp;2020 | Chandy-Lamport Snapshot Algorithm |
| [Lecture 9](./Lecture%209.md)<br>April&nbsp;17<sup>th</sup>,&nbsp;2020 | Chandy-Lamport wrap-up: limitations, assumptions and properties<br>Uses of snapshots<br>Centralized vs. decentralized algorithms<br>Safety and liveness | Delivery guarantees and protocols
| [Lecture 10](./Lecture%2010.md)<br>April&nbsp;20<sup>th</sup>,&nbsp;2020 | Reliable delivery<br>Fault classification and fault models<br>The Two Generals problem | Safety and liveness
| [Lecture 11](./Lecture%2011.md)<br>April&nbsp;22<sup>nd</sup>,&nbsp;2020 | Implementing reliable delivery<br> Idempotence<br>At-least-once/at-most-once/exactly-once delivery<br>Unicast/Broadcast/Multicast<br>Reliable broadcast<br>Implementing reliable broadcast<br>Preview of replication
| [Lecture 12](./Lecture%2012.md)<br>April&nbsp;24<sup>th</sup>,&nbsp;2020 | Replication<br>Total order vs. determinism<br>Consistency models: FIFO, causal and strong<br>Primary-backup replication<br> Chain replication<br>Latency and throughput
| [Lecture 13](./Lecture%2013.md)<br>April&nbsp;27<sup>th</sup>,&nbsp;2020 | **Pause for breath!**<br>Wrapping up replication techniques
| [Lecture 14](./Lecture%2014.md)<br>May&nbsp;1<sup>st</sup>,&nbsp;2020 | Handling node failure in replication protocols<br>Introduction to consensus<br>Problems equivalent to consensus<br>The FLP result<br>Introduction to Paxos | Strongly consistent replication protocols
| [Lecture 15](./Lecture%2015.md)<br>May&nbsp;4<sup>th</sup>,&nbsp;2020 | Paxos: the interesting parts
| [Lecture 16](./Lecture%2016.md)<br>May&nbsp;6<sup>th</sup>,&nbsp;2020 | Paxos wrap-up: Non-termination, Multi-Paxos, Fault tolerance<br>Other consensus protocols: Viewstamped Replication, Zab, Raft<br>Passive vs. Active (state machine) replication
| [Lecture 17](./Lecture%2017.md)<br>May&nbsp;8<sup>th</sup>,&nbsp;2020 | Eventual consistency<br>Strong convergence and strong eventual consistency<br>Introduction to application-specific conflict resolution<br>Network partitions<br>Availability<br>The consistency/availability trade-off
| [Lecture 18](./Lecture%2018.md)<br>May&nbsp;11<sup>th</sup>,&nbsp;2020 | Dynamo: A review of old ideas<ul><li>Availability</li><li>Network partitions</li><li>Eventual consistency</li><li>Vector clocks</li><li>Application-specific conflict resolution</li></ul>Introduction to:<ul><li>Anti-entropy with Merkle trees</li><li>Gossip</li><li>Quorum consistency</li></ul>
| [Lecture 19](./Lecture%2019.md)<br>May&nbsp;13<sup>th</sup>,&nbsp;2020 | More about Quorum Consistency<br>Introduction to sharding<br>Consistent hashing
| [Lecture 20](./Lecture%2020.md)<br>May&nbsp;18<sup>th</sup>,&nbsp;2020 | Online systems vs. Offline systems<br>Raw data vs. Derived data<br>Introduction to Google's MapReduce framework<br>MapReduce example: transform a forward index into an inverted index
| [Lecture 21](./Lecture%2021.md)<br>May&nbsp;20<sup>th</sup>,&nbsp;2020 | MapReduce<ul><li>Types</li><li>Approach to fault tolerance</li><li>Combine functions</li><li>More examples</li></ul> | MapReduce phases
| [Lecture 22](./Lecture%2022.md)<br>May&nbsp;29<sup>th</sup>,&nbsp;2020 | The math behind replica conflict resolution<ul><li>Upper bounds</li><li>Least upper bounds</li><li>Join-semilattices</li></ul> | Strong convergence<br>Partial orders
| [Lecture 23](./Lecture%2023.md)<br>June&nbsp;1<sup>st</sup>,&nbsp;2020 | Filling in the gaps: Overviews of 2-phase commit and Practical Byzantine Fault Tolerance (PBFT)<br>Quick overview of the history of:<ul><li>Lamport and Vector Clocks</li><li>Replication Strategies</li><li>Consensus</li><li>Replication Needs Consensus</li></ul>



# Distributed Systems Lecture 2

## Lecture Given by [Lindsey Kuper](https://users.soe.ucsc.edu/~lkuper/) on April 1<sup>st</sup>, 2020 via [YouTube](https://www.youtube.com/watch?v=G0wpsacaYpE)

| Previous | Next
|---|---
| | [Lecture 3](./Lecture%203.md)

## What is a Distributed System?

Leslie Lamport gives the rather comical definition that:

> *"A distributed system is one in which I can't get my work done because a computer I've never heard of has crashed"*

Although he was joking, this definition captures a very important aspect of a distributed system in that it is one defined by some type of failure.

Martin Kleppmann's definition of a distributed system is somewhat more serious (he's the author of a book called [Designing Data Intensive Systems](https://www.amazon.co.uk/Designing-Data-Intensive-Applications-Reliable-Maintainable-ebook/dp/B06XPJML5D/ref=sr_1_1)).

> A distributed system runs on several nodes (computers) and is characterised by partial failure

However, other definitions of a distributed system include ideas such as:

- Systems where work is distributed fairly between nodes, or
- Where multiple computers "behave as one"

These last definitions, however, are all rather too optimistic because they do not account for any real-life difficulties - one of which is mentioned in Martin Kleppman's definition.

## What is Partial Failure?

Partial failure is where some component of a computation fails, but that failure is not necessarily fatal.  For instance, one machine in a cluster of 1000 could fail without there being any significant impact on the overall "system".  In other words, the presence of this type of partial failure is non-fatal to the operation of your system as a whole.


## "Cloud Computing" vs. "High Performance Computing (HPC)"


The problem with HPC is that it treats partial failure as total failure.  Consequently, HPC must rely on techniques such as check-pointing.  This is where the progress of the calculation is saved at regular intervals so that in the event of a failure, the computation can be continued from the last check point without needing to start over from the beginning.


However, in computing in general and specifically in Cloud Computing, it is expected that various parts of the system will fail.  Consequently, this type of behaviour is a fundamental part of the software design.

Had Ben Franklin been a programmer, he would probably have said:

![Ben Franklin](./img/Ben%20Franklin.jpg)

Failure can occur in many ways.  For instance:

- Network partition
- Hardware failure
- Software failure

### Determining the Cause of Failure

In a minimal cluster of two computers `M1` and `M2`, `M1` wants to ask `M2` for the value of a particular variable:

- `M1` sends a message to `M2` saying *"What's the value of `x`?"*
- `M2` should then respond with another message saying *"`x=5`"*

![Message 1](./img/L2%20Message%201.png)

But in in this very simple scenario, the number of possibilities for failure is still very high:

- `M1`'s message might get lost due to network failure
- `M1`'s message is delivered very slowly due to unexpectedly high network latency
- `M2` could be down
- `M2` might crash immediately after reporting to `M1` that it is alive, but before receiving `M1`'s message
- `M2` might crash as a result of trying to respond to `M1`'s message
- `M2` might refuse to respond to the question due to some type of authentication or authorisation failure
- `M2` responds correctly, but the message never gets back to `M1`
- Some random external event such as a cosmic ray flips a bit in the message thus corrupting it (Byzantine error)

And on and on...

Although the underlying causes are very different, as far as `M1` is concerned, they all look the same.  All `M1` can tell is that it never got an answer to its question.

In fact, it is impossible to determine the cause of such a failure without first having global knowledge of the entire system.

### Timeouts

It is often assumed that `M1` must wait for some predefined timeout period, after which it should assume failure if it does not receive an answer.  But the problem is that network latency is indeterminate; therefore, waiting for an arbitrary timeout period might help to trap *some* errors, but in general, it is not a good strategy for determining failure.

For example, instead of asking *"What is the value of `x`"*, `M1` could ask `M2` to *"Add 1 to `x`"*.

***Q:***&nbsp;&nbsp;How will `M1` know this request was successfully processed?  Should it simply wait for a predetermined timeout period and if it hears nothing back, assume everything's fine?
***A:***&nbsp;&nbsp;No, `M1` can only discover the success or failure of its request when it receives some sort of acknowledgement back from `M2`.

If `M1` does not receive a response within its timeout period, what should it conclude?

We can see that without any additional information, it is not correct for `M1` to assume either success or failure.  All `M1` can say with any certainty is that from its point of view, the state of variable `x` in `M2` is indeterminate.

### Realistic Timeout Values?

If the maximum network delay for message transmission is `D` seconds and the maximum time a machine spends processing a request is `R`, then the upper bound of the message handling timeout should be `2D + R` (two network journeys (send and receive) plus the remote machine's processing time).  This would rule out the uncertainty for timeouts in a slow network, but still leave us completely unable to reason about any other types of failure.

In distributed systems, we must deal not only with the problems of "Partial failure", but also the problem of "Unbounded Latency" (the definition given by [Peter Alvaro](https://dl.acm.org/profile/81453654530) - one of Lindsey Kuper's colleagues)

***Q:***&nbsp;&nbsp;Given they're so hard to debug, why would you want to use a distributed system?
***A:***&nbsp;&nbsp;Well, largely because we have no choice.  All manner of external factors can force us to distribute either a computation or storage (or both) across multiple machines&hellip;

- Too much data to fit on a single machine
- Need a faster response time, so we have to throw more processing power at the problem
- Scalability (need to handle more data, more users, or simply need more CPUs)
- Fault Tolerance (redundancy)


## Time and How We Measure it

Computers use clocks to identify specific points in time (both past and present).  For example:

- This class starts at 09:00
- This item in the cache expires tomorrow at 4:26 PM
- This log event happened yesterday at 11:31:34.352

Computers also use clocks for reasoning about time intervals:

- This class is 65 minutes long
- This access code will expire in 30 seconds time
- This user spent 4 minutes 38 seconds on our website


### Time-of-Day Clocks

Computers have two types of clock, time-of-day clocks and monotonic clocks.

- Time-of-day clocks are typically synchronised across different machines using [NTP](http://www.ntp.org/)
- Time-of-day clocks are ***bad*** for measuring intervals between events taking place on different machines:
    -  The clocks on the different machines may not be synchronised correctly and may disagree on the exact size of a time interval
    -  There are several cases where the time-of-day clock can jump:
        - Daylight saving time just started
        - A leap second happens
        - NTP resets the machine's clock to an earlier value
- Time-of-day clocks are OK for timestamping events at a course degree of accuracy, but not if a high degree of accuracy is needed

There is a general principle in timekeeping: the more accurately you need to measure time, the harder that task becomes.  If you now try to get two or more computers to agree on what the time is, then the difficulty is only compounded.

### Monotonic clocks

A value is said to be *"monotonic"* if it only ever changes in one direction.  So, a monotonic clock is one that will ***never*** jump backwards; its counter is guaranteed only to get bigger.

A monotonic clock:

- Is simply a counter value whose only ever gets bigger (E.G. microseconds since system boot)
- Has no meaning outside the machine on which it exists; therefore, it makes no sense to compare monotonic clock values between different machines.  Monotonic values are useless as timestamps
- Is ideally suited for measuring the duration of a task, or the time interval between events on a single machine

Time of day and monotonic clocks are both physical clocks (I.E. they are concerned with quantifying a time interval between now and some fixed reference point in the past such as Jan 1st, 1970 or when the machine was started)

***Q:***&nbsp;&nbsp;So how do we mark points in time that are valid across multiple machines?
***A:***&nbsp;&nbsp;If we use any sort of physical clock, then it is very tricky.

### What's the Time, Mr Lamport?

If we think we can solve this problem by repeatedly asking a physical clock *"What's the time?"*, then in fact, we are asking the wrong question because we have misunderstood the problem.

Machines in a distributed system don't need to know what the time is in any absolute sense, all they need to be able to do is answer the question ***"Which event happened first?"***.  This is why distributed systems use a very different notion of what a clock is; they use something called a ***Logical Clock*** (a.k.a. a Lamport Clock).

Counter-intuitively, a logical clock measures neither the time of day nor the elapsed interval between two events; instead, it measures nothing more than the ordering of events.

At first, this concept is not easy to grasp because it goes against our firmly established notion of what a clock is (or ought to be).  But in order to answer the all-important question ***"Which event happened first?"*** we don't need to reference the time of day, we just need some sort of counter that clicks up every time an event occurs.  This type of *"clock"* is very important for several reasons:

* Communication is unreliable
    This means that the length of time taken for message transmission is unpredictable (a phenomenon known as *"unbounded latency"*)
* Unpredictable changes of state
    E.G. the last time you asked machine `M2` what the value of `x` was, it said `x=5`; but in the meantime, some other machine has changed `x` to `6` and hasn't told you&hellip;

In these situations, it is vital to know the order in which events occurred.

### Event Ordering

Let's says we have two database events `A` and `B` and we know that `A` happened before `B`.  So we denote this relationship by the syntax `A -> B`.  This is pronounced *"`A` happens before `B`"*

But what does this tell us about causality?

All we can really say is that event `A` ***might*** have been the cause of event `B`, but we cannot be certain about this.  All we can say with absolute certainty is that since `B` happened ***after*** `A`, it is ***impossible*** for `B` to have been the cause of `A`.

Questions about causality are very important in distributed systems because they help us solve problems such as debugging.

If `M1` thinks `x=1`, but `M2` thinks `x=5`, then by knowing when the value of `x` changed in each machine, we can rule out those events that did ***not*** contribute to the problem.  This greatly helps in narrowing down what ***is*** the cause of the problem.

This determinism is also useful when designing systems in which users see a sequence of events.  You know that if event `A` happened before event `B`, then you can ensure that your system will ***never*** display event `B` to the user before they have first seen event `A`.

---

| Previous | Next
|---|---
| | [Lecture 3](./Lecture%203.md)


# Distributed Systems Lecture 3

## Lecture Given by [Lindsey Kuper](https://users.soe.ucsc.edu/~lkuper/) on April 3<sup>rd</sup>, 2020 via [YouTube](https://www.youtube.com/watch?v=83Ha1rX2LSw)

| Previous | Next
|---|---
| [Lecture 2](./Lecture%202.md) | [Lecture 4](./Lecture%204.md)

## Causality and the "Happens Before" Relation

The notation `A -> B` means *"A happens before B"* and helps make the ordering of events in time explicit.

The "happens before" relation allows us to conclude two things:

1. It is possible that event `A` ***might*** have been the cause of event `B`
1. It is ***completely impossible*** for event `B` to have been the cause of event `A`

In other words, the arrow in the happens before relation indicates the direction of possible causality.

## Lamport Diagrams (a.k.a. Spacetime Diagrams)

With time moving downwards, draw a vertical line to represent the events that happen within a process.<sup id="a1">[1](#f1)</sup>   Events are then represented as dots on that line.

![Process events](./img/L3%20Process%20events.png)

This diagram tells us that three events have taken place within this process and that they happened in the order `X` followed by `Y` followed by `Z`.  From this, we can then infer the following:

* Event `X` happened before events `Y` and `Z`, and therefore ***might*** be their cause, but we cannot be certain about this
* Event `Y` happened before event `Z` and therefore ***might*** be its cause, but again, we cannot be certain about this
* Events `Y` and `Z` happened after event `X`. We can therefore say with 100% certainty that `X` was not caused by either `Y` or `Z`
* Event `Z` happened after event `Y`.  We can therefore say with 100% certainty that `Y` was not caused by `Z`

In the case of multiple machines, we would represent these as a set of adjacent vertical lines, each with their own timeline of events.

![Multiple processes](./img/L3%20Multiple%20Processes.png)

### Communication Between Machines

The only way these machines can communicate with each other is by sending messages.  The send and receive events are represented as dots on each machine's timeline.

![Message passing between processes](./img/L3%20Message%20Passing.png)

Generally speaking, given two events, `A` and `B`, we can say that `A` happens before `B` (`A -> B`) if any of the following are true:

- Events `A` and `B` are events in the same process and `B` happens after `A`
- If `A` is a message send event and `B` is the corresponding receive event, then `B` must have happened after `A`.
    Sorry kids, time travel is not possible, so it makes no sense to talk of a message being received ***before*** it was sent
- If `A -> C` and `C -> B`, the we can be certain that `A -> B` (This is known as transitive closure)

This is the definition of the ***"happens before"*** relation.

## Causal Anomalies

Here's an example that highlights the importance of needing to know the exact order in which events occurred.  Without this knowledge, you might well be left wondering why you've received a particular message.

![A causal anomaly](./img/L3%20Causal%20Anomaly.png)

1. Alice thinks Bob has a problem with personal hygiene and sends a message to both Bob and Carol saying *"Bob Smells"*
1. Bob takes offence and immediately responds to both Alice and Carol by saying *"Up yours!"*
1. However, Alice's original message to Carol is delayed for some reason, and results in Bob's rude response arriving ***before*** Alice's original message

Without a clear understanding of concept of the "happens before", Carol will not understand why Bob has apparently started sending her insulting messages.

## Network Models

### How Long Does it Take to Send a Message?<br>(Would that be Synchronous or Asynchronous?)

If we could say with certainty that sending a network message required no more than `N` units of time, then we would have a much better idea of how communication should be managed.  If such an upper limit could be placed on communication performance, then using timeouts to reason about communication failure would be a reasonable approach.

Networks that make such timing guarantees are known as "synchronous networks" (E.G a network in which we know that message transmission will take no more than `N` units of time).  In general however, synchronous networks require the existence of a stable circuit between sender and receiver &mdash; which is exactly what does not exist in either public switched telephone neworks ([PSTNs](https://en.wikipedia.org/wiki/Public_switched_telephone_network)) or the internet.

The internet is an asynchronous network (I.E. a network having no central point of control and in which there is no upper bound on message transmission time)

> As an aside, there is also a type of network known as *"partially synchronous network"* in which the upper bound on transmission time is large, but finite. (For details, see the book [Distributed Algorithms](https://www.amazon.co.uk/Distributed-Algorithms-Kaufmann-Management-Systems-ebook/dp/B006QUTUR2/ref=sr_1_1) by Nancy Lynch)

### But Can We Reason About Transmission Times?

Well, it depends on the type of network you're using...

The least forgiving network model is the asynchronous one.  By *"least forgiving"*, we mean a network that:

*  Makes the least number of assumptions about message transmission, and
*  Allows us the least scope for reasoning about its behaviour

In spite of it being so unforgiving, the most robust designs are built on asynchronous networks.  The flip side of this however is that these are also the hardest networks to reason about.  One of the key consequences here is that it we have no ability to describe all possible behaviours our system might exhibit, and without this ability, we cannot protect our system against ***all*** possible error conditions (only some).

If, on the other hand, you want to prove than a certain type of event is impossible, then you should choose the most forgiving network model (the synchronous one), for if you can prove that a certain event is impossible in the most forgiving network (for instance, where message delivery is known never to exceed `N` units of time), then you can also be certain that the same event will be impossible in the least forgiving network where `N` is unbounded.

Here, a *"forgiving network protocol"* is one that makes the most assumptions and allow us the greatest scope for reasoning about its behaviour


## State

So far, our Lamport diagrams only show events and the transmission of messages between processes.  How then should state be described?

### What is the 'State' of a Computer?

The term "state" is typically understood to mean the contents of a computer's storage (registers, memory and permanent storage) at some particular point in time.

So, if at some particular point in time, `x=5`, then it follows that there must have been some previous point in time when `x` did not equal `5`.  The transition from `x` not equalling `5` to `x` equalling `5` is an event that can be represented on a Lamport diagram.  So, events can also be thought of as representing changes of state.

So, it might seem reasonable to propose that we should be able to reconstruct a machine's state at any point in time if we know two things:

1. The *full* history of all events that led up to `x` becoming equal to `5`
1. The precise order in which those events occurred

In reality however, even if we have this knowledge, it might still not be possible to reconstruct the state.

### Reasoning About State

There are three different ways in which events can be ordered using the `->` *"happens before"* relation:

1. Events `A` and `B` occur in the same process, with `B` happening after `A`
1. If `A` is a message send event and `B` is the corresponding receive event, then `B` ***must*** happen after `A` because it makes no sense to talk of a receive event happening ***before*** its corresponding send event
1. If `A -> C` and `C -> B`, then we can be certain that `A -> B` (Transitive closure)


So, if `A -> B`, then events `A` and `B` form a pair of events ordered by the **"happens before"** relation.

![Reasoning about State](./img/L3%20Reasoning%20About%20State.png)

What can we say about the ordering of these events?

* From rule 1: `B -> C`
* From rule 2: `A -> B` and `D -> C`
* From rule 3: `A -> C`

***Q:***&nbsp;&nbsp; What can we say about the order of events `A` and `B` in relation to event `D`?
***A:***&nbsp;&nbsp; Absolutely nothing!


So, the state of the machine is represented by the smallest set of ordered pairs, that is:

```
 { (A,B)
  ,(B,C)
  ,(A,C)
  ,(D,C)
  }
```

This list includes only those event pairs that obey the ***happens before*** relation.

What then can we say about the events shown in the following diagram?

![Message passing between processes](./img/L3%20Message%20Passing.png)

***Q:***&nbsp;&nbsp; Does `P` happen before `S`?
***A:***&nbsp;&nbsp; Yes, `P` is a send event and `S` is the corresponding receive event, therefore `P -> S`

***Q:***&nbsp;&nbsp; What about `X` and `Z`?
***A:***&nbsp;&nbsp; Yes, events `X` and `Z` occur within the same process and `Z` happens after `X`, therefore `X -> Z`

***Q:***&nbsp;&nbsp; What about `P` and `Z`?
***A:***&nbsp;&nbsp; Yes, `P -> S`, and `S` and `Z` are in the same process with `Z` happening after `S`, therefore `P -> Z`

***Q:***&nbsp;&nbsp; What about `Q` and `R`?
***A:***&nbsp;&nbsp; We do know that `Q` was caused by `T` and that `T -> Z` and `Z -> U` and `U -> R`; however, we are not allowed to determine causality by travelling backwards in time, so we must conclude that `Q` and `R` are ***not*** related by the "happens before" relation.  In spite of the visual position of the dots in the diagram, we are unable to say which event happened first.

Another way of saying this is that the ***"happens before"*** relation cannot be used to form an ordered pair from `Q` and `R`.  All we can say about `Q` and `R` is that these events are **"concurrent"** or **"independent"**.  This is written as `Q || R`.

In the above diagram, events `X` and `P`, and `Z`, `U`, `V` and `Q` are also concurrent.


## Partial Orders

A partial order is where, for a given set `S`, a binary relation holds that exhibits the following properties.  This binary relation is usually, but not always written as `≤` (less than or equals) and allows you to compare two members of `S` using the following properties:

| Property | English Description | Mathematical Description |
|---|---|---|
| Reflexivity   | For all `a` in `S`,<br>`a` is always `≤` to itself | `∀ a ∈ S: a ≤ a`
| Anti-symmetry | For all `a` and `b` in `S`,<br>if `a ≤ b` and `b ≤ a`, then `a = b` | `∀ a, b ∈ S: a ≤ b, b ≤ a => a = b`
| Transitivity  | For all `a`, `b` and `c` in `S`,<br>if `a ≤ b` and `b ≤ c`, then `a ≤ c` | `∀ a, b, c ∈ S: a ≤ b, b ≤ c => a ≤ c`

However, when the members of the set are events whose ordering is determined by some measure of time, it makes no sense to say that event `A` ***"happens before"*** itself; so when speaking of a set of events, the reflexivity property is nonsensical and therefore not applicable.

Also, we will never encounter the situation in a distributed system where event `A` happens before event `B` ***and*** event `B` happens before event `A` (making `A` and `B` the same event).  Thus, the anti-symmetry property can never be adhered to in real life.  Strictly speaking however, whilst this rule is never followed, it is also never violated; therefore, this rule is said to be ***"vacuously true"***.  That is, when dealing with a set of real-life events, we will never find an example that exhibits this property; however, we will also never find an example that violates this property either...

So, the "happens before" relation is a weird kind of partial order because only two of the three rules governing partial orders apply, and even then, one of those two is only vacuously true.

Therefore, the ***happens before*** relation is said to be *"an irreflexive partial order"*.


In distributed systems, we will be dealing with many different kinds of partial order.  It is strange however that the first partial order we encounter is "happens before", but this is because it is both fundamental to distributed systems, but also a weird kind of partial order.


Whenever we talk about a relation being a partial order, we must first look at the set of things we're dealing with.  If we're dealing with the "happens before" relation, then we're dealing with a set of events.

---

| Previous | Next
|---|---
| [Lecture 2](./Lecture%202.md) | [Lecture 4](./Lecture%204.md)

---

***Endnotes***

<b id="f1">1</b>&nbsp;&nbsp; It is not a requirement for the direction of time to be downwards in a Lamport Diagram. This is simply a stylistic choice; however, time is most often drawn moving either downwards, or from left to right.

[↩](#a1)

# Distributed Systems Lecture 4

## Lecture Given by [Lindsey Kuper](https://users.soe.ucsc.edu/~lkuper/) on April 6<sup>th</sup>, 2020 via [YouTube](https://www.youtube.com/watch?v=zQk7U6InXZs)

| Previous | Next
|---|---
| [Lecture 3](./Lecture%203.md) | [Lecture 5](./Lecture%205.md)

## Recap

### What is a Distributed System?

> ***[Martin Kleppman](https://martin.kleppmann.com/)'s definition***
> A collection of computing nodes connected by a network and characterised by partial failure

> ***[Peter Alvaro](https://dl.acm.org/profile/81453654530)'s definition***
>  A collection of computing nodes connected by a network and characterised by partial failure and unbounded latency


### What is the Definition of the *"Happens Before"* Relation

* Events `A` and `B` take place in the same process and `B` happens after `A`
* If `A` is a message send event and `B` is the corresponding receive event, then `B` ***cannot*** have happened before `A`.
* If `A -> C` and `C -> B`, the we can be certain that `A -> B` (Transitive closure)


### The *"Happens Before"* Relation is an Irreflexive Partial Order

A partial order for a set `S` is where the members of `S` can be ordered using a binary relation such as *"less than or equal to"* `≤`.  The partial order then has the following properties:

| Property | English Description | Mathematical Description |
|---|---|---|
| Reflexivity   | For all `a` in `S`,<br>`a` is always `≤` to itself | `∀ a ∈ S: a ≤ a`
| Anti-symmetry | For all `a` and `b` in `S`,<br>if `a ≤ b` and `b ≤ a`, then `a = b` | `∀ a, b ∈ S: a ≤ b, b ≤ a => a = b`
| Transitivity  | For all `a`, `b` and `c` in `S`,<br>if `a ≤ b` and `b ≤ c`, then `a ≤ c` | `∀ a, b, c ∈ S: a ≤ b, b ≤ c => a ≤ c`

The set of all events in a system can be ordered by the *"happens before"* partial order; however, in the case of events, not all of the three properties described above are applicable.  It is impossible to apply the reflexivity property simply because it makes no sense to say that an event *happened before itself*.

### Accurate Terminology

Don't get hung up on thinking that you must always state that the "happens before" relation is an irreflexive partial order.  It’s fine just to call it a "partial order".



## What's an Example of a True Partial Order?

Set inclusion (or set containment).  This is defined as the set of all subsets of any given set.

So, if we have a set `{a, b, c}`, then the containment set `S` contains the following 8 elements; each of which is one of the possible subsets of `{a, b, c}` (Don't forget to include both the empty set and the entire set!):

```
{ {}
, {a}
, {b}
, {c}
, {a, b}
, {a, c}
, {b, c}
, {a, b, c}
}
```

All of these members are subsets of the original set and are related by the relation `⊆` (meaning "is a subset of") and can be represented as a lattice with the empty set at the bottom

![Partial order lattice](./img/L4%20Lattice.png)

The `⊆` relation ("is a subset of") is a true partial order because every element of the set adheres to the rules of:

* Reflexivity
* Antisymmetry
* Transitivity

## Total Orders

As an aside...

***Q:***&nbsp;&nbsp; In the above inclusion set `S`, how is the element `{a}` related to the element `{b,c}`?
***A:***&nbsp;&nbsp; It's not!  In a set defined by a ***partial order***, it is not possible to relate every member of that set to every other member. That's why its called a ***partial*** order!

Some orders however are able to relate every element in a set to every other element in that set.  These are known as ***total orders***.

A good example of a total order is the counting (or natural) numbers.  If our set is the natural numbers and the relation is `≤`, then our lattice diagram of the containment set is simply a straight line:

![Total order](./img/L4%20Natural%20Numbers.png)

This is because every natural number is comparable to every other natural number using the `≤` relation.


## How Can a Computer Determine the *"Happens Before"* Relation?

This question relates to clocks - specifically ***Logical Clocks***

> A logical clock is a very unusual type of clock because it can neither tell us the time of day, nor how large a time interval has elapsed between two events.
> All a logical clock can tell us is the order in which events occurred.

### Lamport Clocks

The simplest type of logical clock is a ***Lamport Clock***.  In its most basic form, this is simply a counter assigned to an event.  The way we can reason about Lamport Clock values is by knowing that:

```
  if A -> B then LC(A) < LC(B)
```

In other words, if it is true that event `A` happened before event `B`, then we can be certain that the Lamport Clock value of event `A` will be smaller than the Lamport Clock value of event `B`.

It is not important to know the absolute Lamport Clock value of an event, because outside the context of the *"happens before"* relation, this value is meaningless.  And even in the context of the *"happens before"* relation, we must have at least two events in order to compare their Lamport Clock values.

In other words, Lamport Clocks mean nothing in themselves, but are consistent with causality.

### Assigning Lamport Clocks to Events

When assigning a value to a Lamport Clock, we need first to make a defining decision, and then follow a simple set of rules:

1. First, decide what constitutes *"an event"*. The outcome of this decision then defines what our particular Lamport Clock will count.
    In this particular case, we decide that receiving a message ***is*** counted as an event.  (Some systems choose not to count *"message receives"* as events).
1. Every process has an integer counter, initially set to 0
1. On every event, the process increments its counter by 1
1. When a process sends a message, the current Lamport Clock value is included as metadata sent with the message payload
1. When receiving a message, the receiving process sets its Lamport Clock using the formula
    `max(local counter, msg counter) + 1`

If we decide that a *"message receive"* is not counted as an event, then the above formula does not need to include the `+ 1`.

### Worked Example

We can see how this formula is applied in the following sequence of message send/receive events:

We have three processes `A`, `B` and `C` and the Lamport Clock values at the top of the process line indicate the state of the clock ***before*** the message send/receive event, and the Lamport Clock values at the bottom of the process line indicate the state of the clock ***after*** the send/receive event has been processed.

![Lamport Clock Message Send 1](./img/L4%20LC%20Msg%20Send%201.png)

![Lamport Clock Message Send 1](./img/L4%20LC%20Msg%20Send%202.png)

![Lamport Clock Message Send 1](./img/L4%20LC%20Msg%20Send%203.png)

As you can see, the value of each process' Lamport Clock increases monotonically (that is, the value only ever stays the same, or gets bigger &mdash; they can never get smaller!)

## Reasoning About Lamport Clock Values

We know that if `A` happens before `B` (`A -> B`) then we also know that `A`'s Lamport Clock value will be smaller than `B`'s Lamport Clock value (`LC(A) < LC(B)`).

But can we apply this logic the other way around?  If we know that `LC(A) < LC(B)` then does this prove that `A -> B`?

Actually, no it doesn't.  Consider this situation:

![Lamport Clock Message Send 1](./img/L4%20LC%20Msg%20Send%204.png)

![Lamport Clock Message Send 1](./img/L4%20LC%20Msg%20Send%205.png)

![Lamport Clock Message Send 1](./img/L4%20LC%20Msg%20Send%206.png)


Let's compare the Lamport Clock values of processes `A` and `B`

```
  LC(A) = 1
  LB(B) = 4
```

Since `LC(A) < LC(B)` does this prove that `E1 -> E2`?

Absolutely not!

Why?  Because we have no way to connect event `E1` with event `E2`.  These two events do not sit in the same process, neither is there a sequence of message send/receive events that allows us to draw a continuous line between them.  So, in this case, we are unable to use the ***happens before*** relation to define any causal relation between events `E1` and `E2`.  All we can say is that `E1` is independent of `E2`, or `E1 || E2`.

So, in plain language:

> If we are unable to trace an unbroken connection between two events, then we are unable to establish a causal relation between those events

Or to use fancier, academic language:

> Causality requires graph reachability in spacetime

So, in summary, when we reason about Lamport Clock values, if we know that `A -> B`, then we can be sure that `LC(A) < LC(B)`.  In other words:

> Lamport Clocks are consistent with causality

However, simply knowing that `LC(A) < LC(B)` does not prove `A -> B`; this is because:

> Lamport Clocks do not characterise (or establish) causality

The above example is derived from the ["Holy Grail"](./papers/holygrail.pdf) paper by Reinhard Schwarz and Friedemann Mattern.


### So, What Are Lamport Clocks Good For?

***Q:***&nbsp;&nbsp; Can we use a Lamport Clock to tell us the time of day?
***A:***&nbsp;&nbsp; Nope

***Q:***&nbsp;&nbsp; Can we use a Lamport Clock to measure the time interval between two events?
***A:***&nbsp;&nbsp; Nope

***Q:***&nbsp;&nbsp; So what are they good for?
***A:***&nbsp;&nbsp; A Lamport Clock is designed to help establish event ordering in terms of the *happens before* relation

Even though Lamport Clocks cannot characterise causality, they are still very useful because they define the logical implication: `if A -> B then LC(A) < LB(B)`

All logical implications are constructed from a premise (`A -> B`) stated in the form of a question, and a conclusion (`LC(A) < LB(B)`) that can be reached if the answer to the question is true.

For any logical implication, we can also take its contra-positive.  Thus, if `P => Q` then the contra-positive states that `¬Q => ¬P`

So, in the case of the "happens before" relation

`if A -> B then LC(A) < LB(B)`

The contra-positive states

`if ¬(LC(A) < LB(B)) then ¬(A -> B)`

The contra-positive states that if the Lamport Clock of `A` is not less than the Lamport Clock of `B`, then `A` cannot have happened before `B`.  This turns out to be really valuable in debugging because if we know that event `A` ***did not*** happen before event `B`, then we can say with complete certainty that whatever consequences were created by event `A`, they could not have contributed to the earlier problem experienced during event `B`.


## Summary

Lamport Clocks are good for certain aspects of determining causality, but they do leave us with indeterminate situations.  This is because a Lamport Clock is consistent with causality but does not characterise it.

In order to remove this indeterminacy, we need a different type of clock, called a Vector Clock.


---

| Previous | Next
|---|---
| [Lecture 3](./Lecture%203.md) | [Lecture 5](./Lecture%205.md)


# Distributed Systems Lecture 5

## Lecture Given by [Lindsey Kuper](https://users.soe.ucsc.edu/~lkuper/) on April 8<sup>th</sup>, 2020 via [YouTube](https://www.youtube.com/watch?v=zuxA6f-XIAc)

| Previous | Next
|---|---
| [Lecture 4](./Lecture%204.md) | [Lecture 6](./Lecture%206.md)



## Recap of Lamport Clocks

Lamport Clocks are consistent with causality, but do not characterise (or establish) it.

If `A -> B` then this implies that `LC(A) < LC(B)`

However, this implication is not reversable:

If `LC(A) < LC(B)` then it does ***not*** imply `A -> B`


## Vector Clocks

Invented independently by Friedemann Mattern and Colin Fidge.  Both men wrote papers about this subject in 1988.

> Addendum
>
> Subsequent investigation by Lindsey Kuper has uncovered that without using the name *"vector clock"*, the concept was already being used by Rivka Ladin and Barbara Liskov in 1986.  See [lecture 23](https://github.com/ChrisWhealy/DistributedSystemNotes/blob/master/Lecture%2023.md#ladin--liskovs-paper-highly-available-distributed-services-and-fault-tolerant-distributed-garbage-collection) for details.

For Vector Clocks however, this relation ***is*** reversable:

`A -> B <==> LC(A) < LC(B)`

A Lamport Clock is just a single integer, but a Vector Clock is a sequence of integers. (The word *"vector"* is being used here in the programming sense, not in the sense of a magnitude and direction)

### Implementing a Vector Clock

There are two pre-conditions that must be fulfilled before you can implement a Vector Clock:

1. You must know upfront how many processes make up your system
1. All the processes must agree the order in which the clock values will occur within the vector

In this case, we know that we have three processes `Alice`, `Bob` and `Carol`, and that the order of values in the vector will be sorted alphabetically by process name.

So, each process will create its own copy of the vector clock with an initial value of `[0,0,0]` for `Alice`, `Bob` and `Carol` respectively.

The Vector Clock is then managed by applying the following rules:

1. Every process maintains a vector of integers initialised to `0` - one for each process with which we wish to communicate

1. On every event, a process increments its own position in the vector clock: this also includes internal events that do not cause messages to be sent or received

1. When sending a message, each process includes the current state of its clock as metadata with the message payload

1. When receiving a message, each process updates its own position in the vector clock using the rule `max(VC(self),VC(msg))`


If, at some point in time, the state of the vector clock in process `Alice` becomes `[17,0,0]`, then this means that as far as `Alice` is concerned, it has recorded 17 events, whereas it thinks that processes `Bob` and `Carol` have not recorded any events yet.



### Calculating the `max` of Two Vector Clocks

But how do we take the `max` of two vectors?

The notion of `max` we're going to use here is a per-element comparison (a.k.a. a pointwise maximum)

For example, if my VC is `[1,12,4]` and I receive the VC `[7,0,2]`, the pointwise maximum would be `[7,12,4]`

### Applying the `<` Operator on Two Vectors

What does `<` mean in the context of two vectors?

It means that when a pointwise comparison is made of the values in vector clocks `VC(A)` and `VC(B)`, at least one value in `VC(A)` is less than the corresponding value in `VC(B)` and no value in `VC(A)` is greater than the corresponding value in `VC(B)`.

> It is assumed here that `VC(A)` and `VC(B)` are actually comparable.  This means that both vector clocks must refer to the same set of clock values listed in the same order.

This comparison can be performed using the `≤` operator as long as we first reject the case where `VC(A) == VC(B)`.  To put that more algorithmically, the following condition must be true:

<pre>
   VC(A) !== VC(B)
&& VC(A).length == VC(B).length
&& for each element at position i, VC(A)<sub>i</sub> ≤ VC(B)<sub>i</sub>
</pre>


### But Is This Comparison Enough to Characterise Causality?

Consider two Vector Clocks `VC(A) = [2,2,0]` and `VC(B) = [1,2,3]`

Is `VC(A) < VC(B)`?

So, taking a pointwise comparison of each element gives:

| Index | <code>VC(A)<sub>i</sub> ≤ VC(B)<sub>i</sub></code> | Outcome
|---|---|---
| `0` | `2 ≤ 1` | `false`
| `1` | `2 ≤ 2` | `true`
| `2` | `0 ≤ 3` | `true`

The overall result is then calculated by `AND`ing all the outcomes together:

`false && true && true = false`

So, we can conclude that `VC(A)` is ***not*** less than `VC(B)`.

Ok, let’s do this comparison the other way around.

Is `VC(B) < VC(A)`?

Again, we perform a pointwise comparison of each element gives:

| Index | <code>VC(B)<sub>i</sub> ≤ VC(A)<sub>i</sub></code> | Outcome
|---|---|---
| `0` | `1 ≤ 2` | `true`
| `1` | `2 ≤ 2` | `true`
| `2` | `3 ≤ 0` | `false`

The overall result is still `false` because `true && true && false = false`

Since `VC(B)` is ***not*** less than `VC(A)` and `VC(A)` is ***not*** less than `VC(B)`, we are left in an indeterminate state.  All we can say about the events represented by these two vector clocks is that they are concurrent, independent or causally unrelated (these three terms are synonyms).

I.E. `A || B`


## Worked Example

Let's see how the vector clocks in three processes (`Alice`, `Bob` and `Carol`) are processed as messages are sent and received:

![Vector Clocks example 1](./img/L5%20VC%20Clocks%201.png)
![Vector Clocks example 2](./img/L5%20VC%20Clocks%202.png)
![Vector Clocks example 3](./img/L5%20VC%20Clocks%203.png)
![Vector Clocks example 4](./img/L5%20VC%20Clocks%204.png)
![Vector Clocks example 5](./img/L5%20VC%20Clocks%205.png)
![Vector Clocks example 6](./img/L5%20VC%20Clocks%206.png)
![Vector Clocks example 7](./img/L5%20VC%20Clocks%207.png)

After these messages have been sent, we can see the history of how the vector clocks in each process changed over time.

![Vector Clocks example 8](./img/L5%20VC%20Clocks%208.png)


## Determining the Causal History of an Event

If we choose a particular event `A`, let's determine the events in `A`'s causal history.

![Causal History 1](./img/L5%20Causal%20History%201.png)

`A` was an event that took place within process `Bob` and by looking back at `Bob`'s other events, we can see one sequence of events:

![Causal History 2](./img/L5%20Causal%20History%202.png)

Also, by following the messages that led up to event `A`, we can see another sequence of events:

![Causal History 3](./img/L5%20Causal%20History%203.png)

What is common here is that:

1. Event `A` has ***graph reachability in spacetime*** from all the events in its causal history.
    That is, without lifting the pen from the paper or going backwards in time, we can connect any event in `A`'s past with `A`.
1. Working backwards from `A`, we can see that all the vector clock values in its causal history satisfy the ***happens before*** relation: that is, all preceding vector clock values are less than `A`'s vector clock value.

In addition to this, by looking at events that come after `A` (in other words, `A` is in the causal history of some future event), we can see that all such vector clock values are larger than `A`'s.

### Are the Vector Clocks of All Events Comparable?

Consider events `A` and `B`.  Can their vector clock values be related using the ***happens before*** relation?

![Causal History 4](./img/L5%20Causal%20History%204.png)

In order for this relation to be satisfied, the vector clock of one event must be less than the vector clock of the other event (in a pointwise sense).  But in this case, this is clearly not true:

```
VC(A) = [2,4,1]
VC(B) = [0,3,2]

[2,4,1] < [0,3,2] = false
[0,3,2] < [2,4,1] = false
```

Neither vector clock is larger or smaller than the other; therefore, all we can say about these two events is that they are independent, concurrent or causally unrelated, or `A || B`.

This does however mean that we can easily tell a computer how to determine if two events are causally related.  All we have to do is compare the vector clock values of these two events.  If we can determine that one is less than the other, then we know for certain that the event with the smaller vector clock value occurred in the causal history of the event with the larger vector clock value.

If, on the other hand, the ***less than*** relation cannot be satisfied, then we can be certain that the two events are causally unrelated.


## Protocols

The non-rigorous definition of a protocol is that it is an agreed upon set of rules that computers use for communicating with each other.

Let's take a simple example:

One process sends the message `Hi, how are you?` to another process.  According to our simple protocol, when a process receives this specific message, it is required to send the response `Good, thanks`

There is nothing in our protocol however that states which process is to send the first message, or what should happen after the `Good, thanks` message has been received.

The following two diagrams are both valid runs of our protocol:

![Protocol 1](./img/L5%20Protocol%201.png)

![Protocol 2](./img/L5%20Protocol%202.png)

What about this?

![Protocol 3](./img/L5%20Protocol%203.png)

Nope, this is not allowed because our protocol states that the message `Good, thanks` should only be sent in response to the receipt of message `Hi, how are you?`.  Therefore, sending such an unsolicited message constitutes a protocol violation.

### So How Long Did the Message Exchange Take?

What about this - is this a protocol violation?

![Protocol 4](./img/L5%20Protocol%204.png)

Hmmm, it's hard to tell.  Maybe the protocol is running correctly and we're simply looking at a particular point in time that does not give us the full story.

The point here is that a Lamport Diagram can only represent logical time - that is, it describes the order in which a sequence of events occurred, but it cannot give us any idea about how much real-world time elapsed between those events.

But considering that a Logical Clock is only concerned with the ordering of events, it is not surprising that the following two event sequences appear to be identical:

![Protocol 5](./img/L5%20Protocol%205.png)

### Complete Protocol Representation?

***Q:***&nbsp;&nbsp; Is it possible to use a Lamport Diagram to give us a complete representation of all the possible message exchanges in a given protocol?
***A:***&nbsp;&nbsp; No!

It turns out that there are infinitely many different Lamport Diagrams that all represent valid runs of a protocol.

The point here is that a Lamport Diagram is good for representing a ***specific*** run of a protocol, but it cannot represent ***all possible*** runs of that protocol, because there will be infinitely many.

Lamport Diagrams are also good for representing protocol violations - for instance, in the diagram above, `Alice` sent the message `Good, thanks` to `Bob` without `Bob` first sending the message `Hi, how are you?`.

### Correctness Properties and Their Violation

When discussing properties of a system that we want to be true, one way to talk about the correctness of such properties is to draw a diagram that represents its violation.

For instance, consider the order in which messages are sent and received.

### Important Terminology

In distributed systems, messages are not only sent and received, but they are also ***delivered***.

Hmmmm, it sounds like there is some highly specific meaning attached to the word ***deliver***...  Yes, there is.

***Sending*** and ***receiving*** can be understood quite intuitively, but in the context of distributed systems, the concept of ***message delivery*** has a highly specific meaning:

* ***Sending***
    The explicit act of causing a message to be transmitted.
    The sending process has complete control over when or even if a message is sent; therefore, sending a message is entirely ***active***.
* ***Receiving***
    An action that happens when a message arrives.
    The receiving process has no control over when or even if a message arrives &mdash; they just show up randomly... or not.  Therefore, from the perspective of the receiving process, receiving a message is entirely ***passive***.
* ***Delivery***
    The purpose of the term ***Delivery*** is to distinguish the passive act of receiving a message from the active choice to start processing the contents of that message. You can't decide when you're going to receive a message, but you can decide when and if to process its contents; therefore, although receiving a message is passive, the choice to deliver a message is entirely ***active***.
    For example, by placing a received message into a queue, a process can defer message delivery until some additional set of conditions becomes true.

### FIFO (or Ordered) Delivery

If a process sends message `M2` after message `M1`, the receiving process must deliver `M1` first, followed by `M2`.

We can represent a protocol violation such as ***FIFO anomaly*** using the following diagram.

![FIFO Anomaly](./img/L5%20FIFO%20Anomaly.png)

This is an example of where a diagram provides a very useful way to represent the violation of some correctness property of a protocol.


---

| Previous | Next
|---|---
| [Lecture 4](./Lecture%204.md) | [Lecture 6](./Lecture%206.md)


# Distributed Systems Lecture 6

## Lecture Given by [Lindsey Kuper](https://users.soe.ucsc.edu/~lkuper/) on April 10<sup>th</sup>, 2020 via [YouTube](https://www.youtube.com/watch?v=UoIiwJ2G2fc)

| Previous | Next
|---|---
| [Lecture 5](./Lecture%205.md) | [Lecture 7](./Lecture%207.md)

## Recap

### Difference Between Receiving and Delivering

* ***Sending*** a message is something you do actively
* ***Receiving*** a message is something that happens to you passively
* ***Delivering*** a message is something you actively do after receiving a message

***Delivery*** is the conscious decision to process a received message.

But why would you want to queue a message before processing it?  Typically, because messages need to be processed in the correct order, which could well be different from the order in which they were received.

### FIFO Delivery

If a process sends message `M2` after `M1`, then any process delivering ***both*** of these messages must deliver `M1` first then `M2`.  Failure to do this constitutes a protocol violation as described in the previous lecture as a "FIFO anomaly"

![FIFO violation or anomaly](./img/L5%20FIFO%20Anomaly.png)

In this case, irrespective of the order in which process `Bob` received messages `{m1}` and `{m2}`, it should always ***deliver*** message `{m1}` first, followed by message `{m2}`.

In the case that `Bob` does not receive one (or either) of these messages, then no FIFO violation could have occurred, because here we are concerned with message ***delivery***, not message ***receipt***.


### FIFO Delivery Implementation

In real-life, it is unusual to have to implement FIFO delivery yourself because most distributed systems communicate using TCP which already implements FIFO packet delivery.

## Causal Delivery

There are different ways of phrasing this, but one way is to say:

> If `m1`'s send happens before `m2`'s send, then `m1`'s delivery must happen before `m2`'s delivery

Here's an example of such a violation

![Causal violation](./img/L6%20Causal%20Violation.png)

In process <code>P<sub>1</sub></code>,  event `A` happens in the causal history of event `B`; therefore, any messages sent from <code>P<sub>1</sub></code> to <code>P<sub>2</sub></code> should be processed in the same causal order as the events that generated them.

But now, let's go back to the "Bob smells" example used in [lecture 3](./Lecture%203.md)

![Causal Anomaly](./img/L3%20Causal%20Anomaly.png)

***Q:***&nbsp;&nbsp; Is this a FIFO violation?
***A:***&nbsp;&nbsp; No (but only in a vacuous sense...)

The reason is that a FIFO violation only occurs when two messages ***from the same originating process*** are delivered out of order by the receiving process.

In the above diagram, there is no single process that sends ***two*** distinct messages to the same receiving process.  Here:

* `Alice` sends a single message to `Bob`
* `Alice` sends a single message to `Carol`
* `Bob` sends a single message to `Alice`
* `Bob` sends a single message to `Carol`
* `Carol` is confused...

However, this scenario is still a causal anomaly.  In general, at least three communicating processes are required to create a causal anomaly.

### Can a Message be Sent to Multiple Destinations?

Yes, this is what's known as a broadcast message - I.E. a single send event that broadcasts a message to multiple (possibly all) participants in a system.  The idea of broadcast messages is something that will be dealt with later.

## Totally-Ordered Delivery

This is another correctness property.

> If a process delivers message `M1` followed by `M2`, then ***all*** processes delivering both `M1` and `M2` must deliver `M1` first followed by `M2`.

Let's say we have two client processes `C1` and `C2` that each broadcast a message to two processes `R1` and `R2`.  In this scenario, processes `R1` and `R2` each maintain their own replica of some key/value store.

If processes `R1` and `R2` do not deliver the messages in the correct order, then we will encounter a violation that results in the replicas disagreeing with each other as to what the value of `x` should be.  In other words, this violation creates an inconsistency between data replicas.

![Total-Order Anomaly](./img/L6%20Total%20Order%20Anomaly.png)

This is known as a ***Total-Order Anomaly*** and is created when process `R1` delivers message `m1` followed by `m2`, but process `R2` delivers message `m2` followed by `m1`.

### Delivery Guarantees

Since we know that causal delivery also ensures FIFO delivery, we can start to arrange these delivery strategies in a hierarchy, with the weakest at the bottom.  Here, we will use the term `YOLO` to indicate the delivery guarantee that makes no guarantees!

![Delivery Hierarchy 1](./img/L6%20Delivery%20Hierarchy%201.png)

Where would Totally Ordered Delivery fit in to this scheme?

In fact, it would get its own branch because a FIFO anomaly is not necessarily an anomaly as far as Totally-Ordered Delivery is concerned.

We recall that a FIFO anomaly is the following:

![FIFO violation or anomaly](./img/L5%20FIFO%20Anomaly.png)

But since the definition of Totally-Ordered Delivery says that ***all*** processes delivering both `m1` and `m2` must do so in a consistent order, then the above FIFO anomaly is not an anomaly for  Totally-Ordered Delivery because there is only one receiving process, so the order in which that process delivers the messages is immaterial.  Thus, this scenario only vacuously conforms to a Totally-Ordered Delivery.

Conversely, Totally-Ordered Delivery violations are not necessarily FIFO violations.

![Delivery Hierarchy 2](./img/L6%20Delivery%20Hierarchy%202.png)

### What Does This Hierarchy Imply?

This hierarchy helps us understand what we can and cannot expect out of a particular delivery guarantee.  For instance, if we implement a system guaranteeing causal delivery, then in doing so, we would also be guaranteeing FIFO delivery, because FIFO delivery sits directly below Causal delivery in the hierarchy.  However, if we implemented a FIFO delivery system, we could make no guarantees about causal delivery.

Similarly, if the system implements Totally-Ordered Delivery, then this guarantee, in and of itself, cannot ensure either FIFO or Causal delivery.

Turning this argument around, we can also gain an understanding of what type of anomalies can occur.  For instance, if we have a FIFO anomaly, then this is also going to be a causal anomaly, but not necessarily a Totally-Ordered anomaly.


## Implementing Delivery Guarantees

### Implementing FIFO Delivery: Sequence Numbers

The rule here is that any process `P2` delivering messages from some other process `P1`, must do so in the order that `P1` sent those messages; which, due to variations in network latency, might well be different from the order in which those messages arrive at `P2`.

How then would we go about eliminating FIFO delivery anomalies?

One possibility is to use sequence numbers.  This is where all messages from a given sender are tagged with a sequence number and a sender id.  Each time a message is sent, the sender increments its sequence number.  On the receiver's side, all the messages from a given sender are added to a queue ordered by the sequence number.  When all the messages have arrived, the receiver can then deliver them in the correct order.

In this case, sequence numbers do not need to be unique across all the processes, because each message is also qualified with a sender id; therefore, it is the combination of the sender id and the sequence number that allows the receiver to discriminate who sent which message and in what order.

***Problems with Sequence Numbers***

What happens if a message is lost?

`Alice` sends messages `m1` and `m2` to `Bob` who delivers them correctly.  However, without her knowing, `Alice`'s message `m3` gets lost and never arrives at `Bob`.  Then `Alice` sends messages `m4` and `m5` which `Bob` receives; however, because `Bob` is still waiting for the message with sequence number `3` to arrive, `Bob` will add any subsequent messages to his queue which may end up waiting forever for the lost message to be delivered.

![Naïve Sequence numbering](./img/L6%20Naive%20Seq%20Nos.png)

Consequently, in a network where message delivery is unreliable, a naïve sequence number strategy like this will break as soon as message delivery fails for some reason.

Strategies to mitigate these problems could include:

* Buffering out of sequence messages for a pre-determined period of time, hoping that the late message arrives either before the message buffer fills or the pre-determined timeout expires
* Processing out of sequence messages on the assumption that the intervening message is lost.  If this assumption turns out to be false and the message delivery was simply delayed, then the late message would have to be dropped

Neither of the above strategies are very good in that they tend to create more problems than they solve...

### Vacuous FIFO Delivery

Now consider this situation.  Are the conditions of FIFO delivery satisfied?

![Vacuous FIFO Delivery](./img/L6%20Vacuous%20FIFO%20Delivery.png)

Yes, but only in a vacuous sense.  Due to the fact that `Bob` drops all the messages he receives, zero messages are delivered; therefore, the conditions of FIFO delivery are vacuously satisfied.

### Implementing FIFO Delivery: Acknowledgments

In this approach, upon receipt of a message, every receiver must send a *"message received"* acknowledgment (such as `ack`) back to the sender.

So, when `Alice` sends a message to `Bob`, neither `Alice` nor `Bob` need concern themselves with sequence numbers.  However, this approach has several distinct drawbacks:

* Communication now becomes sequential.  `Alice` cannot send `m2` to `Bob` until she has received an `ack` from `Bob` that he has received `m1`
* Increases the volume of network traffic
* We are still dependent upon a network that can guarantee reliable message delivery

One way of making this approach to communication more efficient is to gather messages into batches, thus decreasing the granularity of communication.

## Using Vector Clocks to Prevent Causal Anomalies

Let’s look again at the ***Causal Anomaly*** situation:

![Causal Anomaly](./img/L3%20Causal%20Anomaly.png)

The problem here is that `Carol` delivers the message she receives from `Bob` out of causal order, thus resulting in confusion...

Here, we can use vector clocks to solve causal anomalies.

In the [previous lecture](./Lecture%205.md), we looked at using vector clocks to count both message-send and -receive events; but in order to ensure Causal Delivery, it turns out that we only need to count message send events.

![Ensure Casual Delivery 1](./img/L6%20Ensure%20Casual%20Delivery%201.png)

Before sending the message, `Alice` updates her vector clock to `[1,0,0]`

### What Should Bob Do?

`Bob` receives the message from `Alice`.

***Q:***&nbsp;&nbsp; Should he deliver it?
***A:***&nbsp;&nbsp; Yes, he has no reason not to.

`Bob` delivers the message and discovers that it is not to his liking.  But, since `Bob` has the emotional maturity of an eight-year-old, he fails to realise that soap and water will work far better than trading insults; so, he resorts to sending his own broadcast message back to `Alice` and `Carol`

In delivering this message, `Bob` examines the vector clock of the incoming message and discovers that its less than his, but only by the counter in `Alice`'s position.  This is to be expected, since the message came from `Alice`.  He therefore uses the received vector clock to update his own vector clock, and then increments his position in the vector clock.

Since a broadcast message is treated as a single send event to multiple recipients, the same vector clock value of `[1,1,0]` is sent as part of the messages to both `Alice` and `Carol`.

![Ensure Casual Delivery 2](./img/L6%20Ensure%20Casual%20Delivery%202.png)

### What Should Alice Do?

The message now arrives at `Alice`.

***Q:***&nbsp;&nbsp; Should she deliver it?
***A:***&nbsp;&nbsp; Yes, she has no reason not to.

`Alice`'s vector clock is `[1,0,0]` and the incoming vector clock on the message differs only by `1` in `Bob`'s position.  So, we can conclude that only one event has taken place since our last message send event, and that event happened in process `Bob` from whom we received this message.

### But What Should Carol Do?

`Bob`'s message also arrives at Carol with vector clock `[1,1,0]`, but earlier than `Alice`'s original message.

***Q:***&nbsp;&nbsp; Should she deliver it?
***A:***&nbsp;&nbsp; No &mdash; look at the vector clock values!

The reason is that compared to `Carol`'s vector clock (which is still set to `[0,0,0]`), the vector clock on the incoming message is too big.

It’s fine for `Bob`'s position to be set to `1` because this is one bigger than `Carol`'s vector clock position for `Bob` and the message came from `Bob`.

But there's a `1` in `Alice`'s vector clock position.

***Q:***&nbsp;&nbsp; Hmmmm, that's odd.  Where did that come from?
***A:***&nbsp;&nbsp; The value comes from the fact that this message is the response to some event that has taken place in `Alice`, but that ***Carol doesn't yet know about***.

In other words, as far as `Carol` is concerned, this is a ***message from the future*** that has arrived too early and must therefore be buffered.

Finally, `Alice`'s original `"Bob smells"` message arrives at `Carol`.  `Carol` now examines this message's vector clock and discovers that it has the expected value of `[1,0,0]`; therefore, it is fine to deliver this message first.

Once this out-of-sequence message has been delivered, the buffered message can be delivered because `Carol` has now caught up with the event that took place in `Alice`.

`Carol` is no longer confused...

---

| Previous | Next
|---|---
| [Lecture 5](./Lecture%205.md) | [Lecture 7](./Lecture%207.md)

# Distributed Systems Lecture 7

## Lecture Given by [Lindsey Kuper](https://users.soe.ucsc.edu/~lkuper/) on April 13<sup>th</sup>, 2020 via [YouTube](https://www.youtube.com/watch?v=uJ62T48ZdBs)

| Previous | Next
|---|---
| [Lecture 6](./Lecture%206.md) | [Lecture 8](./Lecture%208.md)


## Causal Broadcast Using Vector Clocks

Here's the classic causal anomaly again.

![Causal Anomaly](./img/L3%20Causal%20Anomaly.png)

The problem here is that the message `Carol` receives first is also delivered first.   The anomaly occurs because of out of order ***delivery***, not out of order ***receipt***.

The use of vector clocks helps eliminate the problem of causal anomalies because by comparing the vector clock value on the incoming message with its own vector clock, the receiver can decide whether or not the message should be delivered.

![Causal Broadcast 1](./img/L7%20Causal%20Broadcast%201.png)

In this case, when `Bob` receives `Alice`'s message, its fine for him to deliver it because `Bob`'s vector clock of `[0,0,0]` differs only by one from the vector clock of the incoming message, and this difference is in `Alice`'s position.  Therefore, since it came from `Alice`, it is correct to conclude that this message is the next event in both `Alice` and `Bob`'s causal history.

`Bob` then sends out his rude broadcast message in reply to `Alice`, but `Carol` receives this reply before the original message from `Alice`.

![Causal Broadcast 2](./img/L7%20Causal%20Broadcast%202.png)

By comparing the vector clock value on `Bob`'s message with her own vector clock, `Carol` can determine that this message should be queued, and not delivered yet. `Carol` does this by noticing that `Bob`'s vector clock position is one greater than her vector clock position for him.  Since this message came from `Bob`, this difference is expected.

Ok, so far so good.

However, the message vector clock also has a `1` in `Alice`'s position &mdash; and this is not expected.

Remember that in this scenario, our vector clocks only count message-send events; so when `Carol` sees a `1` in `Alice`'s position, this means that some message send event has taken place in `Alice` that `Carol` does not yet know about (probably because the messages have been received out of order).  Hence, `Carol` can correctly infer that this is a ***message from the future*** and should therefore be queued.


When `Alice`'s delayed message finally arrives at `Carol`, this message carries a vector clock value of `[1,0,0]` which is what `Carol` expects, so this message can be correctly delivered.

![Causal Broadcast 3](./img/L7%20Causal%20Broadcast%203.png)

Now `Carol` examines her message queue and discovers that the message with vector clock `[1,1,0]` can now be delivered, because all the preceding messages in her causal history have been delivered in the correct order.

![Causal Broadcast 4](./img/L7%20Causal%20Broadcast%204.png)

## Rules for Causal Broadcast

1. Before sending a message to process `P2`, process `P1` records this send event by incrementing its own position in its local vector clock.  The updated vector clock is then sent with the message as metadata.
1. At such time as `P2` delivers `P1`'s message, `P2` increments the `P1` clock value in its own local vector clock (I.E. it records the delivery of `P1`'s message)
1. Process `P2` should only deliver `P1`'s message if the clock value received with that message conforms to the following two rules:

    * The clock value for process `P1` in the message must be exactly one bigger than the clock value for process `P1` in the receiving process `P2`.  Or written more algebraically:

        <code>VC<sub>msg</sub>[P1] = VC<sub>P2</sub>[P1] + 1</code>

        ***and***

    * The message clock values for all other positions must be less than or equal to the corresponding positions in `P2`'s vector clock.  Or, for all positions `k` in the vector clock where `(k ≠ P1)`:

        <code>VC<sub>msg</sub>[P<sub>k</sub>] ≤ VC<sub>P2</sub>[P<sub>k</sub>]</code>

### What Do These Rules Mean?

There are two important things to remember here:

1. We are only incrementing vector clock values on message-***send*** events, not message-receive events.
    The value in each vector clock position is simply a count of the number of messages that process has sent so far.
1. These rules only apply to ***broadcast*** messages, not point-to-point messages!
    This means that every process in the system will (eventually) receive every message sent by every other process.

***Rule 1:***&nbsp;&nbsp;<code>VC<sub>msg</sub>[P1] = VC<sub>P2</sub>[P1] + 1</code>

Knowing this, we can understand the above rule to mean that in order to avoid creating a causal anomaly (I.E. by delivering a message out of order),  the receiver's local clock value for the sender must be exactly one smaller than the sender's clock value received in the message.

***Rule 2:***&nbsp;&nbsp;<code>VC<sub>msg</sub>[P<sub>k</sub>] ≤ VC<sub>P2</sub>[P<sub>k</sub>], (k ≠ P1)</code>

The second rule means that the number of message-sends performed by all the other processes in the system (I.E. the vector clock values) must be no bigger than the values recorded in the receiver's local clock.  In other words, the receiver keeps a complete record of all broadcast messages sent in the system; no message-send events are missing.

This is the rule that would be violated if `Carol` tried to deliver `Bob`'s rude "Up yours!" ***message from the future*** at the time it was received.

The vector clock on the message sent from `Bob` to `Carol` is `[1,1,0]`, but `Carol`'s vector clock is `[0,0,0]`.  The `1` in `Bob`'s position is correct because he is sending the message, and it is one greater than `Carol`'s local value, but the `1` in `Alice`'s position is a problem.  According to this, `Alice` has sent out a broadcast message, but `Carol` has no record of it &mdash; yet.

Since `1` is not ≤ `0`, `Carol` correctly concludes that this newly arrived message has been received out of order and therefore must be queued until such time as we receive the delayed message from `Alice`.

### Another Example

Here. `Alice` sends a broadcast message to `Bob` and `Carol` saying ***"I lost my wallet :-("***

![Causal Broadcast 5](./img/L7%20Causal%20Broadcast%205.png)

In the absence of any other messages, its fine for both `Bob` and `Carol` to deliver this message.

A little later, `Alice` finds her wallet and tells `Bob` and `Carol` about this happy event.  However, `Alice`'s message to `Carol` gets delayed.

![Causal Broadcast 6](./img/L7%20Causal%20Broadcast%206.png)

It’s fine for `Bob` to deliver this message because it came from `Alice` and is the next expected message from her.  `Bob` is very happy that `Alice` has found her wallet and sends out a broadcast message to both `Alice` and `Carol` saying how pleased he is.

Unfortunately, `Alice`'s original message doesn't reach `Carol` until after `Bob`'s response arrives.

![Causal Broadcast 7](./img/L7%20Causal%20Broadcast%207.png)

Fortunately, `Carol` recognises that `Bob`'s response is a ***message from the future***, and places it in her message queue.  Otherwise, she would think that `Bob` is a complete jerk because as far as `Carol` is concerned, `Alice` has just lost her wallet and `Bob` seems to be really happy about this!

![Causal Broadcast 8](./img/L7%20Causal%20Broadcast%208.png)

Only after `Carol` delivers the preceding message, does she then deliver the message that arrived too early.

## Can Vector Clocks Establish a Total Order on Messages?

Remember what a total order anomaly looks like:

![Total Order Anomaly](./img/L6%20Total%20Order%20Anomaly.png)

If we assign vector clocks to these send-events and then apply the rules of causal broadcast, we will discover that causal delivery cannot rule out total-order anomalies.

![Casual Delivery Cannot Prevent Total Order Anomaly](./img/L7%20TO%20Anomaly.png)

This is because, if we look back at the hierarchy of delivery guarantees, we can see that Total Order exists on its own branch from Casual and FIFO.

![Delivery Hierarchy](./img/L6%20Delivery%20Hierarchy%202.png)

So how can we rule out causal anomalies and, at the same time, ensure total order?

Well, if we want to maintain both causal order ***and*** total order, then we will need something more than vector clocks and the causal broadcast algorithm we have just described.

In general, it’s pretty annoying to have to enforce total order, so it’s much easier not to enforce it unless you really have to.

## Ways That Potential Causality is Used in Distributed Systems

The ***happens before*** relation is an example of potential causality.

We have already spoken of two of them:

- Ordering of events can be determined after the fact by assigning vector clocks (useful for debugging)
- Causal ordering of events as they happen (E.G. Using vector clocks to achieve causal broadcast)

These techniques provide ordering guarantees that prevent causal anomalies.

## Consistent Global Snapshot

Another thing we have not mentioned yet is something called ***Consistent Global Snapshot***.  This is related to the first point above and is a way to obtain a picture of the global state of a distributed system.  However, this is far from trivial to implement because not only does every process in a system have its own state, every process also has its own idea of the state of every other process.

One thing we can say is that:

> If `A->B` and `B` is in the snapshot, then we should also expect to find `A` in the snapshot

So, the ***Consistent Global Snapshot*** is another important use of the *happens before* relation (or potential causality)

## How Do You Take a Global Snapshot of a Distributed System?

As has already been pointed out, in a distributed system, there really is no such things as an "observable" global state.  Each process has its own state that represents the sum total of activity in that process up until some particular point.  This includes the state of the process' internal memory.

So, we could lasso all the events and internal variables of a process and call that the state...

![Process State](./img/L7%20Process%20State.png)

But what about the state of all the other processes in the system?

One approach might be to use a global clock and inform every process that at a certain time of day (say `09:20`), they must all take a snapshot of themselves.  However, as we have already seen in [lecture 2](https://github.com/ChrisWhealy/DistributedSystemNotes/blob/master/Lecture%202.md#time-and-how-we-measure-it), this approach won't work reliably &mdash; not because a process can't take a selfie (so to speak), but because synchronising clocks between computers is a notoriously difficult task.

![Snapshot Anomaly Caused by Using a Wall clock](./img/L7%20Wallclock%20Snapshot%20Anomaly.png)

Uh oh! Now we have a problem.  Remember what we said above:

> If `A->B` and `B` is in the snapshot, then we should also expect to find `A` in the snapshot

From the diagram, we can see that the message-send event `E` in `P1` causes event `W` in `P2`.

Therefore `E(P1) -> W(P2)`

But since `P2`'s clock is running slightly slower than `P1`'s, the `{p1:snapshot}` message arrives at `P2` (causing event `W`) just ***before*** `P2`'s clock ticks over to `09:20`; therefore, as far as `P2` is concerned, event `W` should be included in the snapshot.

Now when we compare the data in `P1`'s snapshot with the data in `P2`'s snapshot, we are unable to explain the cause of event `W` &mdash; it just pops up out of nowhere because there's a gap in its causal history.  And all of this happens in spite of both processes thinking they took their snapshots at `09:20`.

As we can see, using a machine's time-of-day clock is an error-prone approach to taking consistent snapshots.

So, we need an algorithm that allows us to snapshot an entire system ***consistently***.

## The Chandy-Lamport Algorithm

We now introduce some new terminology:  ***Channels***.

A channel is simply a unidirectional communication path between two processes.

### Assumptions

As an aside, the success of the Chandy-Lamport algorithm relies entirely on the truth of the following assumptions:

1. A message is ***guaranteed*** to arrive at the recipient &mdash; eventually
1. All channels act as FIFO queues, thus making it impossible for two messages to arrive out of order (I.E. we can exclude the possibility of FIFO anomalies)
1. Processes don't crash! (The topic of process failure is dealt with later in [lecture 10](./Lecture%2010.md))

### Channel Naming Convention

Between any two processes `P1` and `P2`, two channels exist.  Communication from `P1` to `P2` passes along channel <code>C<sub>12</sub></code>, and communication in the other direction passes along channel <code>C<sub>21</sub></code>

![Channels 1](./img/L7%20Channels%201.png)

`P1` sends a message to `P2` at event `A` over channel <code>C<sub>12</sub></code>.  This is received by `P2` at event `B`.

`P2` then sends a message back to `P1` at event `C` over channel <code>C<sub>21</sub></code>, but since this message has not yet arrived at `P1`, it is said to be ***in the channel***.

In the diagram above, channel <code>C<sub>12</sub></code> is said to be empty because there are no messages currently in flight, and channel <code>C<sub>21</sub></code> contains one message.

### Applying the Chandy-Lamport Algorithm for Taking a Snapshot

In this case, process `P1` sends the first message, and therefore we will call it the ***initiator process***.

![Channels 2](./img/L7%20Channels%202.png)

In the above diagram

1. Process `P1` sends a message out at event `A` on its only channel <code>C<sub>12</sub></code>
1. `P1` then takes a snapshot of itself (`S1`) and immediately sends out a special message called a ***marker*** on all its channels.
     Sending a marker message is actually part of the snapshot algorithm itself and must be the first thing done after a process records its own state. The marker messages themselves do not form part of the snapshot.
1. Process `P1` then starts to record all the messages it receives on all of its incoming channels

So, what happens when a process receives a marker message?

There are two cases:

1. If this is the first marker this process has seen:
    * It takes a snapshot of itself
    * It marks the channel on which it received the marker message as empty
    * It sends a marker message out on all of its outgoing channels

1. If this process has already seen a marker message before:
    * It stops recording all incoming messages on that channel
    * It sets that channel's state to be the sum of the events that arrived whilst recording was active

So when `P2` receives the marker message from `P1`, it immediately records its state (`S2`), marks channel <code>C<sub>12</sub></code> as empty, and sends a marker out on all its channels (in this case, `P2` only has one channel)

![Channels 3](./img/L7%20Channels%203.png)

What does `P1` do when it sees `P2`'s marker message?

Well, has `P1` seen a marker message before?

Yes, it has.  By sending out the first marker message, `P1` is said to have seen a marker message.  So now `P1` stops recording on the incoming channel on which the marker message arrived.

Did `P1` record anything on this channel?

Let's say that it did.  Let's say that the message sent from `P2` at event `C` actually arrived at `P1` as event `D`.

![Channels 4](./img/L7%20Channels%204.png)

So, event `D` is now a recorded event and the snapshot is complete:

* We have recorded the state of `P1` in `S1`
* We have recorded the state of `P2` in `S2`
* We have recorded the incoming message event `D` in `P1`

So, the above snapshot forms a complete history of the events that occurred in these two processes; but what about the following two snapshots - do they make sense?

![Bad Snapshots](./img/L7%20Bad%20Snapshot.png)

But what about this?  Is this a legal snapshot?

![Good Snapshot](./img/L7%20Good%20Snapshot.png)

Yes, this is perfectly valid - it was just taken prior to event `C` in `P2` happening.

### Is This a Snapshot of the Entire System?

A snapshot of the entire system is derived by a separate process that goes around collecting all the individual process snapshots and stitching them together to form of overall global snapshot.

The Chandy-Lamport algorithm actually predates the invention of vector clocks.  It has been designed to ensure that the entire event history of each process in the system is recorded without any violation of the ***happens before*** relation.

---

| Previous | Next
|---|---
| [Lecture 6](./Lecture%206.md) | [Lecture 8](./Lecture%208.md)



# Distributed Systems Lecture 8

## Lecture Given by [Lindsey Kuper](https://users.soe.ucsc.edu/~lkuper/) on April 15<sup>th</sup>, 2020 via [YouTube](https://www.youtube.com/watch?v=x1BCZ351dJk)

| Previous | Next
|---|---
| [Lecture 7](./Lecture%207.md) | [Lecture 9](./Lecture%209.md)


## Rules of the Chandy-Lamport Algorithm

This is an example of a decentralised<sup id="a1">[1](#f1)</sup> algorithm that allows you to take a global snapshot of a running distributed system.

Any process can start the snapshot without either needing to be given a special designation or the need to announce that this action is about to take place.  The act of initiating a snapshot creates a cascade of marker messages throughout the entire system that cause all the processes to take a snapshot of themselves.


### The Initiator Process

* Records its own state
* Sends a marker message out on all its outgoing channels
* Starts recording messages arriving on ***all*** incoming channels

In this case, the initiator process is `P1`.

![Chandy-Lamport Snapshot 1](./img/L8%20CL%20Snapshot%201.png)

If process `P1` decides to initiate a snapshot, then the following sequence of events takes place:

* `P1` records its own state as `S1`
* Immediately after recording its own state, `P1` sends out marker messages on all its outgoing channels (only one in this case: channel <code>C<sub>12</sub></code>)
* `P1` starts recording any messages that might arrive on its incoming channels (again, only one in this case: channel <code>C<sub>21</sub></code>)

Notice that at the time `P1`'s snapshot happens, message `m` is currently ***in the channel*** from `P2` to `P1` (channel <code>C<sub>21</sub></code>).

### Processes Receiving a Marker Message

> ***IMPORTANT***
>
> ![A Marker FIFO Anomaly Cannot Happen](./img/L8%20Marker%20FIFO%20Anomaly.png)
>
> Due the fact that all channels behave as FIFO queues, we do not need to be concerned about the possibility of FIFO anomalies.  This system is designed such that marker messages cannot arrive ***before*** earlier message-send events in the originating process.
>
> None of what follows would work if we had not first eliminated the possibility of FIFO anomalies!

When a process receives a marker message, it can react in one of two different ways.  How it reacts depends on whether or not that process has already seen a marker message during this run of the global snapshot.

#### Nope, I Haven't Seen a Marker Message Before...

If this is the first time this process has seen a marker message, the receiver:

* Records its own state
* Flags the channel on which the marker message was received as ***empty***
* Sends out a marker message on each of its outgoing channels
* Starts recording incoming messages on all channels ***except*** the one on which it received the original marker message (now flagged as empty)

***Q:***&nbsp;&nbsp; During a snapshot, once a channel is marked as empty, what happens if you then receive a message on that channel?
***A:***&nbsp;&nbsp; Whilst the snapshot is running, messages received on channels marked as empty are ignored!

In the diagram below, since this is the first marker message `P2` has seen, it does the following:

* It records its own state as `S2`
* Flags channel <code>C<sub>12</sub></code> as empty
* Sends out a marker message on all its outgoing channels (in this case, only channel <code>C<sub>21</sub></code>)
* Normally, it would now start recording any messages that arrive on its other, incoming channels, but in this case, since its only incoming channel (<code>C<sub>12</sub></code>) has already been marked as empty, there is nothing to record

![Chandy-Lamport Snapshot 2](./img/L8%20CL%20Snapshot%202.png)

#### Yup, I've Already Seen a Marker Message...

However, if a process sends out a marker message, then we consider that process already to have "seen" a marker message.  So when the receiving process receives a marker message, it:

* Stops recording incoming messages on that channel
* Sets that channel's final state to be the sequence of all messages received whilst recording was active

Message `m` from `P2` (sent at event `C`) arrives on channel <code>C<sub>21</sub></code> as event `D` on process `P1`.  This message arrived ***before*** the marker message because channels always behave as FIFO queues.

Upon receiving this marker message, `P1` then:

* Stops recording on the marker message's channel (<code>C<sub>21</sub></code> in this case)
* The final state of channel <code>C<sub>21</sub></code> is set to the sequence of messages that arrived whilst recording was active

![Chandy-Lamport Snapshot 3](./img/L8%20CL%20Snapshot%203.png)

So, we now have a consistent snapshot of our entire system, which in this simple case, consists of four things:

1. The state of our two processes:
    * `P1`'s state recorded as `S1`
    * `P2`'s state recorded as `S2`
1. The state of all channels between those processes:
    * Channel <code>C<sub>12</sub></code> recorded by `P2` (Empty)
    * Channel <code>C<sub>21</sub></code> recorded by `P1` (Message `m`)


## The Chandy-Lamport Algorithm in a More Detailed Scenario

When a snapshot takes place, every process ends up sending out a marker message to every other process.  So, for a system containing `N` participating processes, `N * (N - 1)` marker messages will be sent.  This might seem inefficient as the number of messages rises quadratically with the number of participating processes, but unfortunately, there is no better approach.

As stated in the previous lecture, the success of the Chandy-Lamport algorithm relies entirely on the truth of the following assumptions:

1. Eventual message delivery is guaranteed, thus making delivery failure impossible
1. All channels act as FIFO queues, thus eliminating the possibility of messages being delivered out of order (FIFO anomalies)
1. Processes don't crash! (See [lecture 10](./Lecture%2010.md))

### A Worked Example

In this example, we have three communicating processes `P1`, `P2` and `P3` in our system, and we want to take a snapshot.

Process `P1` acts as the initiator; so it follows the above steps:

* It records its own state as <code>S<sub>1</sub></code>
* It sends out two marker messages; one to `P2` and one to `P3` - but notice that the arrival of the marker message at `P2` is delayed.
    This turns out not to be a problem.
* `P1` starts recording on both its incoming channels <code>C<sub>21</sub></code> and <code>C<sub>31</sub></code>

![Chandy-Lamport Example Step 1](./img/L8%20Snapshot%20Ex%201.png)

Next, `P3` receives the marker message from `P1`.  Since this is the first marker message it has received:

* It records its own state as `S3`
* Marks the channel on which it received the marker message (<code>C<sub>13</sub></code>) as empty
* Sends out marker messages on all its outgoing channels
* Starts recording on its other incoming channel (<code>C<sub>23</sub></code>)

![Chandy-Lamport Example Step 2](./img/L8%20Snapshot%20Ex%202.png)

Looking at `P3`'s marker message that now arrives at `P1`, since `P1` initiated the snapshot process, this not the first marker it has seen, so `P1`:

* Stops recording incoming messages on that channel (<code>C<sub>31</sub></code>)
* Sets that channel's final state to be the sequence of all messages received whilst recording was active - which is none - so the channel state of <code>C<sub>31</sub></code> is `{}`.

![Chandy-Lamport Example Step 3](./img/L8%20Snapshot%20Ex%203.png)

Now looking at the other marker message from `P3` to `P2`. This is the first marker `P2` has seen, so it:

* It records its own state as `S2`
* Marks the channel on which it received the marker message (<code>C<sub>32</sub></code>) as empty
* Sends out marker messages on all its outgoing channels
* Starts recording on its other incoming channel (<code>C<sub>12</sub></code>)

![Chandy-Lamport Example Step 4](./img/L8%20Snapshot%20Ex%204.png)

Eventually, the initial marker message from `P1` arrives at `P2`.  This is the second marker `P2` has seen, so it:

* Stops recording incoming messages on that channel (<code>C<sub>12</sub></code>)
* Sets that channel's final state to be the sequence of all messages received whilst recording was active - which is none - so the channel state of <code>C<sub>12</sub></code> is `{}`.

![Chandy-Lamport Example Step 5](./img/L8%20Snapshot%20Ex%205.png)

`P2`'s marker message now arrives at `P1`.  This is not the first marker `P1` has seen, so it:

* Stops recording incoming messages on that channel (<code>C<sub>21</sub></code>)
* Sets that channel's final state to be the sequence of all messages received whilst recording was active - which in this case is the message `m3` sent at event `H` in `P2` to event `D` in `P1` - so the channel state of <code>C<sub>12</sub></code> is `{m3}`.

![Chandy-Lamport Example Step 6](./img/L8%20Snapshot%20Ex%206.png)

Lastly, the marker message from `P2` arrives at `P3`.  This is not the first marker `P3` has seen, so it:

* Stops recording incoming messages on that channel (<code>C<sub>23</sub></code>)
* Sets that channel's final state to be the sequence of all messages received whilst recording was active - which is none - so the channel state of <code>C<sub>23</sub></code> is `{}`.

![Chandy-Lamport Example Step 7](./img/L8%20Snapshot%20Ex%207.png)

We now have a consistent snapshot of the entire system composed of three process states:

* <code>P1 = S<sub>1</sub></code>
* <code>P2 = S<sub>2</sub></code>
* <code>P3 = S<sub>3</sub></code>

And six channel states:

* <code>C<sub>12</sub> = {}</code>
* <code>C<sub>21</sub> = {m3}</code>
* <code>C<sub>13</sub> = {}</code>
* <code>C<sub>31</sub> = {}</code>
* <code>C<sub>23</sub> = {}</code>
* <code>C<sub>32</sub> = {}</code>

### What About the Internal Events Not Recorded in the Process Snapshots?

In the above diagram, events `C`, `D` and `E` do not form part of `P1`'s snapshot recorded in state <code>S<sub>1</sub></code> because these events had not yet occurred at the time `P1` decided to take its snapshot.

Similarly, events `J` and `K` do not form part of `P3`'s snapshot recorded in state <code>S<sub>3</sub></code> because these events had not yet occurred at the time the marker message arrived from `P1`.

These events will all be recorded the next time a snapshot is taken.


## How Does the Entire System Know When the Snapshot Is Complete?

An individual process knows its local snapshot is complete when it has recorded:

* Its own internal state, and
* The state of ***all*** its incoming channels

If it can be shown that the snapshot process terminates for an individual process, then it follows that it will terminate for all participating processes in the system.

Now we can appreciate the importance of the assumptions listed at the start.  The success of this entire algorithm rests on the fact that:

* Eventual message delivery is guaranteed, and
* Messages never arrive out of order (all channels are FIFO queues), and
* Processes do not crash (yeah, right! Again, see [lecture 10](./Lecture%2010.md))

In Chandy & Lamport's [original paper](https://lamport.azurewebsites.net/pubs/chandy.pdf) they provide a proof that the snapshot process does in fact terminate.

Determining the snapshot for the entire system however lies outside the rules of the Chandy-Lamport algorithm and needs to be handled by some external coordinator that stitches all the individual process snapshots together.



---

| Previous | Next
|---|---
| [Lecture 7](./Lecture%207.md) | [Lecture 9](./Lecture%209.md)




---

***Endnotes***

<b id="f1">1</b>&nbsp;&nbsp; In this context, a "decentralised algorithm" is one that does not need to be invoked from a special coordinating process; any process in the system can act as the initiator.  A beneficial side-effect of this is that if two processes simultaneously decide to initiate a snapshot, then nothing bad happens.

[↩](#a1)


# Distributed Systems Lecture 9

## Lecture Given by [Lindsey Kuper](https://users.soe.ucsc.edu/~lkuper/) on April 17<sup>th</sup>, 2020 via [YouTube](https://www.youtube.com/watch?v=utsDozs1ZMc)

| Previous | Next
|---|---
| [Lecture 8](./Lecture%208.md) | [Lecture 10](./Lecture%2010.md)


## Big Picture View of the Chandy-Lamport Algorithm

### Chandy-Lamport Assumptions

The Chandy-Lamport algorithm was the very first to define how you can take a reliable snapshot of a running distributed system.  This algorithm does make some fairly large assumptions, but the fact that it works even if marker messages are delayed is a significant achievement.

#### FIFO Delivery

We have assumed that the communication channels used between processes in a distributed system operate as FIFO queues.  This means that a channel is a mechanism for delivering an ordered sequence of messages.  But as we saw in the previous lecture, this is far more than an assumption - it is a requirement.  If channels did not behave as FIFO queues, then the Chandy-Lamport Snapshot Algorithm will break.

So, this requirement then leads to the question:

***Q:***&nbsp;&nbsp; If the delivery mechanism in a distributed system ***cannot*** guarantee ordered delivery (I.E. FIFO anomalies are possible), then are other algorithms available for taking a global snapshot?
***A:***&nbsp;&nbsp; Yes, there are, but such algorithms have other drawbacks such as needing to pause application processing while the snapshot is taking place.

One particularly nice thing about the Chandy-Lamport algorithm is that you can take a snapshot while the application is running (I.E. it’s not a *stop-the-world* style algorithm).  The fact that a process sends out marker messages during its snapshot does not interfere with the application messages already travelling through the system.

#### Reliable Delivery

The Chandy-Lamport algorithm requires that messages are never:

* Lost
* Corrupted
* Duplicated

#### Processes Don't Crash

The Chandy-Lamport algorithm is not robust against processes crashing whilst the snapshot is being taken.  If this were to happen, at best the snapshot would be incomplete; but to obtain a full snapshot, you would have to start the snapshot process over again.

### The Chandy-Lamport Algorithm is Guaranteed to Terminate

Without giving a formal proof, in order to take a snapshot of a distributed system we must make each process responsible for recording:

* Its own internal state
* The state of all messages on its incoming channels

Then, when all the processes in the system have completed their snapshots, the sum of the individual snapshots becomes the consistent snapshot of the entire system.

If it can be demonstrated that these actions will terminate for an individual process, then it follows that they will terminate for the entire distributed system.

In section 3.3 of Chandy & Lamport's [original paper](./papers/chandy.pdf) they say:

> If the graph is strongly connected and at least one process spontaneously records its state, then all processes will record their states in finite time (assuming reliable delivery)

The term ***strongly connected*** means that every process is reachable from every other process via channels.  In our example however, we have assumed that every process is directly connected to every other process by a channel, thus we not only have a strongly connected graph, we have a ***complete graph***.

If we draw the processes in our example system as a graph, every process is connected to every other process, making a total graph.

![Total Graph](./img/L9%20Total%20Graph.png)

However, Chandy & Lamport require only that the graph is strongly connected; for example, like this:

![Connected Graph](./img/L9%20Connected%20Graph.png)

`P3` can still send messages to `P2` but it must send them via `P1`.

## Simultaneous Snapshot Initiators

It is interesting that Chandy & Lamport state that ***at least*** one process must start the global snapshot by recording its own state.  They do not require that ***only*** one process initiates the global snapshot.

So, let's look at what happens when two processes simultaneously decide to take a snapshot.

In the following diagram, processes `P1` and `P2` simultaneously decide to snapshot themselves.

![Simultaneous Snapshot 1](./img/L9%20Simultaneous%20Snapshot%201.png)

Since each is acting as the initiator, they both follow these rules:

* `P1` and `P2` both record their own state, creating states `S1` and `S2` respectively
* `P1` and `P2` both start recording messages on their incoming channels - <code>C<sub>21</sup></code> and <code>C<sub>12</sup></code> respectively
* `P1` and `P2` both send out marker messages on their outgoing channels

Now the marker messages arrive at each process.

![Simultaneous Snapshot 2](./img/L9%20Simultaneous%20Snapshot%202.png)

As soon as the marker messages arrive:

* `P1` and `P2` stop recording messages on their incoming channels
* `P1` and `P2` save the state of each recorded channel.
    In this case, no messages arrived on <code>C<sub>21</sup></code>, but message `m` arrived on <code>C<sub>12</sup></code>

Again, we now have a coherent snapshot of the whole system in spite of the fact that two processes simultaneously decided to act as initiators.

This is known as a ***consistent cut*** - something we'll talk about a little later.

### Is It Possible to Get a Bad Snapshot?

Could we end up with a bad snapshot such as the one shown below?

![Bad Snapshot](./img/L9%20Bad%20Snapshot.png)

No, this is in fact impossible because as soon as a process records its own state, it must immediately send out marker messages.  This is the rule that makes it impossible for message `m` to arrive at `P2` before the snapshot processing has completed.

The rules of the Chandy-Lamport Snapshot algorithm state that as soon as the internal state of `P1` is recorded, marker message ***must*** be sent on all outgoing channels.  So, the marker message will always be sent ***before*** event `B` happens in `P1` that sends message `m` to `P2`.  Also, because channels are FIFO queues, it is impossible for message `m` to arrive at `P2` before the marker message arrives.

To understand how important this is, let's consider what would happen if simultaneous initiators were ***not*** permitted and the initiator had to seek agreement from the other participants before initiating the snapshot:

* `P1` decides it wants to take a snapshot
* `P1` sends a message to all the participants saying *"Hi guys, I'd like to take a snapshot.  Is that OK with you?"*
* But whilst `P1` is waiting for everyone to respond, another process sends out a message saying *"Hi guys, I'd like to take a snapshot.  Is that OK with you?"*

This all gets very chaotic and could well lead to some sort of deadlock.

So, if multiple initiators are not permitted, then there has to be some way for processes to decide who is going to act as the sole initiator.  This then leads into the very challenging problem domain known as ***Agreement Problems*** (Warning: here be dragons!)

Since the Chandy-Lamport algorithm permits multiple initiators, it is very much easier to implement because we do not have to care about solving the hard problem of agreeing on either who will act as the initiator, or when a snapshot should be taken &mdash; ***any*** process can take a snapshot ***any*** time it likes!

Further to this, any process that receives a marker message does not need to care about either who sent that marker, or which process originally acted as the initiator.  Hence, markers can be very lightweight messages that do not need to carry any data such as the identity of the initiator.

The Chandy-Lamport algorithm is an example of a decentralised algorithm.  There are, however, algorithms that are centralised, and these ***do*** require a single process to act as the initiator (We'll talk more about this type of algorithm later in the course).

## Why Do We Want Snapshots in the First Place?

What are snapshots good for?  Here are some ideas:

* ***Checkpointing***
    If we are performing a process that is either expensive or based on non-deterministic input (such as user requests arriving over a network), then in the event of failure, a checkpoint allows us to reconstruct the system's state and provides us with a reasonable restart point.
    For expensive calculations, all our calculation effort up until the last checkpoint is preserved, and for transactional systems, the system state preserved at the checkpoint reduces data loss down to only those transactions that occurred between the checkpoint being taken and the system failing.
* ***Deadlock detection***
    Once a dead lock occurs at time `T` in a system, unless it is resolved, that deadlock will continue to exist for all points in time greater than `T`.  A snapshot can be used to perform deadlock detection and thus serves as a useful debugging tool
* ***Stable Property Detection***
    A deadlock is an example of a ***Stable Property***.  A property of the system is said to be ***stable***, if, once it becomes true, it remains true.
    Another example of a stable property is when the system has finished doing useful work - I.E. Task termination (however, human intervention might be required in order to detect that this state has been reached)

Be careful not to conflate a ***deadlock*** with a process crashing.  Typically (but not always), a deadlock occurs when two running processes enter a mutual wait state.  Thus, neither process has crashed, but at the same time, neither process is capable of doing any useful work because each is waiting for a response from the other.

## Chandy-Lamport Algorithm and Causality

The set of events in a Chandy-Lamport Snapshot will always make sense with respect to the causality of those events.

Now we need to introduce a new piece of terminology: a ***cut***.

A cut is a time frontier that divides a Lamport diagram into past and future events.

![Cut](./img/L9%20Cut.png)

An event is said to be ***in the cut*** if it belongs to the past.  In Lamport diagrams, where time goes downwards, this means events occurring above the line.

So, if event `E` is in the cut and `D->E` then for the cut to be ***consistent***, event `D` must also be in the cut.

This is a restatement of the principle of [consistent global snapshots](https://github.com/ChrisWhealy/DistributedSystemNotes/blob/master/Lecture%207.md#consistent-global-snapshot) that we saw in [lecture 7](./Lecture%207.md).

In both the of following diagrams `B->D`.  Therefore, for a cut to be consistent, it must preserve the fact that event `B` happens in the causal history of event `D`.

So, this cut is valid and is therefore called a consistent cut:

![Consistent Cut 1](./img/L9%20Consistent%20Cut%201.png)

Even though the cut has separated events `B` and `D`, their causality has not been reversed: event `B` remains on the "past" side of the cut, and event `D` remains on the "future" side.

However, in the diagram below, the cut is inconsistent because the causality of events `B` and `D` has been reversed:

![Inconsistent Cut](./img/L9%20Inconsistent%20Cut.png)

The happens-before relation between events `B` and `D` is now broken because the cut has moved the future event `D` into the past, and the past event `B` into the future.

## The Chandy-Lamport Algorithm Determines a Consistent Cut

If you take a cut of a distributed system and discover that the set of events in that cut is identical to a Chandy-Lamport snapshot, then you have a consistent cut.  This is what is meant when we say that a Chandy-Lamport Snapshot determines a consistent cut.

Going back to the more detailed example used in the previous lecture, we can see that the snapshot formed from three process states and six channel states forms a consistent cut.

![Consistent Cut 2](./img/L9%20Consistent%20Cut%202.png)

Another way of saying this is that a Chandy-Lamport snapshot is causally correct.


## Recap: Delivery Guarantees and Protocols

### FIFO Guarantee

If a process sends message `m2` after `m1`, then any process delivering both of these messages must deliver `m1` first.

A violation of this guarantee is a FIFO anomaly:

![FIFO Anomaly](./img/L5%20FIFO%20Anomaly.png)

### A Protocol to Enforce FIFO Delivery

In order to enforce FIFO delivery, we could implement strategies such as:

* Giving each message a sequence number.  The receiving process is then required to deliver these messages in sequence number order
* Requiring the receiving process to acknowledge receipt of a message

### Causal Delivery

The [causal delivery](https://github.com/ChrisWhealy/DistributedSystemNotes/blob/master/Lecture%206.md#causal-delivery) guarantee simply says messages must be delivered in the order they were sent.

> If `m1`'s send happens before `m2`'s send, then `m1`'s delivery must happen before `m2`'s delivery.

A causal anomaly looks like this:

![Causal Anomaly](./img/L3%20Causal%20Anomaly.png)

### A Protocol to Enforce Causal Delivery

In order to enforce causal delivery (at least in the case of broadcast messages), we could implement a causal broadcast strategy based on vector clocks.  Each process is then responsible for maintaining its own vector clock and by means of a queueing mechanism, ensures that no ***messages from the future*** are delivered early.

### Totally Ordered Delivery

If a process delivers `m1` then `m2`, all participating processes delivering both messages must deliver `m1` first.

A violation of totally-ordered delivery looks like this:

![Total Order Anomaly](./img/L6%20Total%20Order%20Anomaly.png)

### A Protocol to Enforce Totally-Ordered Delivery

We did not actually talk about a protocol for enforcing totally-ordered delivery - we just spoke about it being hard!

But here's an idea.  If a fifth process were added to act as a coordinator, then totally-ordered delivery could be ensured by telling every client process that in order to change the state of the data in the replicated databases, it must first check in with the coordinator.  The coordinator then acts as a middleman for ensuring that message delivery happens in the correct order.

However, this approach has several downsides:

* Under high-load situations, the coordinator process could become a performance bottleneck
* If the coordinator crashes, then all updates stop until such time as the coordinator can be restarted (but who's going to monitor the coordinator process &mdash; a coordinator-coordinator process?)

## Safety and Liveness Properties

Let's now briefly introduce the next topic, that of ***safety*** and ***liveness*** properties.

| Safety Property | Liveness Property |
|---|---|
| Something bad will ***not*** happen | Something good ***eventually*** happens
| In a finite execution, we can demonstrate that something bad will happen if this property is not satisfied.<br><br>FIFO anomalies, Causal Anomalies and Totally-Ordered Anomalies are all examples of safety properties because we can demonstrate that their failure causes something bad to happen | For example, all client messages are eventually answered.<br><br>The problem though is that liveness properties tend to have very open-ended definitions.  This means we might have to wait forever before something good happens... Consequently, when considering ***finite*** execution, it is very difficult (impossible?) to provide counter examples.<br><br>This is why liveness properties are much harder to reason about.

---

| Previous | Next
|---|---
| [Lecture 8](./Lecture%208.md) | [Lecture 10](./Lecture%2010.md)

# Distributed Systems Lecture 10

## Lecture Given by [Lindsey Kuper](https://users.soe.ucsc.edu/~lkuper/) on April 20<sup>th</sup>, 2020 via [YouTube](https://www.youtube.com/watch?v=5QH37qLyO7A)

| Previous | Next
|---|---
| [Lecture 9](./Lecture%209.md) | [Lecture 11](./Lecture%2011.md)


## Recap: Safety & Liveness Properties

| Safety Property | Liveness Property
|---|---|
| Something bad will ***not*** happen | Something good ***eventually*** happens
| Can be violated in a finite execution.<br>![FIFO Anomaly](./img/L5%20FIFO%20Anomaly.png) | Cannot be violated in finite execution.<br>![No violation - yet](./img/L5%20Protocol%204.png)
| Examples of safety properties include all the delivery guarantees we've spoken about so far such as FIFO, Causal and Totally-Ordered | An example of a liveness property is the guarantee that the system will ***eventually*** respond to a client request.<br>However, the diagram above is not a counterexample because the definitions of liveness guarantees tend to be open-ended and therefore cannot exclude the possibility of *"waiting forever"*

The trouble with Distributed System design is that in order to be useful, it needs both types of property to be present; however, the open-ended nature of liveness properties makes them hard to reason about.

Let's say we want to implement a protocol that satisfies the safety property of FIFO delivery, but doesn't need to care about any liveness properties.  So, we could build a system that either drops or ignores every message...

![Vacuous FIFO Delivery](./img/L10%20Vacuous%20FIFO%20Delivery.png)

This is completely useless, but at least it guarantees FIFO delivery! (Doh!)

So, it turns out that on their own, neither safety nor liveness properties are of much practical use.  We need a system that implements a combination of both.

### Liveness Property: Reliable Delivery

Other than the *"eventual deliver"* property we've spoken of, the only other liveness property we've mentioned is *"reliable delivery"*, and the definition varies depending on who you ask, but here's one definition:

> Let `P1` be a process that sends a message `m` to process `P2`.
> If neither `P1` nor `P2` crashes, then `P2` eventually delivers message `m`

However, you might also see an extended version of the above definition:

> Let `P1` be a process that sends a message `m` to process `P2`.
> If neither `P1` nor `P2` crashes ***and not all messages are lost***, then `P2` eventually delivers message `m`

These definitions vary only in respect of whether or not we should be concerned about message loss.  This question then leads us into the topic of fault models that we will come to shortly.  However, here we assert that reliable delivery is a liveness property.

But why is this?

Firstly, we can see that the idea of reliable delivery cannot be violated in a finite execution: that is, in a finite execution, we cannot draw a Lamport diagram that demonstrates a violating counter-example.

So, since we know that all the properties we care about are either safety properties, liveness properties or some combination of both, and we know that *"reliable delivery"* is not a safety property, we know it must therefore be a liveness property.

## So, What Exactly is a "Fault"?

Any time you design a system, you need to make certain assumptions about the environment in which that system will be operating.  So, before you can describe your system as being ***fault tolerant***, you must first clearly define what circumstances could occur that constitute a fault, and secondly, how your system will respond under such circumstances.  Only then will you understand what conditions your system needs to tolerate.

In other words, we must start with a clear understanding of what exactly constitutes a fault.

In a simple scenario like the one below, machine `M1` asks machine `M2` the question *"What's the value of `x`?"* and expects to hear something back such as `x=5`.

![Possible Faults](./img/L10%20Possible%20Faults.png)

What sort of faults could occur here?

* `M2` never receives the message because it was lost due to a communication fault
* `M2` gets the message, but is unable to answer it because it became corrupted
* `M2` gets the message, but only after a significant delay
* `M2` does not respond because it has already crashed
* `M2` crashes as a result of trying to answer `M1`'s question
* `M2` is too busy to answer the question
* `M2` ignores the message
* `M2` deliberately responds with the wrong answer
* `M2` sends a response back to `M1` which gets lost, corrupted or delayed
* `M2` sends a response back to `M1`, but then `M1` crashes as it tries to proces the answer
* etc...

The problem here is that even in this minimal scenario, we cannot enumerate all the possible errors the might occur; however, we can categorise them.

### Fault Categories

Let's arrange these types of fault into different informal categories.

| Fault Category | Description
|---|---
| Crash | Software execution halts or hardware fails
| Omission | Messages are sent, but not received (I.E. lost)
| Timing | Messages are sent and processed successfully, but very slowly<br>Also known as a ***performance*** fault
| Byzantine<sup id="a1">[1](#f1)</sup> | Intentionally malicious or arbitrary behaviour

These fault categories have been used in Distributed System's design since about the early 1990's and are presented above in hierarchical order, starting with the lowest level first.

### Crash Fault

At the bottom of this hierarchy is the ***crash fault***.  This simply means that a process has stopped exchanging messages with the other participants in the system.

A crash fault can happen for a variety of reasons: for instance, execution could halt due to a software failure, or the process might continue to handle its own internal messages but cease responding to external messages.  Whilst this second case is not due to software execution halting, as far as the other participants in the system are concerned, this process takes no further part in the overall operation of the system and may as well have crashed.

### Omission Fault

When a process continues execution, but for whatever reason, fails to send or receive some, but not all messages.

### Timing (or Performance) Fault

A process responds either too late or too early.  The typical case is where a process responds too slowly; however, at the hardware level, it is possible for a response to be too fast.

In this course, we're going to sidestep the discussion of timing faults because we will be focussing on the asynchronous message delivery model &mdash; which never makes any delivery time guarantees in the first place!

### Byzantine Fault

A process behaves in an arbitrarily erroneous, or possibly even malicious way.  Usually, such behaviour is intentional. Again, in this course we won't be spending much time talking about this type of fault.

## Fault Hierarchy

Why are the fault categories listed in this particular order?


Let's says we have two different protocols, `X` and `Y`.

| | Protocol `X` | Protocol `Y`
|---|---|---|
| **Tolerates** | Crash Faults | Omission Faults

If Protocol `Y` tolerates omission faults, does it also tolerate crash faults?  If so, why?

### Crash and Omission Faults

If a process crashes, then ***every*** message sent to that process will not be received; therefore, this is a special case of an omission fault in which a process fails to send or receive only a certain number of messages.

![Fault Hierarchy 1](./img/L10%20Fault%20Hierarchy%201.png)

Hence if process `P1` can tolerate process `P2` failing to send or receive ***some*** messages (an omission fault), then by definition, `P1` must also be able to tolerate the case where `P2` fails to send or receive ***all*** messages (a crash fault).

The set of crash faults form a proper subset within the set of omission faults.

### Timing Faults

In the same way that crash faults are a special case of omission faults, omission faults are a special case of timing faults.

A timing fault is where the response to a message is received outside an acceptable timeframe (usually, too slowly), and an omission fault is where the response to a message is never received (infinitely too slow)

![Fault Hierarchy 2](./img/L10%20Fault%20Hierarchy%202.png)


### Byzantine Faults

A Byzantine fault is where a process behaves in an arbitrary or intentionally malicious way.  So, if a protocol is tolerant of Byzantine faults, does this mean it must also tolerate timing faults?

Yes, it does.

The reason is that if a process `B` (for Byzantine) starts behaving in an arbitrary or malicious manner, all other processes communicating with `B` will be unable to distinguish faults in `B` due to timing errors, with faults in `B` due to arbitrary or malicious behaviour.

Consequently, if process `B` decides that to say:

* *"I'm going to pretend to crash"*, or
* *"I'm not going to respond to certain messages from certain other processes"*, or
* *I'm deliberately going to mislead two processes by swapping my responses around*

Any process communicating with `B` will be unable to determine the true cause of such behaviour.

> ***My Aside***
>
> This is because computers are unable of determine the intent of, or motive behind an action, their inferences can only be made on the mechanistic basis of cause and effect

The list of possible fault behaviours here is endless...

![Fault Hierarchy 3](./img/L10%20Fault%20Hierarchy%203.png)

For more details, see the paper ["Atomic Broadcast: From Simple Message Diffusion to Byzantine Agreement"](./papers/atomic_broadcast.pdf) by Cristian et al.

Given the fact that we will confine our discussion to systems that use asynchronous communication, such systems cannot give any guarantees about message delivery times; therefore, for the remainder of this course, discussion around fault categories will look more like this:

![Fault Hierarchy 4](./img/L10%20Fault%20Hierarchy%204.png)

## Are These the Only Fault Categories?

No: these fault categories can be subdivided.  For instance, some Byzantine faults are easier to deal with than others.

For instance, a Byzantine Fault that is relatively easy to deal with is message alteration or duplication.

If you receive a message that has been altered (maliciously or otherwise), then such faults are generally fairly easy to detect using techniques such as checksums or message hashes.  What's much harder to detect is message corruption where the corruption is so subtle that your authentication technique fails to detect it.<sup id="a2">[2](#f2)</sup>

So, we can redraw the above diagram as follows:

![Fault Hierarchy 5](./img/L10%20Fault%20Hierarchy%205.png)

If we detect that a message has been corrupted, the simplest way of handling it is to ignore it completely.  In this case, we have handled the message in the same way as if we had never received it in the first place.  Thus, we have downgraded this particular type of Byzantine fault to an Omission fault.

## Fault Models

Based on the preceding discussion we can define a ***Fault Model*** as:

> The specification of faults that a system may exhibit, which in turn defines the kind of faults which will be tolerated by the system.

Fault models are nested in the same way as fault categories.

In general, the easiest faults to tolerate are the ones in the centre of the diagram, and as we move outwards, fault model implementation become more and more complicated, simply because a greater number and type of bad things can happen.

In this class, we will be looking mostly at the Omission Model.  This will still be hard to implement, however, because there are still plenty of things that can go wrong!

## The Two Generals Problem

This is a classic thought experiment that dates back to 1975 from the appendix of a paper by Akkoyunlu, Ekanadham and Huber called "[Some Constraints and Trade-offs in the Design of Network Communications](./papers/net_comms_constraints_tradeoffs.pdf)"

In this situation, two armies commanded by Generals Alice and Bob want to attack a common enemy; however, several significant challenges must be overcome before victory can be assured:

* Alice's and Bob's armies are camped in two valleys on opposites sides of their common enemy
* The enemy is camped in the valley in between Alice and Bob
* The enemy has sufficient strength that victory cannot be assured unless Alice and Bob attack simultaneously
* Alice and Bob can only communicate with each other by sending messengers through enemy territory
* Alice and Bob cannot be sure that any messages they send will get through because the messenger risks being captured, and the message fails to get through


![Two Generals 1](./img/L10%20Two%20Generals.png)

What form of communication can these Generals have with each other so that they can both be confident that they are acting on some shared, common knowledge?  For instance, if the plan is to attack tomorrow at dawn, then how can both Generals be sure that the other has firstly agreed to this plan, and secondly, is ready to act on it?

Since the armies of Alice and Bob are not strong enough on their own to defeat this enemy, victory is only possible if they arrive at a commonly agreed plan of action

Let's look at a few scenarios:

* Alice sends Bob the message ***"Attack at dawn!"***.

    ***Q:***&nbsp;&nbsp;Having sent this message, should Alice simply go ahead and attack at dawn?
    ***A:***&nbsp;&nbsp;No, because she has no way of knowing that Bob has even received the message, let alone agreed to it.

    If Alice attacks on her own, there is a significant chance of defeat, so she should wait for Bob's confirmation that he has agreed to the plan.

* Let's now say that Bob has received the message, agreed to it, and sent a confirmation back saying *"Yes, we attack at dawn!"*.

    ***Q:***&nbsp;&nbsp;Should Bob now go ahead and attack at dawn?
    ***A:***&nbsp;&nbsp;No!  Because he does not know that Alice has received his confirmation &mdash; again, a lone attack would be very risky.

* Let's then say that Alice receives Bob's agreement to attack at dawn - is this good enough for Alice to launch an attack?  No, because Bob doesn't know that Alice knows that he's agreed to attack...

    And this is all getting very silly and sounds like good material for a Monty Python sketch!

As it turns out, it has been proven impossible to eliminate 100% of the uncertainty inherent in systems where communication reliability cannot be guaranteed.

### Indeterminacy of the Omission Model

In the Omission Model, it is impossible for either of the two Generals to know with 100% certainty that the other has agreed to attack.  This example is just one of many fundamental impossibility results in distributed systems, and it applies in any setting where the communication between participants is liable to failure.

## Work Arounds for the Two Generals Problem

Some possibilities do exist here:

* Instead of trying to decide on the basis of unreliable communication, make a plan in advance and share that plan between the participants.  In other words, act on the basis of shared common knowledge<sup id="a3">[3](#f3)</sup>.
* Since unreliable communication excludes the possibility of achieving ***total*** certainty, the best we can hope for is ***reasonable*** certainty.


To achieve reasonable certainty, we could adopt the following strategy:

1. Alice could send Bob a sequence of messages knowing that on average, at least one will get through.
1. For every one of Alice's messages that successfully reaches Bob, Bob sends back an acknowledgement.  Again, since not of all these acknowledgments will make it back to Alice, multiple acknowledgements are needed in the hope that at least one will get through.
1. Alice receives Bob's first acknowledgement and stops sending her stream of messages.
1. After a certain period of time, Bob's confidence will start to grow that at least one of his acknowledgements got through because Alice has stopped sending her original message.

The objective here is not to remove uncertainty, but to lower it to a level considered acceptable enough to act upon.


---

| Previous | Next
|---|---
| [Lecture 9](./Lecture%209.md) | [Lecture 11](./Lecture%2011.md)


---
***Endnotes***

<b id="f1">1</b>&nbsp;&nbsp; Why is this type of fault called a <b><i>"Byzantine"</i></b> fault?

The name comes from an example in a paper by Leslie Lamport, Robert Shostak and Marshall Pease.  Here, they describe a situation in which, in order to avoid being defeated by their enemy, the different Generals in the Byzantine Army must all agree on a coordinated strategy for capturing a city; however, it is suspected that some of these Generals might be traitors and will thus attempt to disrupt the plans of the loyal generals.

To avoid any political issues that might have been created by choosing Generals and Armies from the recent past, they chose to use an example from the [Byzantine Empire](https://en.wikipedia.org/wiki/Byzantine_Empire) &mdash; the eastern successor empire to the Romans after their empire fell in the 5th Century AD.  The original paper can be found [here](./papers/byzantine.pdf)

The point here is that the behaviour of a small number of malicious participants will not jeopardise the overall success of the system.

[↩](#a1)

<b id="f2">2</b>&nbsp;&nbsp; Discussion of such authentication techniques is not covered in this course

[↩](#a2)

<b id="f3">3</b>&nbsp;&nbsp; Knowledge is said to be "common" when all participants in a system know with 100% certainty that all other participants share the same knowledge.  But not only is this very difficult to establish externally, it is also very fragile.  What would happen for instance, if someone needs to change the plan?  How could the changed plan then become accepted, common knowledge?

[↩](#a3)
# Distributed Systems Lecture 11

## Lecture Given by [Lindsey Kuper](https://users.soe.ucsc.edu/~lkuper/) on April 22<sup>nd</sup>, 2020 via [YouTube](https://www.youtube.com/watch?v=Rly9GBg14Zs)

| Previous | Next
|---|---
| [Lecture 10](./Lecture%2010.md) | [Lecture 12](./Lecture%2012.md)



## Implementing Reliable Delivery

### What Exactly is Reliable Delivery?

The definition we gave in the previous lecture for reliable delivery was the following

> Let `P1` be a process that sends a message `m` to process `P2`.
> If neither `P1` nor `P2` crashes,<sup><b>*</b></sup> then `P2` eventually delivers message `m`

We also qualified this definition with the further criterion (indicated by the star) that says:

**\*** So, it appears there could be some circumstances under which we need to care about message loss, and some circumstances under which we don't.

The difference here depends on which failure model we want to implement.  If we are implementing the Crash Model, then the only kind of failures we will tolerate are processes crashing. So, under these circumstances, we will not handle message loss.  However, if we decide to implement the Omission Model, message loss must also be tolerated and therefore handled.

So, our definition of ***Reliable Delivery*** varies depending on which fault model we choose to implement.

From a practical perspective, the Omission Model is a far more useful approach for handling real-life situations since message loss is a real, everyday occurrence.

Remember also from the previous lecture that due to their hierarchical relationship, if we implement the Omission Model, we have also implemented the Crash Model.

![Fault Hierarchy 1](./img/L10%20Fault%20Hierarchy%201.png)

### But Can't We Have a Consistent Definition of "Reliable Delivery"

Wouldn't it be better to have a consistent definition of "Reliable Delivery" that doesn't accumulate extra caveats depending upon the fault model?

Certainly - that would be something like this:

> If a correct process `P1` sends a message `m` to a correct process `P2` and not all messages are lost, then `P2` eventually delivers message `m`.

Ok, but haven't you just hidden the variability of the earlier definition behind the abstract term ***correct process***?  Yes, that's true &mdash; but you did ask for a consistent definition!

The term ***correct process*** means different things in different fault models.  If we need to implement the Byzantine Fault Model, then a ***correct*** process is a non-malicious or non-arbitrary process; however, if we are implementing the Crash Model, then a ***correct*** process is simply one that doesn't crash.

So, as soon as you see the word ***"correct"*** in a definition like the one above, we should immediately determine which fault model is being used, because this will then tell us what ***correct*** means in that particular context.


### How Do We Go About Implementing Reliable Delivery?

Going back to The Two Generals Problem discussed in the last lecture, one approach to help `Alice` and `Bob` launch a coordinated attack would be for `Alice` to keep sending the message `"Attack at dawn"` until she receives an `ack` from `Bob`.

This could be implemented using the following algorithm:

* `Alice` sends the message `"Attack at dawn"` to `Bob`, then places it into a send buffer that has a predetermined timeout period
* If an `ack` is received from `Bob` during the timeout period, communication was successful and `Alice` can delete the message from her send buffer
* If the timeout expires without receiving an `ack` from `Bob`, `Alice` resends the message

![Reliable delivery 1](./img/L11%20Reliable%20Delivery%201.png)

However, this style of implementation is not without its issues because it can never solve the Two Generals Problem:

* When `Alice` receives an `ack` from `Bob`, she can be sure that `Bob` got her message; however, `Bob` is still unsure that his `ack` was received
* Reliable delivery does not need to assume FIFO delivery, so copies of `Alice`'s original message could be received after `Bob` has already issued an `ack`.

Does it matter that `Bob` receives multiple copies of the same message?

In this situation, due to the nature of this particular message, no it doesn't.  This is partly because this particular strategy for increasing communication certainty requires `Alice` to send multiple messages until such time as she receives an `ack` from `Bob`; consequently, `Bob` will, mostly likely, receive multiple copies of the same message.

However, what if `Bob` was a Key/Value store and `Alice` wanted to modify the value of some variable?  Well, this depends entirely what `Alice`'s message contains.

![Reliable delivery 2](./img/L11%20Reliable%20Delivery%202.png)

If the message simply sets `x` to some absolute value, then this would not result in any data corruption.

![Reliable delivery 3](./img/L11%20Reliable%20Delivery%203.png)

However, if the message instructs the KeyStore to increment the value of `x`, then this will create significant problems if such a message were delivered more than once.

### Idempotency

The word ***idempotent*** comes from the Latin *idem* meaning "the same" and *potens* meaning "power".

In this context, the instruction contained in the message is said to be ***idempotent*** if (in mathematical terms):

`f(x) = f(f(x)) = f(f(f(x))) etc...`

In other words, an idempotent function `f` only has an effect the first time it is applied to some value `x`.  Thereafter, subsequent applications of function `f` to the value returned by `f(x)` have no further effect.

So, assigning a value to a variable is idempotent, but incrementing a variable is not.

Generally speaking, if we can work with idempotent operations, then our implementation of reliable delivery will be easier because we can be certain that nothing bad will happen to our data if, for some reason, the operation is applied more than once.

### How Many Times Should a Message be Delivered?

From the above discussion (and assuming that all communication happens within the asynchronous network model), we can say that reliable delivery therefore means that a message is delivered ***at least once***.

Let's say we have some  function `del` that returns the number of times message `m` has been delivered, then there are three possible options:

| Delivery Strategy | Delivery Count
|---|---
| At least once | `1 ≤ del(m)`
| At most once | `0 ≤ del(m) ≤ 1`
| Exactly once | `del(m) == 1`


Looking at the above table, it can be seen that since ***at most once*** delivery allows for a message to be delivered zero times, then this strategy can be implemented (at least vacuously) by not sending the message at all!  Doh!

But how about the ***exactly once*** strategy?

There does not appear to be any formal proof to demonstrate that this strategy is impossible to implement; however, it is certainly very hard to ensure.  Any time a system claims to implement ***exactly once*** delivery, the reality is that in the strictest sense, other assumptions have been made about the system that then give the appearance of exactly once delivery.  Such systems tend either to work with idempotent messages (which you can deliver as many times as you like anyway), or there is some sort of message de-duplication functionality at work.


## How Many Recipients Receive This Message?

Most of the message sending scenarios we've looked at so far are cases where one participant sends a message to exactly one other participant.

In [lecture 7](Lecture%207.md) we looked at an implementation of causal broadcast.  This is the situation in which ***all*** participants in the system receive the message (excluding of course the process that sent the message in the first place).  By means of vector clocks, we were able to ensure that a ***message from the future*** was not delivered too early.

![Causal Broadcast](./img/L7%20Causal%20Broadcast%208.png)

Then there is the case that one participant sends a message to ***many***, but not all of the other participants in the system.  An example of this the Total-Order anomaly we also saw in lecture 7.

![Total Order Anomaly](./img/L7%20TO%20Anomaly.png)

In this case `C1` sends messages to `R1` and `R2`, but not `C2`; likewise, `C2` sends messages to `R1` and `R2`, but not `C1`.

So, assuming reliable delivery, we have three different message sending strategies:

| Message Sending Strategy | Number of Recipients
|---|---
| Unicast | One
| Multicast | Many
| Broadcast | All


In this course we will not speak to much about implementing unicast messages; instead, we will simply assume that a unicast command exists as a primitive within each process.

In this manner, we could send broadcast or multicast messages simply by invoking the unicast primitive multiple times.

![Broadcast Implemented Using Unicast](./img/L11%20Broadcast%201.png)

Up until now, we have been drawing our Lamport diagrams with multiple messages coming from a single event in the sending process - and this is how it should be.  Conceptually, we need to treat broadcast messages as having exactly one point of origin.

However, under the hood, the mechanism for sending the actual messages could be multiple invocations of the unicast send primitive.  But this will only get us so far.  The problem is that even if we batch together all the message send commands in some transactional way, if we get halfway through sending this batch of messages and something goes wrong, what remedial action can we take about the messages we've already sent - attempt to cancel or revoke them?

So, the reality is that we need a reliable way to define reliable broadcast.


## Implementing Reliable Broadcast

Remembering the discussion of the term ***correct*** given in the section above, reliable broadcast can then be generically defined as:

> If the correct process delivers the broadcast message `m` then all correct processes deliver `m`.

***IMPORTANT ASSUMPTION***
The discussion that follows assumes we are working within the Crash Model where we can pretend that message loss never happens.  Under these limited conditions, we only need to handle the case of processes crashing.

Let's say `Alice` sends a message to `Bob` and `Carol`.

Both `Bob` and `Carol` receive the message, and `Bob` delivers it correctly; however, `Carol` crashes before she can deliver that message.

![Reliable Broadcast 1](./img/L11%20Reliable%20Broadcast%201.png)

Has this violated the rules of reliable broadcast?

Actually, no it hasn't.  This is because since `Carol` crashed, she does not qualify as a ***correct*** process; therefore, its ok that she didn't deliver the message.

Now consider this next scenario: as we've mentioned earlier, under the hood, a broadcast message can be implemented as a sequence of unicast messages.  So, with this in mind, let's say that `Alice` wants to send a broadcast message to `Bob` and `Carol`; but as we now know, this will be implemented at two unicast messages that conceptually form a single send event.

So `Alice` sends the first unicast message to `Bob` who delivers it correctly.  But before `Alice` can send the second unicast message to `Carol`, she crashes.  This leaves both `Bob` and `Carol` running normally; however, `Bob` received the "broadcast" message but `Carol` did not.

![Reliable Broadcast 2](./img/L11%20Reliable%20Broadcast%202.png)

We could argue here that since `Alice` did not successfully send the message to ***all*** the participants, it is therefore not a true "broadcast" message. But this is unsatisfactory really because it sounds like we're trying to squeeze through a loophole in the definition of the word "broadcast".

In reality, `Alice` fully intended to send a message to ***all*** participants in the system; therefore, irrespective of the success or failure of this action, the intention was to send a ***broadcast*** message.  Therefore, this situation is in violation of the specification for a ***reliable broadcast***.

Notice that the definition of a reliable broadcast message speaks only about the correctness of the processes delivering that message; it says nothing about the correctness of the sending process.

Therefore, under this definition, if the correct process `Bob` received and delivered the message, then the correct process `Carol` should also receive and deliver this message.  Since `Carol` never received this message (for whatever reason), this is a violation of the rules of reliable broadcast.

So how can we implement reliable broadcast, if we know that halfway through the sequence of unicast sends, the sending process could crash?

Here's one outline of an algorithm for reliable broadcast:

* All processes keep a set of delivered messages in their local state
* When a process `P` wants to broadcast a message `m`:
    * It must unicast that message to all other processes (except itself)
    * `P` adds `m` to its set of delivered messages
* When `P1` receives a message `m` from `P2`:
    * If `m` is already in `P1`'s set of delivered messages, `P1` does nothing
    * Otherwise, `P1` unicasts `m` to everyone except itself and `P2`, and adds `m` to its set of delivered messages

Let's see this algorithm at work:

`Alice` sends a message to `Bob`, but then `Alice` immediately crashes.

However, since `Bob` has not seen that message before, he adds it to his set of delivered messages and unicasts it to `Alice` and `Carol` &mdash; but then `Bob` immediately crashes!

![Reliable Broadcast 3](./img/L11%20Reliable%20Broadcast%203.png)

Since `Carol` is the only ***correct*** process left running, she delivers the message.  However, since `Alice` and `Bob` have both crashed, they are excluded from our definition of a ***correct*** process, and so the rules of reliable broadcast remain satisfied.

Even with the optimization of not sending a known message back to the sender, this protocol still results in processes receiving duplicate messages.

![Reliable Broadcast 4](./img/L11%20Reliable%20Broadcast%204.png)

`Bob` and `Carol` each receive this message twice.

So, a further optimization can be that if a process has already delivered the received message, then simply do nothing.

## Fault Tolerance Often Involves Making Copies of Things

This is a fundamental concept that will be used a lot as we proceed through this course.

We can mitigate message loss by making copies of messages; but what else might we lose?

In addition to message sends and receives, there are also internal events within a process that record its changes of state (I.E. the changes that occur to a process' internal data).  How can we mitigate against data loss?  Again, by taking copies.

### Why Have Multiple Copies of Data?

There are several reasons:

***Protection Against Data Loss***
The state of a process at time `t` is determined by the complete set of events that have occurred up until that time.  Therefore, by knowing a process' event history we can reconstruct the state that process.  This then allows us to keep replicas of processes in different locations.  If one data centre goes down, then we still have all the data preserved in one or more other data centres.

***Response Time***
Having your data in multiple data centres not only solves the issue of data loss, but it can also help with reducing response times since the data centre that is physically closest to you is the one most likely to give you the fastest response.

***Load Balancing***
If you are experiencing a high volume of requests for the data, then having multiple copies of the data is a good way to distribute the processing load across multiple machines in multiple locations.


### Reliable Delivery

In the case of reliable delivery, we can tolerate message loss by sending multiple copies of the same message until at least one gets through.

### Reliable Broadcast

In the case of reliable broadcast, we can tolerate processes crashing by making copies of messages and then forwarding them.


## Question Received Via Chat

***Q:*** At the moment, we're only working within the Crash Model.  How would this work if we needed to work in the Omission Model?

***A:*** Remembering that fault models are arranged hierarchically, the algorithm used for reliable broadcast will act as the foundation for the algorithm used in the Omission Model.  Therefore, what we will need to do is extend the reliable broadcast algorithm with an algorithm for reliable delivery.

---

| Previous | Next
|---|---
| [Lecture 10](./Lecture%2010.md) | [Lecture 12](./Lecture%2012.md)

# Distributed Systems Lecture 12

## Lecture Given by [Lindsey Kuper](https://users.soe.ucsc.edu/~lkuper/) on April 24<sup>th</sup>, 2020 via [YouTube](https://www.youtube.com/watch?v=2dGJXEGTbGQ)


| Previous | Next
|---|---
| [Lecture 11](./Lecture%2011.md) | [Lecture 13](./Lecture%2013.md)


## Replication

Replication is the main strategy for mitigating loss:

* To avoid message loss, messages are copied and sent multiple times
* To avoid data loss, process state is copied

However, replication is used for more than just mitigating loss.

* ***Scalability/Load Balancing***
    Handling sudden peaks in request volume or sustained high load
* ***Fault Tolerance***
    Multiple, redundant instances of hardware/software
* ***Data Locality***
    If you are physically close to your data, then you are likely to get a faster response to your requests.  Hence, geographic distribution of data tends to provide better response times for users spread out around the world

However, what are the downsides of replication?

### What Are the Reasons Not to Do Replication?

Maintaining consistency of data across replicas is especially challenging when you consider that processes:

* Can crash due to software or hardware failure
* Are physically distant from each other
* Are continually changing state asynchronously
* Are connected by an unreliable communication network

But mitigation of these problems was the reason for wanting to do replication in the first place!  So, all the reasons for needing replication also make it hard to implement.

Another consideration is cost.

If a message is lost during transmission, you can simply resend it; so, the cost of transmission failure is paid only ***after*** the failure has occurred; however, if a server crashes, you cannot avoid data loss unless you ***already*** have a replica server up and running.  So, to protect against hardware failure, you must incur the cost of running replica servers ***before*** anything has gone wrong.

## Total Order vs. Determinism

Looking back at our total order anomaly diagram, we can see that this problem raises the issue of maintaining data consistency across replicas.

![Total Order Anomaly](./img/L12%20TO%20Anomaly.png)

The problem here is that each replica holds a different value of `x`.

Let's look at the simplest case where, instead of replicating the data, we only have one copy.

Depending on the order in which messages arrive, we might end up with `x=2`

![Single Replica 1](./img/L12%20Single%20Replica%201.png)

Or, we might end up with `x=1`

![Single Replica 2](./img/L12%20Single%20Replica%202.png)

So simply reducing the number of replicas to one does not solve our problem.

A further problem is that neither of the situations described above can be considered wrong.  Both runs of the system are valid and correct, and neither violate Total-Order delivery.

Remember that if we want totally-ordered delivery:

> If a process delivers message `M1` followed by `M2`, then all processes delivering both `M1` and `M2` must deliver `M1` first followed by `M2`.

Process `R1` above is the only process delivering messages; therefore, it can never be in violation of the Totally-Ordered Delivery rule!  This gives process `R1` a lot of control over when to deliver messages.  In fact, process `R1` can decide for itself what *"Total Order"* actually means by controlling when it delivers messages.

In fact, `R1` could deliver messages in different orders across different runs and still not violate the safety property of Totally Ordered Delivery; however, it would be violating a different property called ***Determinism***

## Determinism

Determinism is a property that relates multiple runs of a system to each other.

![Determinism Violation](./img/L12%20Determinism%20Violation.png)

If `R` delivers messages in one order on one run, but in a different order on the next run, then this is a violation of determinism.

> ***Totally-Ordered Delivery***
> This is a property that relates to a single run of a system
>
> ***Determinism***
> This is a property that relates to multiple runs of the same system

BTW, any property relating to system behaviour across multiple runs is known as a ***hyperproperty***.

When there's only one replica, it will establish its own total order; however, when we have multiple replicas, we need each replica to behave with the same, consistent total order so that all the clients think they are dealing with a single system.

Here's an informal definition of what we want:

> A replicated storage system is ***strongly consistent*** if clients can't tell that it's replicated

As far as the clients are concerned, they should think that there is only one data storage system, even though, under the hood, there could be multiple replicas all working together.

Every strongly consistent replication protocol that we're going to discuss will implement a ***total order*** on events, but each will do so in different ways.

However, before we jump into these details, let's look at some of the ways that a client could tell that its working with multiple replicas.  To put this the other way around, let's look at the different ways in which replicas might disagree.

### Disagreements Between Replicas: Read Your Writes

Here's a possibility.

![Replica Disagreement 1](./img/L12%20Replica%20Disagreement%201.png)

The client wants to bind the value `5` to the name `x`, so it sends the message `x=5` to `R1`; but this value is not replicated across to `R2`.  So, when the client next queries the value of `x`, it gets back the unexpected result of `undefined` (in other words *"Who's x?"*)

In this case, this is known as a ***Read Your Writes*** anomaly and is one of the most fundamental questions you should ask of any replicated storage system &mdash; that is, if I've just written a value, do I get the same value back when I perform a subsequent read?

There are some systems that still don't provide this!

### Disagreements Between Replicas: FIFO Consistency

> ***FIFO Consistency***
> FIFO consistency is where writes done by a single process are seen by all processes in the order they were issued.

Here's a situation in which violation of this property results in replica disagreement.

![Replica Disagreement 2](./img/L12%20Replica%20Disagreement%202.png)

Let's says we have a banking system with two replicas `R1` and `R2`.  The client `C1` makes the following sequence of transactions against `R1`:

* Deposits \$50
* Receives an acknowledgement for the deposit
* Withdraws \$40
* Receives an acknowledgement for the withdrawal

Ok, that's fine.  `C1` can be very confident that her balance is \$10 &mdash; at least according to the records held in `R1`.


However, `R1` now sends out some synchronising messages, but `R2` delivers these messages in the wrong order.  After delivering the second message first, the client's balance is now incorrectly shown to be \$40 overdrawn.  If at this point in time, some automated balance checking process such as `C2` queries the client's balance, it will get the incorrect impression that this client has been spending too much money.

> ***Aside***
> Wells Fargo Bank actually got in trouble for doing exactly this.  They deliberately reordered transactions so that debits were processed before credits, thus maximising their ability to charge overdraft fees.

This is an example of a FIFO anomaly between replicas `R1` and `R2` and is a violation of FIFO consistency.

### Disagreements Between Replicas: Causal Consistency

> ***Causal Consistency***
> Writes that are potentially causally related (I.E. related by the ***happens before*** relation `->`) must be seen by all processes in the same order


In this situation, all the events happen in chronological order such that the ***happens before*** relation is never violated.  However, replica `R2` is missing an event in its causal history and consequently gives the wrong answer to a query.

![Replica Disagreement 3](./img/L12%20Replica%20Disagreement%203.png)

The follow sequence of events happens:

* Client `C1` deposits $100 and receives an `ack`
* Client `C2` performs a balance enquiry against `R1` who accurately reports it as \$100
* `C2` then decides to withdraw \$50, but this request is processed by replica `R2`
* Since `R2` has no record of the event that deposited \$100, it accurately, but incorrectly declines the withdrawal on the grounds of there being insufficient funds

This problem is created by the fact that `R2` is missing an event in the causal history of the request to withdraw \$50.

***Q:***&nbsp;&nbsp; Why did `C2` makes its request against `R2` instead of `R1`?
***A:***&nbsp;&nbsp; Well, in distributed systems, it is often the case that the client has no control over which replica serves its request.  Having said that, some distributed systems maintain consistency by forcing a client's requests to be served by the same replica - however, decisions like this are taken by the distributed system and lie beyond the control of the client.

### Hierarchy of Consistency Guarantees

As with fault models, consistency guarantees can be arranged in a hierarchy.

![Consistency Hierarchy](./img/L12%20Consistency%20Hierarchy.png)

This is a very incomplete list - over 50 different types of consistency have been identified!  This is mentioned, not because we will need to learn all of these consistency guarantees in this course, but because different systems make different choices about which guarantees they feel it appropriate to make.

Higher up this hierarchy is not necessarily better.  There are cases when it makes good sense to offer only weaker consistency guarantees.

## Replication Strategies That Enforce Strong Consistency

Remember that we informally defined strong consistency as the case where a client cannot tell that the data has been replicated.

### Primary Backup Replication

Here the idea is pretty straight-forward and has been around since the 1970's.  We pick a system to act as the primary, and all the other systems act as backups. This arrangement has the following advantages:

* It provides fault tolerance.  If the primary fails, then one of the backups can immediately take over.
* Since the clients only ever talk to the primary, whatever total order is used by the primary is sufficient to maintain consistency.  However, if we got rid of the division between primary and backup system and allowed any system to service client requests, then we would need to solve the harder problem of establishing a consistent total order across all these systems.


In this scenario, clients only ever interact with the primary.  When a client write message arrives at the primary, it is replicated to all the backup systems in parallel, each of which must send back an `ack` to the primary.

![Primary Backup Replication 1](./img/L12%20Primary%20Backup%20Replication%201.png)

When the primary receives `ack`s from all its replicas, it then delivers the message to itself, and finally sends an `ack` back to the client.  This is known as the ***Commit Point***.

![Primary Backup Replication 2](./img/L12%20Primary%20Backup%20Replication%202.png)

When the client wants to read a value, the answer need only come from the primary.  There is no need for reads to be broadcast to the replicas.

### Primary Backup Replication: Drawbacks

There are several drawbacks to primary backup replication:

* During a write operation, the fastest response time can be no less than the sum of the time taken for the slowest replica to send back its `ack`, plus the time taken for the primary to deliver the message to itself
* Under high load conditions, the primary becomes a bottleneck
* Having only one primary has at least two limitations:
    * Under high load situations, we cannot spin up more instances of the primary (horizontal scaling)
    * We cannot ease response time problems created by data locality

But could we do better?

Yes, we could redirect all reads to the backups and leave the primary to handle only writes.

On the surface, this looks like a good solution, but upon closer examination, we discover that we could end up with some weird timing issues and potentially start reading ***data from the future***.

How so?

If a write is issued to the primary, that write is broadcast to all the backups.  However, the backups never send their `ack`s back to the client - only the primary receives these `acks`.  Only after the primary has received `ack`s from all its backups, and has delivered the message to itself, does it then send an `ack` back to the client.

This means that if we direct a read request to a backup for data that has just been updated, but before the `ack` has reached the client (via the primary), then potentially, we could be reading data from a state held in one of the backups that is ***ahead*** of the primary.  I.E. we will be reading ***data from the future***

But we can fix this problem by making a small change to the way `ack`s are handled.

Which leads us to...

### Chain Replication

In chain replication, the last backup to receive the write request sends its `ack` not back to the primary, but directly to the client.

In Chain Replication, the process that we previously called the "Primary" is now called the "Head", and the process that acted as the last backup is now called the "Tail".  In between, there can be any number of processes that we here call simply "Backup".

The division of labour is now modified slightly:

* All write requests from clients are handled by the "Head" process
* The "Head" then passes the write instruction to the first backup in the chain
* Each backup successively passes the write request down the chain until it reaches the "Tail"
* When the "Tail" process completes the write, we know that since it is the last link in the chain, all the other replicas must ***already*** have completed their writes, so we can send an `ack` directly back to the client

![Chain Replication - Write](./img/L12%20Chain%20Replication%201.png)

This then means that should the client wish to make a subsequent read; it can direct that request to the backup from which it received the `ack`.

![Chain Replication - Read](./img/L12%20Chain%20Replication%202.png)

This is a relatively new strategy that was first published by Robbert van Renesse and Fred Schneider in a 2004 paper called ["Chain Replication for Supporting High Throughput And Availability"](./papers/chain_replication.pdf)

***Q:***&nbsp;&nbsp; But how can this be faster? The response time experienced by the client will now be the ***sum*** of the times taken for each process to complete the write and propagate the request through to the next link in the chain.  How can this then be described as *High Throughput*?

***A:***&nbsp;&nbsp; Well, to answer this question, we must first define what we mean by "Throughput".

> **Throughput**: The number of operations a system can perform per unit of time

The answer to this question also depends on the ratio of reads and writes we expect our system to handle.  For systems the perform mostly writes, then Primary Backup Replication will probably achieve higher throughput, but for systems that perform mostly reads, Chain Replication will probably achieve higher throughput.

### Chain Replication: Drawbacks

In Primary Backup replication, when the primary performs a write, the replication messages are broadcast (I.E. sent out in parallel) to all the backup processes.  Therefore, the longest wait time will be no longer than the time taken for the slowest backup to complete the write and send out its `ack`.  So, no matter how many backups you have, the worst-case scenario will never be worse than the slowest individual backup process.

However, in Chain Replication, the length of the backup chain defines the overall response time for a write to complete.  As the chain length increases, so the overall response time increases because write replication propagates sequentially down the length of the chain.

This then increases the system's ***write latency***.

What about read latency though?  Read latency for a Chain Replication system does not vary with chain length because all reads are directed to the tail.

Both of these strategies are commonly used; however, the decision as to which one will work best for you is governed primarily by the balance of reads and writes you expect your system to receive.

---

| Previous | Next
|---|---
| [Lecture 11](./Lecture%2011.md) | [Lecture 13](./Lecture%2013.md)

# Distributed Systems Lecture 13

## Lecture Given by [Lindsey Kuper](https://users.soe.ucsc.edu/~lkuper/) on April 27<sup>th</sup>, 2020 via [YouTube](https://www.youtube.com/watch?v=5oCUmo9PKaw)

| Previous | Next
|---|---
| [Lecture 12](./Lecture%2012.md) | [Lecture 14](./Lecture%2014.md)


## Primary Backup (P/B) Replication

In P/B Replication, the clients only ever talk to the primary node `P`.  Any time `P` receives a write request, that request is broadcast to all the backup nodes, which independently send their `ack`s back to the primary.

When the primary has received `ack`s from all its backups, it then delivers the write to itself and sends an `ack` back to the client.  This point in time is known as the ***commit point***.

The write latency time experienced by the client is the sum of the times taken to complete each of the following four steps (imagine we have some function `rt(From, To)` that can measure the response time between two nodes):

<code>rt(C, P) + rt(P, B<sub>slowest</sub>) + rt(B<sub>slowest</sub>, P) + rt(P, C)</code>

Irrespective of the number of backups in this system, all write requests are completed in these four steps.

![Primary Backup Replication - Writes](./img/L12%20Primary%20Backup%20Replication%201.png)

Read requests are handled directly by the primary.

![Primary Backup Replication - Reads](./img/L12%20Primary%20Backup%20Replication%202.png)


The read latency time is the sum of the time taken to complete the two steps:

`rt(C, P) + rt(P, C)`

### Primary Backup Replication: Drawbacks

There can only be one primary node; thus, it must handle all the workload.

In addition to the primary becoming a bottleneck, this arrangement does not allow for any horizontal scalability.

## Chain Replication

Chain Replication was developed to alleviate some of the drawbacks of Primary Backup Replication.

![Chain Replication - Write](./img/L12%20Chain%20Replication%201.png)

Here, the write latency time grows linearly with the number of backups and is calculated as the sum of the time taken to complete the `3 + n` steps (where `n` is the number of intermediate backups between the head and the tail):

<code>rt(C, H) + rt(H, B<sub>1</sub>) + &hellip; + rt(B<sub>n</sub>, T) + rt(T, C)</code>

So, if you have a large number of backups, the client could experience a higher latency time for each write requests.

The point however of Chain Replication is to improve read throughput by redirecting all reads to the tail.

![Chain Replication - Read](./img/L12%20Chain%20Replication%202.png)

Now the read latency time is simply the sum of the time taken to complete the two steps:

`rt(C, T) + rt(T, C)`

Here are some figures from the [Chain Replication paper](./papers/chain_replication.pdf) by Renesse and Schneider.  Looking at Figure 4 at the top of page 8

![Chain Replication Paper - Figure 4](./img/L13%20Chain%20Replication%20Paper%20Fig%204.png)

These graphs compare the request throughput times of three different backup strategies (where `t` represents the number of replicas in the system):

* ***Weak Replication***
    Client requests can be served by any replica in the system.
    Indicated by the solid line with `+` signs
* **Chain Replication**
    Client write requests are always served the head, read requests are always served the tail.
    Indicated by the dashed line with `x` signs
* ***Primary Backup Replication***
    All client requests are served the primary.
    Indicated by the dotted line with `*` signs

As you can see, Weak Replication offers the highest throughput because any client can talk to any replica.  So, this is good illustration of how throughput can be improved simply by throwing more resources at the problem. However, it must also be understood that Weak Replication cannot offer the same strong consistency guarantees as either Primary Backup or Chain Replication.

Weak Replication therefore is only valuable in situations where access to the data is *"read mostly"*, and you're not overly concerned if different replicas occasionally give different answers to the same read request.

Comparing the Chain and P/B Replication curves, notice that if none of the requests are updates, then their performance is identical. The same is true when the update percentage starts to exceed about 40%.

However, look at the Chain Replication curve.

Instead of descending in a gradually flattening curve, there is a hump at around the 10-15% mark.  This is where the benefits of Chain Replication can be seen.

By why should this improvement be seen at this particular ratio of writes to reads?

The answer here lies in understanding how the workload is distributed between the head and tail processes in Chain Replication.  According to the research done by Renesse and Schneider, their experiments showed that when 10-15% of the requests are writes, then this produces the best throughput &mdash; presumably because the workload has now been distributed evenly between the head and tail processes.

It turns out that in practice, this ratio of writes to reads is quite representative of many distributed systems that are *"out there in the wild"*.


## Dealing with Failure

If the primary process in a P/B Replication system fails, who is responsible for informing the clients that one of the backups has now taken on the role of primary?

Well, clients always need to know who to contact in the first place, and this role could be performed by some sort of coordinator acting as a communication proxy.

In the P/B Replication system, the coordinator must at least ensure that:

* Each client knows who is acting as the primary
* Each replica knows who the head is

In Chain Replication, coordination is slightly more involved in that:

* Each client must know who is acting as the head ***and*** who is acting as the tail
* Each replica needs to know who the next replica is in the chain
* Everyone must agree on this order!

### Coordinator Process

So, in both situations, it is necessary to have some sort of internal coordinating process whose job it is to know who all the replicas are, and what role they are playing at any given time.

> ***Assumptions***
>
> * Not all the processes in our system will crash.
>    For a system containing `n` processes, we are relying on the fact that no more than `n-1` processes will ever crash (Ha ha!!)
> * The coordinator process is able to detect when a process crashes.
>
> However, we have not discussed how such assumptions could possibly be true because the term *"crash"* could mean a variety of things: perhaps software execution has terminated, or execution continues but the process simply stops responding to messages, or responds very slowly...
>
> Failure detection is a deep topic in itself that we cannot venture into at the moment; suffice it to say, that in an asynchronous distributed system, perfect failure detection is impossible.

The coordinator must perform at least the following roles:

* It must know about all the replicas in the system
* It must inform each replica of the role it is currently playing
* It must monitor these replicas for failure
* Should a replica fail, the coordinator must reconfigure the remaining replicas such that the overall system keeps running
* It must inform the clients which replica(s) will service their requests:
    * In the case of P/R Replication, the coordinator must inform the clients which replica acts as the primary
    * In the case of Chain Replication, the coordinator must inform the clients which replica acts as the head and which acts as the tail

#### Coordinator Role in P/B Replication

In the event of failure in a P/B Replication system, the coordinator must keep the system running by:

* Nominating one of the backups to act as the new primary
* Informing all clients to direct their requests to the new primary
* Possibly starting a new replica to ensure that the current system workload can be handled and configuring that replica to act as a backup
* etc...

#### Coordinator Role in Chain Replication

The coordinator must perform a similar set of tasks if failure occurs in a Chain Replication system.  If we assume that the head process fails, then the coordinator must keep the system running by:

* Nominating the head's successor to act as the new head
* Informing all clients to direct their write requests to the new head
* Possibly starting a new replica to ensure that the current system workload can be handled and reconfiguring the chain to include this new backup
* etc...

Similarly, if the tail process fails, the coordinator makes the tail process' predecessor the new tail and informs the client of the change.

### What if the Coordinator Fails?

If we go to all the trouble of implementing a system that replicates data across some number of backups, but uses a single coordinator process to manage those replicas, then in one sense, we've actually taken a big backwards step because we've introduced a new *"single point of failure"* into our supposedly fault tolerant system.

So, what steps can we take to be more tolerant of coordinator failure&hellip;

* Simply spin up some replicas of the coordinator?  And should we do this in just one data centre, or across multiple data centres?
* But then how do you keep the coordinators coordinated?
* Do you have a coordinator coordinator process?  If so, who coordinates the coordinator coordinator process?

This quickly leads either to an infinite regression of coordinators, or another [Monty Python sketch](./img/very_silly.png)... (Spam! spam! spam! spam!)

This question then leads us very nicely into the next topic of ***Consensus*** &mdash; but we won't start that now.

It is amusing to notice that in Renesse and Schneider's paper, one of the first things they state is *"We assume the coordinator doesn't fail!"* which they then admit is an unrealistic assumption.  They then go on to describe how in their tests, they had a set of coordinator processes that were able to behave as a single process by running a consensus protocol between them.

It is sobering to realise that if we wish to implement both strong consistency between replicas ***and*** fault tolerance (which was the problem we wanted to avoid in the first place), then ultimately, we are forced to rely upon some form of consensus protocol.

But consensus is both ***hard*** and ***expensive*** to implement.  This difficulty might then become a factor in deciding ***not*** to implement strong consistency.  Now it looks very appealing to say *"If we can get away with a weaker form of consistency such as Causal Consistency, then shouldn't we look at this option?"*

That said, there are times when consensus really is vitally important.

---

| Previous | Next
|---|---
| [Lecture 12](./Lecture%2012.md) | [Lecture 14](./Lecture%2014.md)


# Distributed Systems Lecture 14

## Lecture Given by [Lindsey Kuper](https://users.soe.ucsc.edu/~lkuper/) on May 1<sup>st</sup>, 2020 via [YouTube](https://www.youtube.com/watch?v=WgYwBLStCbs)

| Previous | Next
|---|---
| [Lecture 13](./Lecture%2013.md) | [Lecture 15](./Lecture%2015.md)

## Recap: Strongly Consistent Replication Protocols

These all work by establishing some sort of total order on operations

* ***Primary Backup (P/B) Replication***

    The write path is one where the client talks to the primary, then the primary broadcasts that write to all the backups.  Each backup then acknowledges the primary and when all the acknowledgments have been received, the primary delivers the write to itself and acknowledges the client.
    The point at which the primary delivers the message to itself is known as the *Commit Point*.

    ![Primary Backup Replication - Write Path](./img/L12%20Primary%20Backup%20Replication%201.png)

    The read path is where the client talks directly to the primary

    ![Primary Backup Replication - Read Path](./img/L12%20Primary%20Backup%20Replication%202.png)

    If a backup crashes, it can simply be replaced by another backup; however, if the primary crashes, although a backup can take over, we must be careful to ensure that the state of the backup is not ahead of the state of the primary. In other words, the backup we are about to promote to the role of primary must not be in the process of performing writes that have not yet been acknowledged back to the client (via the now failed primary).  If this is not ensured, then promoting that backup to the role of primary might cause ***writes from the future*** to appear in the new primary, thus potentially confusing the clients.

    In order to manage this, an internal coordinator process is required that holds state about what the other processes are doing.  For instance, the coordinator must know:

    * Which nodes are up or down at any given time and what role they are playing
    * Monitoring all the nodes for failure (perhaps by some sort of ping or heartbeat mechanism)
    * Reassigning the role of a node in the event that some other node fails
    * Communicating with the clients in the event that a new node has taken over the role of primary

* ***Chain Replication***

    The write path is one where the client talks to the head of the chain.  The head then propagates the write request sequentially down the chain until it arrives at the tail node.  The *commit point* occurs when the tail node delivers the message to itself and send an `ack` back to the client.

    ![Chain Replication - Write Path](./img/L14%20Chain%20Replication%201.png)

    The read path is where the clients talk directly to the tail node.

    ![Chain Replication - Read Path](./img/L14%20Chain%20Replication%202.png)

    Similarly, in Chain Replication there also needs to be an internal coordinator process that performs all the tasks needed in P/B Replication, but additionally:

    * Knows the order of nodes in the chain
    * Can reconfigure the chain in the event of node failure
    * Informs the clients which node acts as the head and which node acts as the tail

* ***Coordinators - A Single Point of Failure?***

    The main reason for inventing these replication strategies is to mitigate the effects of process failure.  Redundant copies of a process are created so that in the event of failure, one of the copies can immediately step into the gap.  That's all very well, but without there being some coordinator process to monitor the processes doing the actual work, we're no closer to protecting ourselves against failure than when we started.

    The problem here is that the coordinator process is exactly that &mdash; a process &mdash; which means it’s just a liable to failure as any other process. So, if the coordinator fails, we're dead and everything falls apart.

    On its own, a single coordinator process is little more than a single point of failure; so, who monitors the coordinator?

    Well, we could have a coordinator coordinator; but then who monitors the coordinator coordinator? Another coordinator for the coordinator coordinator?  Hmmmm, this situation will rapidly turn into either an infinite regression of coordinator processes, or a [Monty Python sketch](./img/very_silly.png)...

    What we tend to do here is implement a replication strategy between multiple copies of the coordinator process that behave, from the perspective of an external observer, as if they were a single process.

    ***Q:***&nbsp;&nbsp; But isn't that going to be expensive and slow?
    ***A:***&nbsp;&nbsp; Yes, but if you really need strong consistency, then this is the type of approach you will need to take.

    Alternatively, you might decide that the extra overheads of time, expense and complexity are sufficiently high that you can tolerate a weaker form of consistency.


## Consensus: Making Sure Everyone Agrees

Making sure the coordinator process does not fail turns out to be a difficult problem to solve.

At the end of the previous lecture, we mentioned that in the original [Chain Replication paper](./papers/chain_replication.pdf), one of the first things Renesse and Schneider state is that *"We assume the coordinator doesn't fail!"* &mdash; and they then admit that this is an unrealistic assumption.  They then go on to describe how in their tests, they had a set of coordinator processes that were able to behave as a single process by running a consensus protocol between them.

### When Do You Need Consensus?

Assuming we have a set of processes that must all act in some coordinated fashion, then consensus will be needed in situations such as:

1. ***The Totally-Ordered (or Atomic) Broadcast Problem***
    All processes need to deliver the same set of messages in the same order

1. ***The Group Membership Problem*** or ***Failure Detection Problem***
    A group of processes must agree on some shared state (either their own, or the state of some other group of processes) &mdash; whilst at the same time, any one of these processes could be starting, going slow, crashing or restarting

1. ***The Leader Election Problem***
    One process plays a distinguished role, and all the others need to know who it is

1. ***The Distributed Mutual Exclusion Problem***
    All processes take turns in getting mutually exclusive access to some shared resource (E.G. a file)

1. ***The Distributed Transaction Commit Problem***
    All processes jointly contribute towards a transactional unit of work.  It must then be agreed upon as to whether that unit of work should be committed or aborted

All of these problems share the same common requirement &mdash; they all need to agree on some shared set of information.  Exactly ***what*** needs to be agreed on varies; it could be the order in which messages are delivered, or whether a set of processes are alive or dead, or who the leader is, or who gets access to a shared resource, or whether a transaction should be committed or aborted: but irrespective of these details, the consensus problem boils down to working out how to agree on information that constitutes  *"common knowledge"*.

What makes this really hard is the fact that faults can occur: namely ***crash faults*** or ***omission faults***.  But even in the somewhat simpler case where we only need to deal with crash faults, this problem is still really hard.

### Now Children, Don't Argue...

Why is it so hard?  Because agreement must be reached:

* In the presence of failure and asynchrony, and
* Without there being any external process to act as arbiter, and
* Without an individual participant knowing what value has been contributed by any of the other participants

So, let's say we have three processes that all need to agree on the value of a single bit - should it be `1` or `0`?  This seems like a simple enough request, but given the above constraints, this is much harder than it appears.

In simple terms, each process contributes its opinion on what this bit should be, and there are only two possible outcomes:

![Consensus Outcomes](./img/L14%20Consensus%201.png)

Irrespective of the individual contributions, all participants must agree on either a `0` or a `1`.

One approach is to use the majority opinion, and this will play a major role when we look into the implementation details, but first let's take a look at the properties that consensus algorithms ***try*** to satisfy.

## Properties a Consensus Algorithm Tries to Implement

In order for consensus to be reached, all algorithms try to implement the following properties:

* ***Termination***
    Each correct process eventually decides on a value.

    Notice that this property makes no attempt to ensure that two correct processes ***agree*** on some common value, only that each correct process will eventually output something.

* ***Agreement***
    All correct processes agree on the same value.

If these were the only two properties we needed to account for, then we could simply ignore all the input values and output some arbitrary value...  Boom! Consensus!

But whilst this vacuously conforms to the requirements of consensus, it's not going to be very useful in practice.  So, we need a third consensus property:

* ***Validity*** (or ***Integrity***, or ****Non-Triviality****)
   The agreed upon value must be one of the proposed values


The problem is that, in reality, it turns out to be impossible for a consensus algorithm to satisfy all three of these properties. This is known as the ***FLP Result*** after a paper published in 1983 by Michael Fischer, Nancy Lynch and Michael Paterson.  In simple terms:

> ***FLP Result***
> In any system where messages are sent asynchronously ***and*** crashes can occur, then it is impossible to satisfy all three properties of termination, agreement and validation.

This paper is called the ["Impossibility of Distributed Consensus with One Faulty Process"](./papers/FLP.pdf) and its practical implication is that all consensus algorithms must compromise on at least one of these properties. (A good summary of the FLP Result can be found [here](https://www.the-paper-trail.org/post/2008-08-13-a-brief-tour-of-flp-impossibility/))

The problem is that if we compromise on either the agreement or validity properties, then we will have a system that fulfils the requirements, but possibly only in a vacuous sense and will therefore not be very useful.  Consequently, consensus algorithms must compromise on termination.

With termination compromised, it means that if we get a response, it will always be one of the original input values, but it might take an infinitely long period of time to arrive at an answer...  If that's the case, then we would need to impose some sort of timeout on the consensus algorithm such that if it does not find an answer within a predetermined period of time, we try again &mdash; which also might not terminate, resulting in:

![Non-terminating Consensus](./img/L14%20Consensus%202.png)

Nothing, nada, nix.  But this is a risk we cannot avoid.

## The Paxos Consensus Algorithm

This algorithm was invented by Leslie Lamport in 1990, but it took him 8 years to get it published.  In the original paper, he used the analogy of a parliamentary procedure with laws and voting and ballots; and many people still use this terminology when explaining the algorithm.  However, he later adopted a different set of terminology that was used in his ["Paxos Made Simple"](./papers/Paxos%20Made%20Simple.pdf) paper published in Nov 2001.  This is the terminology we will use here.

Paxos is not a single algorithm; instead it is a family of algorithms.

Here, we are just going to look at the "vanilla" Paxos algorithm.  In this case, a process can act in one (or more) of three roles:

* ***Proposer***
    Proposes a value

* ***Acceptor***
    Contributes towards choosing from one of the proposed values

* ***Learner***
    Does not directly participate in negotiating the final value.  Instead, a learner simply adopts the value agreed upon by the other participants.

It is entirely possible for Paxos participants to take on two, or even three roles; but to start with, it is simplest to assign one role to one participant.

One of the first things that needs to be known by all the nodes in a Paxos system is how many acceptors are needed to form a majority.

So, if there are three processes performing the role of acceptor, then a majority is two; if there are five, then the majority is three.  This fact must be known ***in advance*** by all participating processes - you can't start running the Paxos algorithm until this knowledge has first been shared.

We must also keep these additional things in mind:

* Paxos nodes need to be able to remember what values they have already accepted, so they must have some form of persistent storage.
* Paxos is a protocol that decides upon a ***single*** value, not a sequence of values.  If you want to decide upon a sequence of values (which is often the case), then you need to run the protocol again.  There are various optimisations that can be implemented at this point but were not going to talk about those yet.  To start with, we will simply confine ourselves to the process of agreeing upon a single value.

### Paxos Algorithm: A Basic Worked Example

In this example, the participants are:

* A single proposer `P`,
* Three acceptors <code>A<sub>1</sub></code>, <code>A<sub>2</sub></code> and <code>A<sub>3</sub></code>, and
* Two learners <code>L<sub>1</sub></code> and <code>L<sub>2</sub></code>

So, the first thing to note is that a majority of acceptors in this case is two.  This fact was distributed to the participants when they started.

Knowing how many acceptors constitute a majority, the proposer `P` sends out a broadcast `prepare` message to at least the majority of acceptors.  This message does not contain the value being negotiated, instead it simply contains a proposal number that must obey the following rules:

1. The proposal number must be ***unique***.
    If the Paxos consensus algorithm is being implemented by multiple proposers, then before the algorithm starts, each of the proposer processes must have already agreed upon how they will maintain proposal number uniqueness (for instance, one proposer might use even numbers and the other, odd).
1. The proposal number must be ***higher*** than any proposal number previously used by that proposer.
    This means each proposer must keep a record of the last proposal number it used.  Each time the proposer sends out a `prepare` message, the proposal number must be incremented in such a way as to maintain uniqueness.

![Paxos 1](./img/L14%20Paxos%201.png)

In this case, the proposal number is `5`.  Remember that this is ***not*** the value upon which consensus is being sought.  It is simply a logical clock value that will be later used to identify the value upon which consensus is being sought.

The acceptor processes then look at the proposal number and ask the following question:

***Acceptor:*** *"Have I already agreed to ignore messages with this proposal number?"*

If the answer is yes, then this message is simply ignored.  However, if the answer is no, then the acceptors reply with a `promise` message containing the value of the proposal number to which they now promise to respond.

(This rule contains some subtleties that we're glossing over for now, but for the time being, we'll leave it at this)

![Paxos 2](./img/L14%20Paxos%202.png)

At this point, we've reached a milestone in the progress of the algorithm because we now have a majority of acceptors who have all agreed that they will respond to subsequent messages identified with this specific proposal number.  At this point, the acceptors still have no idea what value is going to be proposed; all they have done is agree on how to identify that as yet unseen value.

In addition to this, there can now never be a majority of acceptors who have promised to respond to any proposal number less than `5`. (A minority might still agree on some lower proposal number, but that is now of no consequence.)

In other words, we've now got enough people paying attention in order to make a decision!

Now the proposer sends an `accept` message to a majority of acceptors.  For the sake of initial simplicity, we'll choose the same set of acceptors as before.  The `accept` message carries with it both the agreed upon proposal number (`5`) and for the first time, the value upon which consensus is being sought - in this case, let's say it’s simply binary `0`.

At this point in time, we're discussing the simple case in which all the acceptors are accepting the first value they've seen in this run of the algorithm (more of that in the next lecture)

![Paxos 3](./img/L14%20Paxos%203.png)

As soon as the acceptors receive the `accept` message, they will ask themselves exactly the same question as before:

***Acceptor:*** *"Have I already agreed to ignore messages with this proposal number?"*

If yes, then the message is simply ignored.  If not however, the acceptor does two things:

1. It sends an `accepted` message back to the proposer containing both the proposal number ***and*** the accepted value.
1. It broadcasts the `accepted` message to all the learners

So, acceptor <code>A<sub>1</sub></code> responds both to the proposer and broadcasts its acceptance to all the learners.

![Paxos 4](./img/L14%20Paxos%204.png)

Likewise, acceptor <code>A<sub>2</sub></code> does the same thing in parallel.

![Paxos 5](./img/L14%20Paxos%205.png)

### At What Point is Consensus Achieved?

Consensus is reached when the majority of acceptors respond to the proposer with their `accepted` messages:

![Paxos 6](./img/L14%20Paxos%206.png)

The non-intuitive part is that although we identify this as being the point in time when consensus was reached, not everyone knows it yet!

The proposer and learners only learn that consensus has been reached ***after the fact***, because by the time the `accepted` messages arrive from the majority of acceptors, consensus has already occurred.

So, the key point here is that the moment at which consensus is reached is different from the moment when everyone finds out about it.

### What About the Details We've Skipped Over?

There are various subtleties that take place in these algorithms that, at the moment, we have simply glossed over; however, these will be dealt with in the next lecture when we look at the cases in which there is more than one proposer, and what to do in the event of process failure.  We will also look at why the Paxos algorithm is not guaranteed to terminate.

## Summary: Simplified Steps in the Paxos Algorithm

* When an acceptor gets a `prepare(n)` message, it asks *"Have I already agreed to ignore messages with the proposal number `n`?"*
    * If yes, then the message is simply ignored
    * If no, the acceptor now promises to ignore any request with a proposal number less than `n` and it replies to the proposer with a `promise(n)` message.
        (We've skipped over some details here that we'll need to revisit in the next lecture)
* Once the majority of acceptors have sent their `promise(n)` messages back to the proposer, the proposer responds by sending an `accept(n,val)` message back to the majority of acceptors.  Here, `n` is the agreed upon proposal number and `val` is the proposed value upon which consensus is sought.
    (Again, we've skipped over some details here that we'll need to revisit in the next lecture)



## Questions

***Q:***&nbsp;&nbsp; How do the acceptors learn that consensus has been reached?
***A:***&nbsp;&nbsp; Unless the acceptor is also playing the part of a learner, then it actually won't know that consensus has been reached.

***Q:***&nbsp;&nbsp; Why is this algorithm so complicated?
***A:***&nbsp;&nbsp; The algorithm's complexity is a necessary feature of it needing to be able to withstand process failure.

---

| Previous | Next
|---|---
| [Lecture 13](./Lecture%2013.md) | [Lecture 15](./Lecture%2015.md)

# Distributed Systems Lecture 15

## Lecture Given by [Lindsey Kuper](https://users.soe.ucsc.edu/~lkuper/) on May 4<sup>th</sup>, 2020 via [YouTube](https://www.youtube.com/watch?v=UCmAzWvrFmo)

| Previous | Next
|---|---
| [Lecture 14](./Lecture%2014.md) | [Lecture 16](./Lecture%2016.md)

## Course Admin...

...snip...

Read Amazon's [Dynamo](https://www.allthingsdistributed.com/files/amazon-dynamo-sosp2007.pdf) paper and Google's [MapReduce](https://static.googleusercontent.com/media/research.google.com/en//archive/mapreduce-osdi04.pdf) paper.

...snip...

### Problematic Exam Question: Chandy-Lamport Snapshot Bug

The following diagram shows a buggy implementation of the Chandy-Lamport snapshot algorithm.

Process `P2` initiates the snapshot, but then something goes wrong.  Where's the bug?

![Chandy-Lamport Snapshot Bug](./img/L15%20Chandy-Lamport%20Snapshot%20Bug.png)

The Chandy-Lamport algorithm assumes FIFO delivery of all messages &mdash; irrespective of whether they are application or marker messages; so, if we trace through the steps shown in the diagram, we can discover the bug:

* `P2` initiates the snapshot so it records its own state (the green ellipse around event `E`), then immediately sends out a marker message to `P1`
* `P1` receives the marker message and immediately records its own state (the green ellipse around events `A`, `B`, `C`, and `D`) and then sends out its marker message
* After `P2` sends out its marker message, its snapshot is complete, and it continues processing events in the normal way &mdash; resulting in event `F` sending out an application message to `P1`.

The bug is created by the fact that this diagram shows a FIFO anomaly created when the application message from `P2` event `F` ***overtakes*** the snapshot marker message.

As a result, `P1` event `D` is recorded in `P1`'s snapshot, but the event that caused it (`P2` event `F`) is missing from `P2`'s snapshot.  Thus, our snapshot is not a ***consistent cut***.

Remember that for a cut to be consistent, it must contain ***all*** events that led up to a certain point in time.  So, the inclusion of event `D` in `P1`'s snapshot is the problem because this is effectively a ***message from the future***.

This is an example of a situation in which a FIFO anomaly (out of order message delivery) leads to a causal anomaly (an inconsistent cut).

## Paxos: The Easy Parts

At the end of the last lecture, our discussion of the Paxos Algorithm got us up to here:

![Paxos Consensus Reached](./img/L14%20Paxos%206.png)

This was a very simple run of Paxos involving:

* One proposer,
* Three acceptors, and
* Two learners

In this example, the proposer `P` sent out `prepare` messages to a majority of the acceptors, which in this case, was two out of three; however, it would be been equally valid for `P` to have sent `prepare` messages to all the acceptors.  In fact, doing so would be quite smart because it mitigates against message loss, because on balance, even if one message is lost, you have still communicated with the majority of acceptors.

The same idea applies when the proposer listens for `promise` messages coming back from the acceptors.  It only needs to hear from a majority of the acceptors before it can be happy.  Exactly who those acceptors are is not important, and if it does hear back from all the acceptors then that's great, but it’s not a requirement.  It just needs to hear from a majority.

So, when we speak of a ***majority***, we are speaking of at least the ***minimum*** majority. For instance, if there are five acceptors, then the minimum majority is three: but if we hear back from four or all five, then this is not a problem.  The issue is that we must hear back from at least the minimum number of acceptors required to form a majority.

There are other subtleties involved in this algorithm that we will now go through, including what happens when there is more than one proposer.

## Milestones in the Paxos Algorithm

One thing that was mentioned in the previous lecture was that three specific milestones are reached during a run of the Paxos algorithm.  These are:

1. When the proposer receives `promise(n)` messages from a majority of acceptors.

    ![Paxos Milestone 1](./img/L15%20Paxos%20Milestone%201.png)

    A majority of acceptors have all promised to respond to the agreed proposal number `n`; and by implication, they have also promised to ignore any request with a proposal number lower than `n`.

1. When a majority of acceptors all issue `accepted(n,val)` messages for proposal number `n` and some value `val`.

    ![Paxos Milestone 2](./img/L15%20Paxos%20Milestone%202.png)

    Now, even though the other processes participating in the Paxos algorithm do not yet realise it, consensus has in fact been reached.
1. When the proposer(s) and learners receive `accepted(n,val)` messages from a majority of the acceptors.

    ![Paxos Milestone 3](./img/L15%20Paxos%20Milestone%203.png)

    It is only now that the proposer(s) and the learners ***realise*** that consensus has already been reached


## Paxos: The Full Algorithm (Mostly)

A run of the Paxos algorithm involves the following sequence of message exchanges - primarily between the proposer and acceptors:

1. ***The Proposer***
    Sends out `propose(n)` messages to at least the minimum number of acceptors needed to form a majority.  The proposal number `n` must be:
    *  Unique
    *  Higher than any previous proposal number used by ***this*** proposer

    It’s important to understand that the proposal number rules are applied to proposers ***individually***.  Consequently, if there are multiple proposers in the system, there does not need to be any agreement between proposers about what the next proposal number should be.

1. ***The Acceptor***
    When the acceptor receives a `prepare(n)` message, it asks itself *"Have I already agreed to ignore proposals with this proposal number?"*.  If the answer is yes, then the message is simply ignored; but if not, it replies to the proposer with a `promise(n)` message.

    By returning a `promise(n)` message, the acceptor has now committed to ignore all messages with a proposal number smaller than `n`.

1. ***The Proposer***
    When the proposer has received `promise` messages from a majority of acceptors for a particular proposal number `n`, it sends an `accept(n,val)` message to a majority of acceptors containing both the agreed proposal number `n`, and the value `val` that it wishes to propose.

1. ***The Acceptor***
    When an acceptor receives an `accept(n,val)` message, it asks the same question as before: *"Have I already agreed to ignore messages with this proposal number?"*.  If yes, it ignores the message; but if no, it replies with an `accepted(n,val)` both back to the proposer ***and*** broadcasts this acceptance to all the learners.

Up till now, we have assumed that there is only one proposer &mdash; but next, we must examine what happens if there are multiple proposers.

### What Happens If There Is More Than One Proposer?

In this scenario, we will make two changes.  We will run the Paxos algorithm with two proposers, and for visual clarity, since learners do not actually take part in the steps needed to reach consensus, we will omit them from the diagram.

Let's say we have ***two*** proposers <code>P<sub>1</sub></code> and <code>P<sub>2</sub></code> and as before, three acceptors. (We also have two learners, but we'll ignore them for the time being.)

Remember we previously stated that in situations where there are multiple proposers, these proposers must have already agreed on how they will ensure the uniqueness of their own proposal numbers.  So, in this case, we will assume that:

* Proposer <code>P<sub>1</sub></code> uses odd proposal numbers, and
* Proposer <code>P<sub>2</sub></code> uses even proposal numbers

So, proposer <code>P<sub>1</sub></code> sends out a `prepare(5)` message to a majority of the acceptors.  This is the first proposal number these acceptors have seen during this run of the protocol, so they are all happy to accept it and respond with `promise(5)` messages.

Proposer <code>P<sub>1</sub></code> is seeking consensus for value `1`, so it now sends out `accept(5,1)` messages and the majority of acceptors respond with `accepted(5,1)`

![Multiple Proposers 1](./img/L15%20Multiple%20Proposers%201.png)

Ok, that's fine; we seem to have agreed on value `1`.

Meanwhile in Gotham City, proposer <code>P<sub>2</sub></code> has no idea what's been going on, and decides to send out a `prepare(4)` message to all the acceptors...

![Multiple Proposers 2](./img/L15%20Multiple%20Proposers%202.png)

The `prepare(4)` message arrives at acceptors <code>A<sub>1</sub></code> and <code>A<sub>2</sub></code> ***after*** they have already agreed on proposal number `5`.  Since they are now ignoring proposal numbers less than `5`, they simply ignore this message.

Acceptor <code>A<sub>3</sub></code> however has not seen proposal number `4` before, so it happily agrees to it and sends back a `promise(4)` message to proposer <code>P<sub>2</sub></code>.

Proposer <code>P<sub>2</sub></code> is now left hanging.

It sent out `prepare` messages to all the acceptors but has only heard back from a minority of them.  The rest have simply not answered, and given the way asynchronous communication works, <code>P<sub>2</sub></code> cannot know ***why*** it has not heard back from the other acceptors.  They could have crashed, or they might be running slowly, or, as it turns out, the other acceptors have already agreed to <code>P<sub>1</sub></code>'s proposal and are now having his babies...

So, all <code>P<sub>2</sub></code> can do is wait for its timeout period, and if it doesn't hear back within that time, it concludes that proposal number `4` was a bad idea and tries again.  This time, <code>P<sub>2</sub></code> shows up in a faster car (proposal number `6`).

![Multiple Proposers 3](./img/L15%20Multiple%20Proposers%203.png)

But wait a minute, consensus (milestone 2) has ***already*** been reached, so the acceptors now have a problem because:

* Acceptors cannot go back on their majority decision
* Acceptors cannot ignore `prepare` messages with a ***higher*** proposal number

So, here's where we must address one of the subtleties that we previously glossed over.

Previously, we stated only that if an acceptor receives a `prepare` message with a ***lower*** proposal number, it should simply ignore it.  Well, OK, that's fine.

But what about the case where we receive a proposal number that is ***higher*** than the last one?  Here is where we need to further qualify ***how*** that `prepare` message should be handled.

In this case, each acceptor must consider the following situation:

> *"I've already promised to respond to proposal number `n`,
> but now I'm being asked to promise to respond to proposal number `n+1`"*

How the acceptor reacts now depends on what has happened in between receiving the `prepare(n)` message and the `prepare(n+1)` message.

Either way, the acceptor cannot ignore the higher proposal number, so it is going to send out some sort of `promise` message; but this time, the acceptor must consider whether it has already accepted a value based on some earlier, lower proposal number.

* If no, then we accept the new proposal number with a `promise(n+1)` message as normal
* If yes, then we accept the new proposal number with a `promise(n+1, ...)` message, but in addition, we are obligated to tell the new proposer that we've already accepted a value using an older proposal number.

In the latter case, you can see that the `promise` message needs to carry some extra information.

In the above example, acceptor <code>A<sub>1</sub></code> has already agreed with proposer <code>P<sub>1</sub></code> that, using proposal number `5`, the value should be `1`; but now proposer <code>P<sub>2</sub></code> comes along and presents proposal number `6` to all the acceptors.

![Multiple Proposers 4](./img/L15%20Multiple%20Proposers%204.png)

So, in this specific situation, acceptor <code>A<sub>3</sub></code> responds simply with `promise(6)` because although it previously agreed to proposal number `4`, nothing came of that, and it has not previously accepted any earlier value.

Acceptors <code>A<sub>1</sub></code> and <code>A<sub>2</sub></code> however, must respond with the message `promise(6,(5,1))`.

This extra information in the `promise` message effectively means: *"Ok, I'll move with you to proposal number `6` but understand this: using proposal number `5`, I've already accepted value `1`"*.

### So, What Should A Proposer Do with Such a Message?

Previously, we said that when a proposer receives sufficient `promise(n)` messages, it will then send out `accept(n,val)` messages.  But here's where our description of the protocol needs to be refined.  What should the proposer do if, instead of receiving a `promise(n)` message, it receives a <code>promise(n,(n<sub>old</sub>,val<sub>old</sub>))</code> message?

In our example, proposer <code>P<sub>2</sub></code> has received three `promise` messages:

* A straight-forward `promise(6)` from <code>A<sub>3</sub></code>, and
* Two `promise(6,(5,1))` messages from <code>A<sub>1</sub></code> and <code>A<sub>2</sub></code>

Proposer <code>P<sub>2</sub></code> must now take into account that using proposal number `5`, consensus has already been reached on value `1`.

In this case, both `promise` messages contain the value `1` that was agreed upon using proposal number `5`; however, it is perfectly possible that <code>P<sub>2</sub></code> could receive multiple `promise` messages containing values agreed on by proposal numbers older than `5`.

So, the rule is this: proposer <code>P<sub>2</sub></code> must look at all the older, already agreed upon values, and chose the value corresponding to the most recent, old proposal number.

This is pretty ironic (and amusing) really because proposer <code>P<sub>2</sub></code> now has no choice over what value to propose.  It is constrained to propose the one value upon which consensus was most recently reached!  So, the fact that it wants to send out its own proposal is somewhat redundant, because the only value it can propose is one upon which consensus has already been reached...

So, now we must revise rule 3 given above.  Previously we stated:

>  When the proposer has received `promise` messages from a majority of acceptors for a particular proposal number `n`, it sends an `accept(n,val)` message to a majority of acceptors containing both the agreed proposal number `n`, and the value `val` that it wishes to propose.

But now we understand that the proposer does not have complete liberty to send out the value ***it wishes*** to propose; instead, it must first consider:

* If I have received any `promise` messages containing old agreed values, then I am obligated to propose the most recently agreed value
* If I have received only simple `promise(n)` messages, then I am free to propose any value I like

So now, <code>P<sub>2</sub></code> can only send out the message `accept(6,1)`.

![Multiple Proposers 5](./img/L15%20Multiple%20Proposers%205.png)

Notice that <code>P<sub>2</sub></code> has not had to use the earlier proposal number `5`, but it was constrained to propose the value `1`, because this value has already been agreed upon.

So, what do the acceptors do now?  They simply invoke rule 4 above and respond with `accepted(6,1)`.

![Multiple Proposers 6](./img/L15%20Multiple%20Proposers%206.png)

Let's isolate the messages that were exchanged between proposer <code>P<sub>2</sub></code> and acceptor <code>A<sub>3</sub></code>.

![Multiple Proposers 7](./img/L15%20Multiple%20Proposers%207.png)

<code>A<sub>3</sub></code> only sees the following exchange of messages.

* <code>P<sub>2</sub></code> first tried proposal number `4`, but nothing came of that
* <code>P<sub>2</sub></code> tried again with proposal number `6`
* <code>A<sub>3</sub></code> went with the highest proposal number (`6`) and subsequently agreed to accept value `1`

As far as <code>A<sub>3</sub></code> is concerned, it thinks that value `1` was <code>P<sub>2</sub></code>'s idea.  It has no clue that <code>P<sub>2</sub></code> was proposing a value already agreed upon by others.

---

| Previous | Next
|---|---
| [Lecture 14](./Lecture%2014.md) | [Lecture 16](./Lecture%2016.md)

# Distributed Systems Lecture 16

## Lecture Given by [Lindsey Kuper](https://users.soe.ucsc.edu/~lkuper/) on May 6<sup>th</sup>, 2020 via [YouTube](https://www.youtube.com/watch?v=h8wGZVOh43c)

| Previous | Next
|---|---
| [Lecture 15](./Lecture%2015.md) | [Lecture 17](./Lecture%2017.md)


## Course Admin

...snip...

### Review of Question in the Midterm Exam

Lots of people struggled with this question in the midterm exam, and since it is a fundamental concept, if you don't understand this, you'll struggle later with other concepts based on it.

The question was this: *"In a distributed system, what should a physical clock be used for and what should it not be used for?"*

So, what are physical clocks good for in a distributed system?

We spoke of two types of physical clock:

* A time-of-day clock
* A monotonic clock

These two types of physical clock stand in contrast to a logical clock.

| | Time-of-day Clock | Monotonic Clock
|---|---|---|
| Marking points in time | ![Neutral emoji](./img/emoji_neutral.png)<br>OK for processes running on a single system, but not much good in distributed systems because there can be no shared clock. | ![Sad emoji](./img/emoji_sad.png)<br>Completely useless because they are simply counters that increment from some ["unspecified point in the past"](https://pubs.opengroup.org/onlinepubs/9699919799/basedefs/V1_chap04.html#tag_04_16) which is unique to each machine (E.G. Nanoseconds since system start).<br>Monotonic clock values from different machines cannot be meaningfully compared.
| Durations/Intervals | ![Sad emoji](./img/emoji_sad.png)<br>The problem here is that time-of-day clocks can jump around due to daylight saving time and leap seconds.| ![Smiley emoji](./img/emoji_smiley.png)<br>On a single machine, these are great because they only go forward from some "unspecified point in the past".

***Q:***&nbsp;&nbsp; So, what are physical clocks good for in distributed systems?
***A:***&nbsp;&nbsp; Timeouts!

Timeouts (measured using a monotonic clock) are used in a wide variety of places for failure detection.  E.G. A Paxos proposer uses a timeout when waiting for responses to a new proposal number.

***Q:***&nbsp;&nbsp; So, what are physical clocks ***not*** good for in distributed systems?
***A:***&nbsp;&nbsp; Measuring the order of events

Why?  Because if you try to determine the order in which a sequence of events have occurred by marking each event's point in time, we will run into problems when we try to compare time values recorded on different machines.

If we use time-of-day clocks, then these will only be comparable in a very course sense because they are prone to jumping around due to factors such as daylight-saving time and leap seconds.

If we try to use monotonic clock values, then things get even worse because they are simply counters from some *"unspecified point in the past"*; thus, it is meaningless to compare values coming from different machines.

So physical clocks are simply not suitable for measuring the order of events that occurred on different machines.

## Paxos: Nontermination

All consensus algorithms try to satisfy the following three properties:

* Termination
* Validity / Integrity
* Agreement

We have already stated that for a consensus algorithm running in a distributed system where failures are possible, it is impossible to implement all three properties.  This is known as the [FLP Result](./papers/FLP.pdf).

Therefore, all consensus algorithms must compromise on one these properties, and Paxos compromises on the termination property &mdash; which risks cases where non-termination could occur.

So, what kind of situation would lead to non-termination?

Simply put, the Paxos algorithm will not terminate in cases where multiple proposers contend with each other for the proposed value.

Consider this sequence of events:

![Paxos Nontermination 1](./img/L16%20Paxos%20Nontermination%201.png)

* Proposer <code>P<sub>1</sub></code> sends out `prepare(5)` messages to acceptors <code>A<sub>1</sub></code> and <code>A<sub>2</sub></code>
* Neither acceptor has seen this proposal number yet, so they both respond with `promise(5)`
* But quite independently of this, proposer <code>P<sub>2</sub></code> sends out its `prepare(6)` messages to acceptors <code>A<sub>2</sub></code> and <code>A<sub>3</sub></code>
* Even though acceptor <code>A<sub>2</sub></code> has already promised to ignore proposal numbers less than `5`, it has not yet accepted any values at this proposal number, so it's not a problem if it now promises to accept this new, higher proposal number
* Acceptor <code>A<sub>3</sub></code> is receiving its first proposal number, so it happily promises to ignore proposal numbers lower than `6`.

Unaware of what the other acceptors have just agreed to, proposer <code>P<sub>1</sub></code> now sends out its `accept(5,"foo")` message thinking that it already has agreement from the majority of acceptors.

![Paxos Nontermination 2](./img/L16%20Paxos%20Nontermination%202.png)

* Acceptor <code>A<sub>1</sub></code> is still on proposal number `5`, so it sends back an `accepted(5,"foo")` message as expected
* But due to proposer <code>P<sub>2</sub></code>'s earlier `prepare(6)` message (that proposer <code>P<sub>1</sub></code> knows nothing about), acceptor <code>A<sub>2</sub></code> has now promised to ignore messages with a proposal number lower than `6`.
* So, proposer <code>P<sub>1</sub></code> sits there waiting for a response.  It fails to receive responses from the majority of acceptors, and eventually times out.
* Not being one to give up, <code>P<sub>1</sub></code> sends out another `prepare` message, this time for the higher proposal number `7`.
* Just as before, acceptors <code>A<sub>1</sub></code> and <code>A<sub>2</sub></code> are happy to oblige and respond with `promise(7)` messages.

Now, unaware of all the collusion going on between <code>P<sub>1</sub></code> and the acceptors, <code>P<sub>2</sub></code> sends out its `accept(6,"bar")` message.

![Paxos Nontermination 3](./img/L16%20Paxos%20Nontermination%203.png)

* Acceptor <code>A<sub>3</sub></code> happily responds with `accepted(6,"bar")`
* But since acceptor <code>A<sub>2</sub></code> has already promised to ignore messages with a proposal number lower than `7`, it simply ignores <code>P<sub>2</sub></code>'s `accept` message
* <code>P<sub>2</sub></code> hangs around waiting for a majority of acceptors to respond, but this never happens, so it times out
* Not being one to give up, <code>P<sub>2</sub></code> sends out another `prepare` message, this time for the higher proposal number `8`.


And on and on we can go here - with each proposer continually trying to outbid the others.  Consensus will never be reached.

This is known as the ***"Duelling Proposers Problem"***.

In this case, we have used three acceptors, but actually only two would have been sufficient to demonstrate non-termination.

### So, Why Not Just Have One Proposer?

All of this confusion seems to be created by the fact that we have multiple proposers all trying to outbid each other.  Couldn't we solve this problem simply by restricting the number of proposers to one?

Well, let's see what would happen if we tried to enforce that there is exactly one proposer:

* When considering fault tolerance, if we ensure that the proposer always writes its data to persistent storage, then even if it dies, we can nominate another process to act as the new proposer, and then we'll be able to carry on as before.
* But hang on, how do we decide which node will take over?
* Oh, that's a leader election problem...
* And to solve a leader election problem we need consensus
* And if we use Paxos to elect a new leader, that algorithm might never terminate

And we're back to where we started...

So, we cannot insist on there being only one proposer because our consensus algorithm depends on a consensus algorithm.  For instance, if we relied on Paxos to determine a new leader, then we're depending on an algorithm that might never terminate.

Some consensus algorithms go through a phase in which they elect a leader (which requires consensus) and then that leader becomes the sole proposer.  This does not eliminate the possibility of the *Duelling Proposers Problem* (because it could still occur during leader election phase); however, it confines non-termination to the leader election phase and removes it from the value proposal phase.

This is strategy for reducing risk, not removing it.

## Would It Ever Make Sense to Compromise on a Different Property?

So far, we have seen that the Paxos algorithm values *agreement* and *validity* over termination; therefore, it sees non-termination as an acceptable risk in the quest to achieve agreement and validation.

But is there another way we could work here?

### What Would Happen if we Compromised on Agreement?

Leader election is one situation in which it is more important for the algorithm to terminate than it is for everyone to agree.

So now we could elect the proposer in the Paxos algorithm using a different leader election algorithm that risks producing multiple values, but we know will terminate.  If this algorithm elects a single proposer most of the time, then that's great; however, if it elects multiple proposers, then this is also OK because we know that Paxos can work with multiple proposers.

So, this leads us nicely into the next topic - Multi-Paxos.

## Multi-Paxos

All the runs of the Paxos algorithm that we've looked at so far are concerned with deciding on a single value.  If we want to decide on a sequence of values, then the Paxos algorithm must be rerun.

As it turns out, agreeing on a sequence of values is a widespread problem; for example, in [lecture 14](./Lecture%2014.md#when-do-you-need-consensus), we looked at a list of problems that all require consensus, and one of these was the problem of Totally-Ordered Broadcast

> Remember that in Totally-Ordered Broadcast, we need to ensure that a set of processes all deliver a set of messages in the ***same order***.  Therefore, consensus must be reached on which message should be delivered first, which second and which third etc.
>
> This turns out to require us to make the same decision over and over for each message in the queue.

The problem here is that in the best case, in order for Paxos to decide on a single value, a minimum of two round trips are needed between the proposer and the majority of acceptors.  In the case that we have three acceptors, this will require a total of 8 messages to be exchanged between the proposer and at least two of the acceptors.

![Minimum Number of Message Exchanges Needed by Paxos](./img/L16%20Paxos%20Minimum%20Msg%20Exchange.png)

In order for this minimum to be achieved, it is assumed that:

* All processes are correct (I.E. they don't crash or exhibit some weird Byzantine behaviour)
* Only one proposer is involved

However, what's the downside here?  Having to repeat this message exchange sequence over and over again is not very efficient!

### Paxos Algorithm Phases

A full run of the Paxos algorithm is divided into two distinct phases:

* The prepare/promise phase, and
* The accept/accepted phase

![Paxos Algorithm Phases](./img/L16%20Paxos%20Phases.png)

However, we can apply an optimisation here.

After a single run of the Paxos algorithm has completed, the proposer knows that the majority of acceptors have agreed to its last proposal number; therefore, if we require consensus on another value, we can skip the prepare/promise phase and simply repeat the accept/accepted phase for the next value.

For Multi-Paxos to work successfully however, we need to make two assumptions:

1. The proposal number does not change (hopefully because there is only one proposer)
1. The proposer process does not crash

Since we want consensus on a sequence of values, we can arbitrarily add our own additional sequence number into the `accept` messages to keep track of this value.


### Multi-Paxos in Action

So, let's say we want consensus on the sequence of values `"foo"` and `"bar"`.  We still need to go through the prepare/promise phase, but we only need to do that once.  After that, we can simply repeat the accept/accepted phases:

![Multi-Paxos](./img/L16%20MultiPaxos.png)

Notice that the `accept` and `accepted` messages now contain an additional sequence number after the value:

* `prepare(5)` is answered with `promise(5)` as normal
* <code>P<sub>1</sub></code> now sends an `accept(n, val, seq)` message where:
    * `n` is the promised proposal number,
    * `val` is the value upon which consensus is being sought, and
    * `seq` is some arbitrary sequence number


Ok, but what happens if we do have a second proposer who starts injecting their own proposal numbers?

In this case, we will not be able to repeat the second phase because some of the acceptors will be ignoring <code>P<sub>1</sub></code>'s `accept` messages.  Now, <code>P<sub>1</sub></code> will simply time out and start the prepare/promise phase again.  In other words, nothing breaks and Multi-Paxos gracefully degenerates back to regular Paxos &mdash; however, we do not expect this situation to happen very often.

Using this approach, Totally-Ordered Delivery can be achieved by a set of processes using the (Multi-)Paxos consensus algorithm between them to agree on message delivery order.

## But Is This the Whole Story?

Here's another type of consensus algorithm:

* We have one acceptor process
* We have multiple proposer processes
* Each proposer sends their value to the acceptor who somehow decides which value to accept
* Whatever value is returned from the acceptor is now the *"agreed"* value.

Boom! All the required properties have been fulfilled!

Why can't we just do this?

Well how about fault tolerance?  What if our single acceptor process crashes?

### Tolerating Crash Faults

As we've mentioned before, the [FLP result](./papers/FLP.pdf) demonstrates that if we need to be able to withstand crashes, then it is impossible to have a consensus algorithm that exhibits all three properties of agreement, validity and termination.

Consensus algorithms tend to be designed in a very defensive way in order to make them as robust as possible in the event of processes crashing &mdash; which is part of the reason for all the complexity in the Paxos algorithm.

#### Acceptor Failure

In the examples we've worked with so far, we have always had three acceptors.  So how many of these acceptors could crash without bringing Paxos down?

* If we start with three acceptors, then two is a majority
* If one acceptor crashes, we are still left with a majority of the original three
* Therefore, Paxos still works

Similarly, if we have five acceptors, then by the above reasoning, we can tolerate up to two acceptors crashing.

In general then, if `f` is the maximum number of failed acceptors we can tolerate, then we must start with a total of `2f + 1` acceptors.

#### Proposer Failure

Again, if we start with the idea that `f` is now the number proposer failures we are able to tolerate, then we must decide how many proposers our system must have when it starts.

We know from the above discussion, that Paxos actually works very well if there is only one proposer, so 1 is the minimum we can work with.  If we can tolerate `f` failures, then it is clear that our system should start with at least `f + 1` proposers.

This is the degree to which Paxos can tolerate crash faults.

### Tolerating Omission Faults

How well does Paxos tolerate omission faults?

What happens if a proposer sends a `prepare` message to all the acceptors, but for some reason that message never arrives at some of those acceptors?

Well, the proposer only needs to hear back from a majority of acceptors; so, if a `prepare` message does not arrive at one out of three acceptors, then this will not create a problem.  The proposer will still hear back from two out of three which is a majority.

Ok, let's ramp up the severity &mdash; what if the proposer sends a `prepare` message to all three acceptors, and all three messages got lost?

Again, other than slowing things down, nothing bad would happen because after waiting for its time out period, the proposer would simply try again with a new proposal number.  At this point, we might run into a non-termination problem, but that is not an omission fault.

So Paxos does OK in the case of omission faults - it might not terminate, but as we've seen with the *"Duelling Proposers Problem"* shown above, we don't need to experience message loss in order for non-termination to occur.

## Other Consensus Protocols

Here we will mention a few other consensus protocols.  We will not look into them in any detail, but since we have had a detailed look at Paxos, you now have a good foundation from which to study these algorithms on their own.

These consensus algorithms all have a couple of common features:

1. They are designed to achieve consensus on a sequence of values, not just one - which makes them more like Multi-Paxos than basic Paxos
1. They all include leader-election as a fundamental part of the protocol

These consensus protocols are:

* ***Viewstamped Replication (VSR)***
    Developed by Brian Oki and Barbara Liscov (1988) and documented in this [paper](./papers/VSR.pdf).
    An explanation of this protocol by Bruno Bonacci is available on YouTube [here](https://www.youtube.com/watch?v=1EzNa-zAYS8)

* ***ZAB (Zookeeper Atomic Broadcast)***
    Developed at Yahoo in the late 2000's as part of their Open Source Zookeeper system often used for configuration management.
    A paper by André Medeiros on the theory and practice of ZAB is available [here](./papers/ZAB.pdf).

* ***Raft***
    Developed by Diego Ongaro and John Ousterhout in 2014.  The whole point of Raft is understandability.
    It is very well explained on their website <https://raft.github.io>.

Also, [this paper](./papers/Paxos%20vs%20VSR%20vs%20ZAB.pdf) provides a useful comparison of the Paxos, VSR and ZAB algorithms.


## Active and Passive Replication

The following statement is confused:

*"Primary Backup replication is active replication"*

To remove this confusion, we should first define exactly what these terms mean.

Let's say we're doing Primary Backup on a replicated back account.  This is the situation we looked at in [lecture 12](https://github.com/ChrisWhealy/DistributedSystemNotes/blob/master/Lecture%2012.md#primary-backup-replication).

We receive an instruction to deposit \$50 into an account that already has a balance of \$20.  But there are two ways we could implement this deposit operation.

### Active Replication

We could apply the deposit instruction to the primary `P` and then broadcast that instruction to both backups.  These backups then apply that instruction to their own replicas of the account.

When the `ack`s from all the backups have been received by the primary, the primary delivers the message to itself and finally sends an `ack` to the client.

![Primary Backup Replication 1](./img/L16%20Primary%20Backup%201.png)

Now processes `P`, <code>B<sub>1</sub></code> and <code>B<sub>2</sub></code> hold identical state because they all applied the same instruction to the same initial account balance

This is active replication because the operation has been executed on every replica where we want it to take effect.

### Passive Replication

Alternatively, the primary `P` could execute the deposit instruction, but not commit it yet.

Now that `P` knows what the new balance is, instead of sending the deposit instruction, it simply sends the new account balance to the backups.

![Primary Backup Replication 2](./img/L16%20Primary%20Backup%202.png)

The backups simply apply store the new state of the account and send back their `ack` messages.  Then, as before, the primary sends an `ack` to the client.

This is passive replication because the operation is executed only on the primary node, and then state update messages are sent to the backups.

### These Are Both Examples of Primary Backup Replication

Irrespective of whether an active or passive strategy is used, both approaches shown here are examples of primary backup replication:

* The clients still communicate only with the primary
* The primary executes the required operation and communicates (in some way) with the backups
* The backups all acknowledge that they have successfully processed whatever message was sent to them
* Lastly, the primary commits the work itself and sends an acknowledgement back to the client

Exactly what type of message the primary sends to the backups is an internal implementation detail &mdash; as far as the external observer is concerned, it’s all primary backup replication

### Should We Choose Active or Passive?

So, what would cause us to choose one approach over the other?

Well, we need to consider factors such as the size of the resulting updated state, and the cost of the computation needed to derive that updated state.

For instance, what should we do if the primary receives the operation *"Increment everyone's account balance by one cent"* &mdash; and we have a million bank accounts?  In this case, the size of the state change would be huge, so passive backup would not be a good approach.

The following factors should be evaluated when deciding between active and passive replication:

* The update requires me to run a computation that costs `t` units of time
* I have `n` nodes on which this update must be applied
* The new state created by the computation is `s` bytes in size
* The network connecting the nodes transmits data at a rate of `r` bytes per unit of time

The question then boils down to crunching these numbers in order to work out which option gives me the quickest result.  In general, then:

* If an operation results in a large state change, then active replication is probably going to be better because sending the operation over the network uses up much less bandwidth than sending the changed stated
* If the cost of an operation is high, then passive replication is probably going to be better because the cost of computation is incurred only once (on the primary)

Active replication is also known as *"State Machine Replication"*

---

| Previous | Next
|---|---
| [Lecture 15](./Lecture%2015.md) | [Lecture 17](./Lecture%2017.md)

# Distributed Systems Lecture 17

## Lecture Given by [Lindsey Kuper](https://users.soe.ucsc.edu/~lkuper/) on May 8<sup>th</sup>, 2020 via [YouTube](https://www.youtube.com/watch?v=-a1Ua1P9cNg)


| Previous | Next
|---|---
| [Lecture 16](./Lecture%2016.md) | [Lecture 18](./Lecture%2018.md)


## Amazon Dynamo

Please read the [Amazon Dynamo Paper](./papers/Dynamo.pdf) in preparation for the next lecture.  In the world of distributed systems, this is one of the most influential papers of the last 20 years, and also one of the most highly cited.

Before we discuss the paper however, we'll first look at some different, preparatory topics.

## Strong Consistency Between Replicas

So far, we have seen that strong consistency can be achieved using backup strategies such as Primary Backup Replication or Chain Replication.  We also saw that ultimately, strong consistency relies on consensus because in order to achieve fault tolerance, you need to have a coordinator, and under the surface, that coordinator is really a collection of processes acting as one.

The fundamental point here is this:

> If you want to implement a system that is strongly consist ***and*** you need it to tolerate node failure, then you ***must*** implement some sort of consensus mechanism.

The thing about strong consistency is that it is hard to enforce.  Consider the good old total-order anomaly example that we've seen so many times:

![Total-Order Anomaly](./img/L6%20Total%20Order%20Anomaly.png)

This anomaly is ***not*** a causal anomaly.  If it were a causal anomaly, then either the order of events leading up to a particular point in time would have become scrambled, or parts of that causal history are missing.  Such anomalies can be fixed by adding a vector clock to each message, thus allowing the delivering process to establish the correct message order.

But as we can see here, a total-order anomaly cannot be solved simply by adding vector clocks to the messages:

![Total-Order Anomaly with Vector Clocks](./img/L17%20TO%20Anomaly.png)

All the vector clocks have been incremented correctly, but if we compare these vector clock values between replica `R1` and replica `R2`, we cannot say that one is greater than the other.

So, using vector clocks alone, we are left in a situation where these two final events in `R1` and `R2` are causally independent making the total order of these messages is ***undecidable***.

So, what do we do here?

One option is to run a consensus algorithm, but as we have seen, such algorithms are expensive and might not terminate.  So, a better solution is to have a situation in which the order in which messages arrive at the replicas doesn't matter.

## Eventual Consistency

So, in what situation does the order of two updates not matter?  One situation is where two, unrelated values are being updated by two different clients.

![Eventual Consistency](./img/L17%20Eventual%20Consistency.png)

***Q:***&nbsp;&nbsp; Given that the informal definition of strong consistency is that the clients cannot tell that the data has been replicated, is this form of consistency ***strong***?
***A:***&nbsp;&nbsp;  No, this is not strong consistency because in between these writes, the clients can still do reads, and depending on the timing of the reads and writes and which replica they read from, this would allow them to discover differences in the state of `x` and `y`.

In spite of the fact that clients can discover differences in the data, these differences are short-lived and eventually consistency is achieved.  Whilst this is not perfect, it is a much better situation than having two replicas disagree with each other.


![Eventual Consistency](./img/Eventual%20Consistency.jpg)

So, informally, we say:

> ***Eventual Consistency***: Replicas eventually agree if clients stop submitting updates

***Q:***&nbsp;&nbsp; So, what sort of property is eventual consistency?  Is it a liveness property, or a safety property?
***A:***&nbsp;&nbsp; It’s a liveness property because it cannot be violated in a finite execution.

Even in the case of the total-order anomaly we saw earlier where the two replicas disagreed on the value of `x`, we could still implement some message passing mechanism that would resolve this disagreement and achieve eventual consistency.

So eventual consistency is a very different consistency model than the other models we looked at so far such as:

* Strong consistency
* Causal consistency
* FIFO consistency
* etc...

All of these consistency models are ***safety*** properties (because you can violate them in a finite execution), whereas eventual consistency is a ***liveness*** property.

With eventual consistency, the clue is in the name ***eventual***.  This refers to the fact that consistency will be achieved, but only after  some unspecified period of time has elapsed &mdash; so, you could wait forever without violating this condition.

The term "*eventual consistency*" has been something of a buzzword in the last 15 years, and has often been mistakenly lumped together with strong, causal and FIFO consistency.  This is not the case because these are two different categories of property.

## Strong Convergence

Strong convergence is a safety property that is defined as:

> Replicas that have delivered the same ***set*** of updates have equivalent state

This is the situation illustrated by the diagram above.  Even though the updates to `x` and `y` arrived in a different order, the same set of updates arrived and both replicas eventually ended up holding the same state.

Thus, these replicas are said to be ***strongly convergent***.

***Strong Eventual Consistency*** = Eventual consistency + Strong convergence

Here we have combined the liveness property of eventual consistency with the safety property of strong convergence.


That's all very well, but doesn't this scenario seem rather unrealistic?  After all, we have assumed that client `C1` will only update key `x` and client `C2` will only update key `y`.  This doesn't really smell like a real-life situation.

So how can we allow strong convergence ***and*** allow both clients to update the same key?

Well, we could implement a consensus protocol, but that's a pretty heavyweight solution.  How could we do this without needing to go to these lengths?

So, here's an idea...  What if we kept both updates and instead of binding a single value to the key name, instead we bind a set of values:

![Strong Convergence 1](./img/L17%20Strong%20Convergence%201.png)

Since sets are unordered, the values held in each replica are considered equivalent.

The only issue now is that any client wanting to read `x` will get back a set of values rather than a single value.  It is now up to the client to perform conflict resolution and decide which value is authoritative.  The manner in which this conflict is resolved is application specific.

Conflict resolution aside, this situation conforms to the requirements of strong convergence because after the same set of updates have been applied by both replicas, they have converged to the same state. (The compromise here is on agreement about which value is the right one).

This situation is deeply important to Amazon as it concerns the replication of shopping carts.

Consider the situation where you want to add items to your shopping cart from two devices, your laptop and your phone.

![Amazon Shopping Cart 1](./img/L17%20Amazon%20Cart%201.png)

* From your laptop on the left, you add a book to your shopping cart.
    This information is added to shopping cart 1 and then replicated over to shopping cart 2

* From your phone on the right, you also add a pair of jeans.
    This information is added to shopping cart 2 and then replicated over to shopping cart 1

By the time these additions to the shopping cart have been processed, the state of your shopping cart in both replicas is the same.

But the key point here is that each replica holds ***two different versions*** of the shopping cart.  One version contains only the book, and the other only the jeans.

Now when a client performs a read of the shopping cart, it gets back both versions of the cart.

![Amazon Shopping Cart 2](./img/L17%20Amazon%20Cart%202.png)

So, what should the client do here to resolve this conflict?

Under the specific conditions of multiple devices adding items to the same shopping cart, it is not accurate to describe this situation as a ***conflict***.  In this specific situation, the actual state of the shopping cart is simply the union of the two sets, and this point is discussed in the Dynamo paper.

![Amazon Shopping Cart 3](./img/L17%20Amazon%20Cart%203.png)

However, simply forming the union of two versions of the data is not necessarily the correct approach in all situations.

This is an example of a wider problem called *"Application-Specific Conflict Resolution"*, and this is a huge topic in its own right!

At this point, if you have questions related to how such conflicts can be resolved, that's not surprising &mdash; but unfortunately, we don't have time at the moment to look more deeply into this topic.

## Network Partitions

Another concept mentioned in the Dynamo Paper is that of ***Network Partitions***.

A network partition is where in a network of communicating computers, two subsets of computers can each talk to each other within their own subset, but the two subsets cannot communicate with each other.

![Network Partition 1](./img/L17%20Network%20Partition%201.png)

Rarely, it is also possible for one-way communication to happen across the partition boundary.

One significant issue for distributed systems is that network partitions can occur randomly, whilst communication between systems is taking place.

Fortunately, we have a way of talking about network partitions using the fault models we have already discussed.  Here, we can use the omission model and consider any message that attempts to cross the partition boundary as being lost.

> ***Aside***
>
> Don't confuse the concept of network partitioning with data partitioning.
>
> A network partition is a transient fault that disrupts or breaks communication between parts of a network &mdash; and this is generally considered to be a bad thing
>
> Data partitioning (also known as ***sharding***) is where you have more data than will fit into one machine, so you need to split the storage across multiple machines.  This requires you to decide which data will live where.
>
> Data partitioning is not intrinsically bad, but network partitions are.

## Availability

Dynamo claims to be a *"highly available"* system.  This is a relative term that describes the level of availability offered by the system to client requests.  Availability is best understood not as a binary property that is either present or absent, but as variable quality that sits somewhere on a sliding scale or a spectrum.

Perfect availability (which is not possible in reality) is the situation in which every request receives a response.  Ideally, we would also like to add that every request receives a ***fast*** response, but for the purposes of this discussion, we don't need to worry too much about response times.

Consider what would happen in a Primary Backup Replication scenario where the primary receives a write request, but then a network partition suddenly appears between the primary and its backups.

![Network Partition 2](./img/L17%20Network%20Partition%202.png)

The primary has now lost contact with its backups, so what should it do?

Should the primary simply acknowledge the write back to the client, then queue up the write to be sent to the backups as and when the network partition heals?

Well, yes, but this raises further issues...

1. Even though network partitions are generally short-lived events, you cannot say for certain how quickly they will heal
1. What if the primary crashes?  Now we have a whole load of issues:
    * If a backup now has to take over the role of the primary, data will have been lost because whichever backup takes over will be out of sync
    * We've already sent an acknowledgement to the client saying that their write was successful, yet when the backup takes over, the client's data will be missing.
    * The client will be able to detect the missing data, and will go away deeply saddened by all the trust issues this has created...

***Q:***&nbsp;&nbsp; So why doesn't the primary just wait for the partition to heal?
***A:***&nbsp;&nbsp; Because this might take an arbitrarily large amount of time, or never happen.

The downside here is that network partitions are a fact of life, so this forces us to choose between what we hope will be the lesser of two evils:

* Should we wait for the partition to heal and risk waiting an arbitrarily long period of time?
* Should we update the primary and send an acknowledgement back to the client, but risk data loss if the primary crashes whilst the network partition exists?

It looks like we're caught between a rock and a hard place here.  Typically though, any system that implements strong consistency will prioritise consistency over availability.  In other words, to have the client experience a large response time is better than having to say to that client *"Sorry, we lost your data"*.

So, this means that the acknowledgement seen in the diagram above would never be sent unless the network partition has first been healed and communication with the backups restored.

If we now adjust our definition of availability to mean that every client receives a request *within some fixed amount of time*, even then we would be unable to make such a guarantee because we have no idea how long a network partition might take to heal.  There are however, some strategies for honouring a response time constraint.  We could:

* Inform the client that the update has been accepted, but no backup is available
* Inform that client that while the network partition exists, *"Updates are temporarily unavailable"*

Unfortunately, the last option here is somewhat vacuous because although we advertise that our system is highly available, what we really mean is that *"It's highly available, except when it isn't"*.  This is not really in the spirit of true high availability.

As we have already stated, any system that implements strong consistency will prioritise consistency over availability, which means that in the event of a hopefully short-lived network partition, the system will sit around and wait before responding to the client.  The highest priority here is to avoid data loss, and if required, this must be achieved at the expense of availability.

Amazon's Dynamo however prioritises things the other way around.  Dynamo prioritises availability at the expense of consistency.

The dilemma here is that you cannot guarantee both availability ***and*** consistency: the presence of failure in your system forces you to prioritise one over the other.  This is true regardless of the replication strategy you choose to use.

Consider a different situation now; here, a client can talk directly to two replicas, but a network partition has suddenly appeared between the two replicas.

The client sends an update to replica 1 changing the value of `x` from `4` to `5`.

![Consistency/Availability Trade-off 1](./img/L17%20Tradeoff%201.png)

Let's say that due to the sudden appearance of a network partition, the heartbeat between <code>R<sub>1</sub></code> and <code>R<sub>2</sub></code> fails, so <code>R<sub>2</sub></code> knows that it's lost contact with <code>R<sub>1</sub></code> and its data is now potentially out of sync.

![Consistency/Availability Trade-off 2](./img/L17%20Tradeoff%202.png)

<code>R<sub>2</sub></code> now receives a query for the value of `x`.  How should it respond?

## The Trade-off Between Availability and Consistency

<code>R<sub>2</sub></code> only has two, rather poor options:

1. Risk violating strong consistency by returning the potentially wrong answer of `x=4`, or
1. Risk violating availability by saying *“Hang on please, I need to phone a friend”* and hoping that the network partition heals very quickly

This problem is known as CAP: ***C***onsistency, ***A***vailability, ***P***artition Tolerance

You cannot achieve all three, so pick the two you need and then learn to deal with the problems created by the other one.

By now it should be no surprise to learn that this situation contains some subtleties that are often overlooked:

* The consistency being spoken of is specifically strong consistency
* The availability being spoken of is perfect availability

Even though you can't have all three of these qualities, it doesn't actually matter that much, because you can provide a system that has *"good enough"* availability.

For instance, Amazon does not claim that Dynamo offers *perfect* availability, only *high* availability and are prepared to offer a slightly weaker form of consistency.  Some other companies choose to balance these priorities slightly differently.

When designing a distributed system, you need to decide which of these qualities is of the greatest importance to you, and then build the system to provide you with the correct balance.  In Amazon's case as an online retailer, fast response times are of higher priority than the occasional lost item, so availability is prioritised over consistency.

So, systems are designed along a spectrum with availability at one end and consistency at the other.  Notice however, that partition tolerance is not shown on this spectrum.  This is because it is a nastier type of fault and is much harder to tolerate.

![Consistency/Availability Trade-off 3](./img/L17%20Tradeoff%203.png)

## Questions

***Q:***&nbsp;&nbsp; Where does MongoDB lie on this spectrum?
***A:***&nbsp;&nbsp; More over to the availability end

However, systems like Dynamo are configurable in terms of the degree to which availability is prioritised over consistency (Dynamo has a configurable feature called "Quorum consistency")

When it was first published in 2007, one of the things that made the Dynamo paper so influential was that it contradicted the prevailing opinion that strong consistency must be given the highest priority.  Up until then, the majority of the research effort had assumed that the priority was to improve strong consistency and Byzantine fault tolerance.  However, Amazon realised if you emphasise strong consistency, you are then also forced to minimise the occurrence of network partitions; but in practice, this turns out to be extremely difficult simply because networks fail &mdash; get over it!

So, basically Amazon said *"Chasing after super high degrees of strong consistency is fool's errand because this also forces us to try to prevent the inevitable (network partitions).  So, let’s just accept that we'll get better results in the long term if we prioritise availability"* (or words to that effect...)

As soon as a highly successful online retailer said *"Not only do we not care about Byzantine Fault tolerance, we don't even care about strong consistency"*, people began to sit up and take notice.  This shift of priority became very influential for systems that came later because up until then, many companies had been over-engineering their approach to achieve high degrees of strong consistency.

---

| Previous | Next
|---|---
| [Lecture 16](./Lecture%2016.md) | [Lecture 18](./Lecture%2018.md)

# Distributed Systems Lecture 18

## Lecture Given by [Lindsey Kuper](https://users.soe.ucsc.edu/~lkuper/) on May 11<sup>th</sup>, 2020 via [YouTube](https://www.youtube.com/watch?v=xakpenkbOr0)

| Previous | Next
|---|---
| [Lecture 17](./Lecture%2017.md) | [Lecture 19](./Lecture%2019.md)

## Review of the [Amazon Dynamo Paper](./papers/Dynamo.pdf)

Prior to the publication of this paper, the prevailing assumption was that, given the CAP properties of consistency, availability and partition tolerance, it was ***obvious*** that the highest priority should be given to consistency.

Amazon said no &mdash; we don't care about consistency; we care about availability.  The main focus of their paper was to describe both how availability can be successfully prioritised over consistency, and to offer an analysis of the consequences of such a reprioritization.

### Availability

We defined availability to be ***"All requests receive a meaningful response"***.  It would possibly be better to qualify this definition by adding that a response should be given within a certain period of time, but as we saw in the previous lecture, such time guarantees are very hard to deliver without compromising either availability or consistency.

The primary focus of the Dynamo system is to say that if someone wishes to add an item to their shopping cart, then go ahead.  This activity must be prioritised over potential data loss that might occur through some sort of failure.

### Network Partition

A network is said to be ***partitioned*** if machines on that network can no longer communicate with each other.  Such situations are temporary and unintentional.

### Eventual Consistency

This idea is not new, it’s been around since at least the 1990's, but it has experienced a resurgence since the publication of the Dynamo paper to such an extent, that many people think eventual consistency was invented at around this time.  It is common, but incorrect, for people to cite a [2008 article](./papers/Vogels.pdf) by Werner Vogels as the origin of this term.  If you need a citation, it is better to quote from older work by Doug Terry and explained in articles such as [this one](https://littlemindslargeclouds.wordpress.com/tag/eventual-consistency/).

Eventually consistency can be defined as ***"Replicas will eventually agree if clients stop sending updates"***

This consistency model is not however a safety property - it is a liveness property, because it cannot be violated in a finite execution.

For Dynamo however, it is not immediately clear what safety properties it offers.  We have said that for a system to offer strong consistency, then for nodes that deliver the same set of messages, their states will agree - even if those updates arrive in different orders.  This is clearly a safety property, and Amazon has given this a lower priority over the liveness property of availability.

### Vector Clocks

Dynamo uses vector clocks to logically timestamp events in an attempt to resolve conflicts.  But as we have seen, vector clocks cannot resolve anomalies created by processing causally independent events.  In such cases, Dynamo offers two different approaches to conflict resolution:

* For the vast majority of cases, if causally independent versions of the data are discovered, then all available versions are simply sent to the client to be sorted out using application-specific conflict resolution, or
* Much less frequently, it adopts a simple ***"last-write-wins"*** strategy

### Application-Specific Conflict Resolution

Since the client application has a far better idea of what actions the user is performing, this is the best context within which to handle conflict resolution.  In the case of the user's shopping cart, if it turns out that the server ends up with two or more causally unrelated versions, then all this data is simply passed to the client-side application for resolution.  In the case of shopping carts, the correct approach is for the client simply to create a new shopping cart from a union of the different cart versions.

But why take set union over set intersection?  To sell more products?  Well, maybe, but by taking the union, it guarantees never to miss an item, whereas the intersection of non-identical sets guarantees that at least one item will be dropped.  It is true that the decision to use set union might, occasionally, result in a deleted item popping up again, but in practice, that situation is rare.

Dynamo is designed in such a way that you can elect to implement your own, client-side conflict resolution mechanism, or you can simply delegate this to the server, in which case, the ***last-write-wins*** approach is used.

## Write Commutativity

Addition and multiplication are commutative operations because the order of the operands does not change the outcome of the operation.

<code>3 + 4 &equiv; 4 + 3</code>  and <code>3 * 4 &equiv; 4 * 3</code>

It something of an abuse of terminology to describe writes as *"commutative"* because this term describes the outcome of a binary operation on the basis of the order in which the operands are applied; however, in spite of this imprecise usage of terminology, in the case of adding items to a shopping cart, the order in which the writes happen is immaterial; so in that sense, we can consider writes to be a commutative operation.  This approach works because a shopping cart is simply a set in which there is no causal relationship between the members: the presence of a book in your shopping cart is unrelated to the presence of a pair of jeans.

This fact alone is enough to gives us strong convergence; however, the paper also talks about vector clocks.  Why are vector clocks needed when we've just established that there's no causal relationship between the items in a shopping cart?

They're needed because addition is not the only operation you can perform on the items in a shopping cart.  Causal anomalies can occur if deletions are not processed correctly.  So, if, by means of a vector clock, we can demonstrate that version `A` of a shopping cart is the causal antecedent of version `B`, then version `A` can be safely thrown away.  However, if no causal relationship can be established between say, versions `C` and `D`, then divergence has occurred (possibly due to concurrent writes) and both versions of the shopping cart must be sent to the client for resolution.

## Resolving Replica Disagreement

It’s one thing for a disagreement to exist between replicas, but ***recognising*** that such a disagreement exists is also a challenge.  By drawing a Lamport Diagram, we are taking a God's-eye view of the situation and from this perspective, disagreements are obvious.

![Total-Order Anomaly](./img/L12%20TO%20Anomaly.png)

However, without some additional strategy in place, neither replica can tell that a disagreement exists.

### Anti-Entropy Protocol

Dynamo handles conflicts in replicated state using an anti-entropy protocol.

What this means in practice is that once per second, every node picks another node at random, and those two nodes compare their state.  If they discover a difference, they then start exchanging more detailed state information until the differing key/value pair is located.

### Gossip Protocol

A gossip protocol is different from, but related to, an anti-entropy protocol.

In Dynamo, data is partitioned across a set of nodes organised in a ring.  At any time, a node may fail, or a new node might be added to that ring, so the gossip protocol is used to resolve the changing state of node membership in the ring.

Using the gossip protocol, each node shares its own membership information with the others, and additionally, each node needs to know who the other current ring members are and what role they play.

So, we have two related, but distinct forms of conflict resolution protocol at work here:

* The anti-entropy protocol resolves conflicts between the state of each node's keystore
    I.E. Questions related to *"What do you think the value of `x` is?"*

* The gossip protocol resolves conflicts related to membership
    I.E. Questions related to *"Who do you think is up and running?"*


One thing the Dynamo paper states is that Amazon used to maintain a global view of the state of each node in a Dynamo system; however, after a while, they discovered that this global view was not needed (probably because it created some sort of bottle-neck) and that a local view was sufficient.

Both of these protocols are examples of *eventually consistent* protocols that implement strong convergence in application state.

> ***ASIDE***
>
> In the context of the Dynamo Paper, the terms ***anti-entropy*** and ***gossip*** are used to describe two different mechanisms for resolving distinct, but related types of conflict.
>
> However, in other papers, you may find that these terms are used synonymously; with "anti-entropy" being used as a fancy term for "gossip"

### Are These Two Types of State Conflict So Different?

Conceptually, resolving a conflict in the shared state of a key/value store, and resolving a conflict of group membership are quite similar.  The key difference lies on how much data needs to be exchanged; firstly, to discover a difference, and secondly to resolve that difference.

In terms of discovering differences in group membership, only a small amount of data needs to be exchanged before a difference is discovered and then resolved.  However, in the case that a key/value store must be shared between multiple nodes, a potentially huge amount of data might need to be exchanged before a difference is discovered.

### Using Merkle Trees to Discover State Differences

In order to exchange state data efficiently, Dynamo minimises the amount of network traffic by using Merkle (or Hash) Trees.  A Merkle Tree is a (typically binary) tree in which the value of each parent node is the hash of the values of its children.  Thus, two nodes can discover a difference in the state of their entire key/value stores simply by comparing the hash value of the root nodes of their Merkle Trees.  If these values differ, then somewhere further down the tree, a difference must exist.  Only then do the nodes start exchanging lower level hash values until the different key/value pair is discovered.

This solves the "*cost of data transfer*" problem.

![Merkle Tree 1](./img/L18%20Merkle%20Tree%201.png)

The above diagram represents the Merkle Tree that would be created for a keystore containing four values.  In order for two nodes to discover if their keystores are identical, all they need to do is compare the hash value `H7` of their root nodes.  If these are identical, then everything else beneath that point in the tree must also be identical.

If two data stores do differ in only one item, then the difference can be discovered by traversing the Merkle Tree until the differing leaf node value is discovered.

![Merkle Conflict 1](./img/L18%20Merkle%20Conflict%201.png)

Here, we can see that the value of `B` differs between replicas 1 and 2.  Consequently, the value of all the parent nodes above `B` will differ.  So, when replicas 1 and 2 compare root node has values, they will discover that these values differ (the difference here is illustrated using colour rather than any numerical value):

![Merkle Conflict 2](./img/L18%20Merkle%20Conflict%202.png)

The root nodes are compared and found to be different, so the child node values are compared

![Merkle Conflict 3](./img/L18%20Merkle%20Conflict%203.png)

The `H6` node in each tree is the same, so the difference cannot lie beneath this node and this side of the tree can be entirely ignored.  However, the `H5` node values differ, so the difference must lie somewhere beneath this node.

![Merkle Conflict 4](./img/L18%20Merkle%20Conflict%204.png)

The children of `H5` are compared, and the difference is found to be with node `H2`.

![Merkle Conflict 4](./img/L18%20Merkle%20Conflict%204.png)

The child of `H2` turns out to be a leaf node.

![Merkle Conflict 5](./img/L18%20Merkle%20Conflict%205.png)

So, this is where the differing key/value pair is located and we have established that replica one thinks `B=2`, but replica 2 thinks `B=9`

So, the Merkle Tree comparison strategy effectively *"binary chops"* its way through the data in the keystore to locate the differing value(s).

We should also note that the values stored in the keystore are not necessarily simple integers as shown here; they are usually entire data objects. So, this strategy identifies the exact differing value, and agreement can be reached by transferring only that value over the network.

If multiple key values differ, then these can also be discovered using the same strategy.  In the worst case, you would need to compare all the values in the keystore; but this is a highly unlikely situation.  In reality, the differences between large keystores are small, thus making this an efficient difference detection strategy - especially when these differences need to be discovered over a network.

Merkle Trees are used in a wide variety of situations, not only for comparing keystore values.  They are often used in the case of authentication.  In the case of Dynamo however, they explicitly state that this strategy is employed within a trusted, non-threatening environment.  So, under these conditions, the primary consideration here is to save on network bandwidth.  Attacks from hostile third parties are explicitly excluded from this discussion; therefore, there is no need for Dynamo to have any concept of user or request authentication.  However, Merkle Trees are useful in both situations.

### Resolving State Differences

This is a very different question from detecting that replicas disagree with each other.  The use of Merkle Trees is confined simply to making difference detection as efficient as possible.  Once a difference has been discovered however, we must now engage in a very different type of conflict resolution, and this is application specific.

Once the Merkle Tree has been used to identify differing key/value pairs, the difference can be resolved at the keystore level simply by storing both versions of the object, so in the example we used above, the resolved state of the keystore would be:

![Merkle Tree 2](./img/L18%20Merkle%20Tree%202.png)

Now, when a client wants to read the value of `B`, it would receive `{2,9}` instead of a single value.  Given that the client application understands the meaning of the data far better than the keystore does, it is typically the client's responsibility to decide which version of the object is correct, and it might do this on the basis of something like a timestamp or a vector clock carried in the object's metadata.


One question that often comes up here is *"What if the two replicas hold completely different key/value pairs?"*.

In the case of the Dynamo paper, this problem does not really become an issue because when a ring of nodes is started, each node is informed about the key range that it will be responsible for.  Therefore, significant structural differences between replica keystores are minimal.

However, more generally, the Merkle Tree does not need to be specifically a binary tree.  It could be a combination of Merkle Tree and a Prefix Tree (known as a *Merklix Tree*).

Alternatively, you could build a Merkle Tree with a branching factor higher than two.


## Quorum Consistency

In the remaining time in this lecture, we will only have time to touch this topic briefly.

In Primary Backup replication and Chain Replication, the clients are restricted to talking only to specific nodes:

* In Primary Backup Replication, the client always talks to the primary node for both reads and writes
* In Chain Replication, the client talks to the head node for reads and the tail node for writes

However, in Dynamo the clients can talk to ***any*** node.  In fact, the clients typically hold a node table that is updated every 10 seconds, and based on this information, the client calculates which node to talk to, based on who gave the fastest response to their previous operation.

The question now becomes this: *"How many replicas should I talk to before getting an answer I can consider reliable?"*

In a quorum consistency environment, there are three specific, configurable values that control how this question should be answered.

* `N` - The number of replicas (typically 3)
* `W` - **The Write Quorum**
    The number of replicas that must respond to a write operation in order to consider that operation a success (typically 2)
* `R` - **The Read Quorum**
    The number of replicas that must respond to a read operation (typically 2)

> ***ASIDE***
>
> There is a detail concerning the definition of the read quorum value that needs to be mentioned.
>
> Opinions differ as to whether the read quorum specifies simply the number of responding replicas, or the number of agreeing replicas.
>
> In this course, we will only concern ourselves with the simple case that the read quorum refers to the number of responding replicas, and not worry about whether those replicas all respond with the same value.


If we suppose the following configuration:

```
N = 3
W = 3
R = 1
```

This configuration implements a system that prioritises read performance because:

1. We require all three replicas to acknowledge the success of a write (thus providing strong consistency), and
1. Knowing that all the replicas contain the same data, we can be sure that a read from ***any*** replica will be authoritative

This is a popular Dynamo configuration setting, often known as Read One, Write All (or ROWA) and it does provide reliable writes and fast reads, but consider this:

***Q:***&nbsp;&nbsp; Is it fault tolerant?
***A:***&nbsp;&nbsp; No, it’s not because if one of the nodes crashes, or a network partition suddenly separates the client from one of the replicas, then it can no longer perform any writes - because we have stipulated that all three nodes must respond to a write operation before we can consider it successful.

So, whilst this `331` configuration this gives certain advantages, it does so at the risk of reduced fault tolerance.

---

| Previous | Next
|---|---
| [Lecture 17](./Lecture%2017.md) | [Lecture 19](./Lecture%2019.md)

# Distributed Systems Lecture 19

## Lecture Given by [Lindsey Kuper](https://users.soe.ucsc.edu/~lkuper/) on May 13<sup>th</sup>, 2020 via [YouTube](https://www.youtube.com/watch?v=2edhMsGlwng)

| Previous | Next
|---|---
| [Lecture 18](./Lecture%2018.md) | [Lecture 20](./Lecture%2020.md)

## Continuation of Quorum Consistency

We finished the last lecture with this overview of quorum consistency.

In a quorum consistency environment, there are three specific, configurable values that control how a system can be configured.

* `N` - The number of node replicas
* `W` - **The Write Quorum**
    The number of replicas that must respond to a write operation in order to consider that operation a success
* `R` - **The Read Quorum**
    The number of replicas that must respond to a read operation

Depending on what balance our system needs to have between availability and consistency, we need to tune the `NWR` values accordingly.

For instance, if we want strong consistency, then we could use `N=3, W=3, R=1`.  This means that a write operation is only considered successful if it has been acknowledged by all three nodes.  A direct consequence of setting `W=N` is that we now know for certain that all the nodes will agree with each other; therefore, if we set `R=1`, we can be 100% confident that it won’t matter which node answers a read request, because they all ***already*** agree.

Whilst this is a popular configuration setting, the trouble is that if any of the write nodes crash, or a network partition suddenly appears, you're unable to perform any further writes.

Instead of using `N=3, W=3, R=1`, the Dynamo paper recommends `N=3, W=2, R=2`

This now creates the possibility of a read conflict.

![Dynamo Read Conflict 1](./img/L19%20Dynamo%20Read%20Conflict%201.png)

A client changes the new value of `x` from `4` to `5` by writing to replicas `R1` and `R2`.

If the client then immediately reads the value of `x`, it is possible that before all the nodes have synchronized their values, this read operation might be handled by replicas `R2` and `R3`.

![Dynamo Read Conflict 2](./img/L19%20Dynamo%20Read%20Conflict%202.png)

This will result in the client receiving different values of `x`.

At this point, it is important to understand that there is a discrepancy between different system implementations about what exactly the read quorum value `R` means in practice.  Does is refer to:

* The number of nodes that must respond to a read request, or
* The number of nodes that must respond to a read request *with the same value*?

In the context of the Dynamo paper where Amazon prioritise availability over consistency, it seems clear that the read quorum value `R` is used to refer simply to the number of nodes that must respond to a read request.  If they return conflicting values, then so be it.

In general, though, if we ensure that `R + W > N`, then we can be certain that every write quorum intersects with every read quorum, thus ensuring that we avoid what's known as a *"stale read"*.  A stale read is where ***all*** of the responses are out of date.  The `R + W > N` approach ensures that a read will always return at least one correct response.

For instance, if we set the write quorum to `2` and the read quorum to `1`, then it’s possible that we could be writing to replicas `R1` and `R2` and reading from replica `R3`.  Thus, until the nodes synchronise their state, read operations could return stale values.

A further caveat is to understand that simply satisfying the inequality `R + W > N` only helps prevent stale reads, it does not ensure fault tolerance because as we saw in the first example, setting `N=3, W=3, R=1` guarantees strong consistency, but does so at the expense of fault tolerance.

The Dynamo paper quotes the configuration settings as `N=3, W=2, R=2` because this ensures that ***someone*** will respond to a read operation with the correct value.  In Amazon's situation, if a read request returns a set of conflicting values, then typically, the client application must resolve the conflict.

***Q:***&nbsp;&nbsp; What's wrong with the "Read One, Write All" approach?
***A:***&nbsp;&nbsp; Several reasons.  Firstly, ensuring strong consistency is slow.  Since we have to wait for all the nodes to acknowledge a write operation, the write response time cannot be any faster than the slowest node.  Also, this configuration is not fault tolerant.  If a node crashes or a network partition suddenly appears, then immediately, we have lost the ability to performs writes.

## Sharding or Data Partitioning

Here's one of those annoying situations in distributed systems where the same term is used to mean two, totally different things.  The word *"partitioning"* here is used to mean the way you split up your data between different nodes (which is a good thing), as opposed a sudden loss of communication caused by a network partition (which is a bad thing).

In the systems we've spoken of so far, all the machines store all the data.  So, each machine has a full copy of your entire keystore.

![No Sharding](./img/L19%20No%20Sharding.png)

But this approach has several drawbacks:

* ***Scalability***
    If you're running primary backup replication, then under heavy load conditions, all the work falls on the primary which soon becomes a bottleneck
* ***Quantity***
    Maybe you have more data than will fit on a single machine
* ***Synchronisation***
    Each copy must synchronise with all the others every time there is a write

But how about an approach like this?

![Sharding 1](./img/L19%20Sharding%201.png)

So now, we don't have the problem of stale reads because each machine only handles a known subset of the data.  The trade-off here is that in this example, we have now lost fault tolerance because there is no replication; but it could be reinstated quite easily.

![Sharding 2](./img/L19%20Sharding%202.png)

This technique is known as ***Sharding*** or ***Data Partitioning***.

Each fragment of data stored on a replicated node is known as a ***shard*** or a ***replica group***.

![Sharding 3](./img/L19%20Sharding%203.png)

There are multiple reasons for why you might want to adopt this approach.  These include:

* If the range of client requests is more or less evenly distributed across the full range of keys in your keystore, then this will improve throughput
* Or, you might simply have too much data to fit on one machine, in which case, sharding is the only viable option

The design shown above is somewhat simplistic in that we have a single key/value pair stored per shard.  In reality however, shards will typically store broad ranges of key/value pairs.  But even taking this into account, the arrangement shown above still does not represent the way Dynamo implements sharding.

Here's another arrangement that combines these various approaches into one:

![Sharding 4](./img/L19%20Sharding%204.png)

Each node now holds an overlapping range of key/value pairs.  `x` can be found on `M1` and `M2`, `y` can be found on `M1` and `M3`, and `z` can be found on `M2` and `M3`.  So, it looks like we have the best of both worlds here: we have replication across nodes ***and*** sharding.

In fact, what we have done is implement a distributed version of Primary Backup Replication.  In the previous examples of PB Replication, we had a single node acting as the primary for all the data, and then all of that data was replicated across all the backup nodes.  Consequently, the primary had to handle all the reads and writes and could become the bottleneck under high load situations.

By sharding the data, we have said that one node can act as the primary - not for all the data, but just a subset of that data.  So now the roles of primary and backup have been distributed across multiple nodes.

![Sharding 5](./img/L19%20Sharding%205.png)

So, each node plays the role of primary for some values and backup for others.

| Key | Primary | Backup
|---|---|---
| `x` | `M1` | `M2`
| `y` | `M3` | `M1`
| `z` | `M2` | `M3`

Given this division of labour, when the client wants the value of `x`, it will talk to the node acting as the primary for `x` - which in the case, happens to be `M1`.  Similarly, a client wanting the value of `z` will know that it can talk directly to `M2`.

Not only have we split up the workload of serving read/write requests, but each machine now only needs to store two thirds of the entire dataset.

The only remaining detail to consider is that each primary must replicate all write requests to their respective backup node(s).

![Sharding 6](./img/L19%20Sharding%206.png)

No matter how the sharding is implemented, we have two forms of replication at work here:

![Key Replication](./img/L19%20Key%20Replication.png)

![Dataset Replication](./img/L19%20Dataset%20Replication.png)


The choice for how you replicate data and how it is sharded are somewhat orthogonal.  In the rest of this discussion, we will focus only on sharding techniques and assume that replication will be implemented somehow.

## Partition Strategies

How do you decide which key/value pairs go where?  To answer this question, we must first establish what goals our partitioning strategy needs to meet.  We really need to achieve two goals here:

* ***Goal 1***&nbsp;&nbsp; Avoid any read or write hotspots
* ***Goal 2***&nbsp;&nbsp; Make the data easy for clients to find quickly

| Strategy | Goal 1 | Goal 2
|---|---|---
| Random distribution of data across all the nodes | ![Tick](./img/tick.png) | ![Sad face](./img/emoji_sad.png)<br>The clients now have no idea where the data lives...
| Put all the data on one node | ![Sad face](./img/emoji_sad.png)<br>Under high load conditions, this will create a performance bottleneck | ![Tick](./img/tick.png)

So, neither of these are good ideas.

### Partitioning Data by Key Range

If we know that the key values in our dataset fall into some range, then we can distribute that data by allocating each node a range of key values.

So, if you're handling data that is sorted alphabetically, then you could distribute the data across three machines such that keys starting with a particular letter will be handled by a known machine.

| Alphabetic Range | Machine
|---|---
| `a-h` | `M1`
| `i-r` | `M2`
| `s-z` | `M3`

But there's a big problem here: unless the data is uniformly distributed across the key range, then you will still have hotspots.

How do we take data that has a non-uniform distribution within its key range, and map it some other domain such that the mapping process yields the uniform distribution we're looking for?

Hashing!

### Partitioning Data by Hash Function

A good hashing function such as MD5 will distribute its input space evenly across its output space.

The MD5 algorithm returns a number in the range `0` to <code>2<sup>128</sup> - 1</code>.  For instance:

![MD5 Output Space](./img/L19%20MD5%20Output%20Space.png)

What we need to do now is make sure that each node looks after an evenly sized chunk of the hash function's output space.  However, an easier way to calculate this is to say that since we wish to distribute the hash values across 3 machines, then we can simply calculate `modulus 3` of the hash value to give a server number of `0`, `1` or `2`.

So, we can extend this diagram to help us identify the target node:

![MD5 Has to Node Number](./img/L19%20MD5%20To%20Node.png)

This is the *"Hash mod `N`"* approach and as good as it is, this naïve implementation has a significant drawback.

The problem is that if `N` changes, then this completely alters which machine should hold which key value: and this is true not only for new keys, but also for all the existing keys.

For instance, if we added a new machine `M4`, then this could result in having to move our `"aardvark"` from `M1` to `M0` &mdash; and this would upset him because he's just settled into his new home and now you want to move him again (you know how touchy Aardvarks can be&hellip;)

It is certainly true that when a new machine is added, some of the existing data will need to be redistributed, but it does not makes sense to move existing data from one old node to another old node.  In an ideal situation, the addition of a new node should cause only the smallest amount of data to be redistributed, and certainly not cause data to be moved between existing nodes.

So, what is the minimum amount of data that should be redistributed after the addition of a new node?

Let's say we have 6 keys distributed over 3 nodes.  This then averages out to 2 keys per node.

![Node Addition 1](./img/L19%20Node%20Addition%201.png)

Now, due say to a spike in request volume, we need to add a new node `M4`.  If we still wish to maintain an even distribution of keys per node, then we need to rearrange the existing data to include this new node.  But how many keys should we move and which ones?

In general, if we have `K` keys distributed across `N` nodes, then on average, each node will store `K/N` keys.  Previously `K=3` and `N=6`, so no prizes for figuring out that each node should hold 2 keys.  However, if `K` now increases to 4, then `K/N` becomes `1.5`.  Since we can't move half a key, we'll round this value down.  So, in general we can say that each node will hold `floor(K/N)` keys.

![Node Addition 2](./img/L19%20Node%20Addition%202.png)

The addition of the new node has caused a single key to be transferred to  `M4`.  In this case, we chose to move `"zzzzz"` because the Aardvark likes living in `M3`, and we didn't want to upset him.

Notice that data is only transferred from an old node to the new node; no data is ever transferred between the old nodes.

### Consistent Hashing

This is yet another case in which a word we've previously used to mean one thing ("*consistent*") is now being used to mean something different - but the use of the word "consistent" in this context has its origins in network design, not distributed systems.

The first change we need to make is to arrange our nodes in a ring.  The position of a node around the ring is calculated by hashing some value unique to each node - say a combination of the node name and its IP address.

The MD5 hash function has a vast output space ranging from `0` all the way up to <code>2<sup>128</sup> - 1</code>.  This is such a huge range of values that we cannot represent it graphically in any meaningful way, so for the purposes of the following diagrams, let's pretend the hash function's output space occupies only the range `0` to `63`.

![Dynamo Node Ring 1](./img/L19%20Ring%201.png)

So, in this scenario, our reduced-output-space hash function has positioned our four nodes roughly evenly around the ring at the following locations:

* `M1` is at location `08`
* `M2` is at location `20`
* `M3` is at location `32`
* `M4` is at location `47`

Let's now say we want to add the new key `"apple"`.  When put through the hash function, this key yields the value `14`.

![Dynamo Node Ring 2](./img/L19%20Ring%202.png)

There is no node sitting exactly at location `14` on the ring, so we scan clockwise around the ring looking for the next available node, which in this case, turns out to be `M2`.

The rule here is that keys belong to their clockwise successor on the ring.

Now let's say our old friend the Aardvark wants to move in.  In our particular scheme, `"aardvark"` hashes to `62`, so we repeat the same process as before:

![Dynamo Node Ring 3](./img/L19%20Ring%203.png)

There is no node at location `62`, so we continue clockwise around the ring, passing go, collecting $200 and encountering `M1`.  So, `"aardvark"` will be stored in node `M1`.

### Key Replication

Dynamo also uses this scheme to decide where a key should be replicated.

If we assume that the ring's replication factor is 3, then this means every key must be stored on a total of 3 nodes &mdash; but how do we decide which three nodes?  The approach here is the following:

* Every key has a *"home"* node.  This is the node the key is stored on using the *scan clockwise* approach described above.
* Once the key is stored on the home node, it is then forwarded to the next clockwise node around the ring and stored there too.
* The key continues to be forwarded clockwise around the ring until it has been stored in the correct number of replicas.

So, in the example where we stored `"apple"` on `M2`, the replication factor of 3 requires that this key is also replicated on nodes `M3` and `M4`

![Dynamo Node Ring 4](./img/L19%20Ring%204.png)

The Dynamo Paper refers to this list of nodes as the *"preference list"*, and it usually includes more nodes than the replication factor requires because some nodes could be down or unavailable.  So, in Dynamo, you keep working your way down the preference list using the next available node until the ring's replication factor has been satisfied.

### Adding a New Node

We started this discussion in order to understand how we could move as little data as possible when a new node is added to the ring.

As it currently stands, whenever a new key is added to our ring, it will land on the home node calculated from the following hash function ranges:

| Hash Function Range | Home Node |
|---|---|
| `09` to `20` | `M2`
| `21` to `32` | `M3`
| `33` to `47` | `M4`
| `48` to `08` | `M1`

Ok, but now let's add a new node `M5` at position `60`.

* How does this change things?
* How much data will we need to move?

| Hash Function Range | Home Node |
|---|---|
| `09` to `20` | `M2`
| `21` to `32` | `M3`
| `33` to `47` | `M4`
| `48` to `60` | `M5` &lt;&mdash; New node
| `61` to `08` | `M1`

So, effectively, we have taken `M1`'s hash function range and split it in half. The range of keys with hash values between `48` and `08` would previously all have landed on `M1`, but now `M5` has arrived at location `60` and taken over the lower part of the range from `48` to `60`.  Therefore, the only keys that need to be moved are the keys currently stored in `M1` whose hash function values fall in the range `48` to `60`.

Nothing else needs to change.

![Node Addition 3](./img/L19%20Node%20Addition%203.png)

None of the other nodes are affected.  In fact, these other nodes do not even need to know that a new node at some other, distant part of the ring has been added.

### What Happens if a Node Crashes?

In our diagram, let's look at the consequences of node `M2` crashing.  First, let's assess what we already know:

* `M2` is responsible for keys having hash values in the range `09` to `20`
* `M3` is responsible for keys having hash values in the range `21` to `32`
* `M3` is the successor of `M2` and our ring uses a replication factor of 3; therefore, all the keys that use `M2` as their home node have ***already*** been replicated in both `M3` and `M4`

![Node Crash 1](./img/L19%20Node%20Crash%201.png)

All that happens is that `M3` simply extends its hash value range to include `M2`'s range.  In this case, `M3`'s hash value range now extends from `09` to `32`.

All of `M2`'s keys backed up in `M3` are now promoted from backup to primary copies, and any new key values in the range `09` to `32` are written directly to `M3`.

At this point in time, the administrator will probably want to bring up a new node to replace `M2`, but until they do, `M3` takes up the slack.

### Can Consistent Hashing Go Wrong?

Yes.  If your input values fall into a narrow range, then there will not be a particularly good distribution of nodes around the ring, which in turn, could cause a node to become overloaded and potentially crash.

One trick that Amazon use in Dynamo is the idea of virtual nodes.  This is where, instead of mapping a node to a single hash value on the ring, it is mapped to a set of values.  This means that one physical node could be mapped to 10, or 20 or even 50 different hash value locations around the ring.  Using this trick, you are much more likely to achieve an even node distribution around the ring.

In addition to improving the distribution of nodes around the ring, you could have a different number of virtual nodes per physical node to account for differing storage capacities of the physical hardware running each node.

For instance, if the hardware on which one node is running has a 1Tb hard drive, then for instance, you might allocate 20 virtual nodes to this one physical node.  However, if another node in the same ring is running on a machine with a 2Tb hard drive, you might choose to allocate 40 virtual nodes knowing that due to its increased storage capacity, this machine can handle a bigger hash value range.

Unfortunately, the use of virtual nodes has a couple of downsides.

Firstly, if lots of virtual nodes are assigned to a physical node and that physical node goes down, then this has a large impact on the rest of the ring because it appears that suddenly, lots of "nodes" have disappeared.  Now lots of other nodes will need to take over the gaps that have appeared in the hash value ranges.  The Dynamo paper, however, declares this to be a feature because if a physical node running multiple virtual nodes goes down, then the workload becomes spread out around the ring, rather than being taken on a single successor.  Although this point does tend to make sense, it is somewhat harder to reason about objectively.

Secondly, replication of virtual nodes is more complicated because you should not replicate data between two virtual nodes if those nodes are running on the same physical machine, because then you haven't achieved true fault tolerance &mdash; the data still lives on the same hardware!



## Finally, A Word from Our Sponsor

In preparation for the next lecture, please read Google's [MapReduce](./papers/MapReduce.pdf) paper, and remember &mdash; be nice to Aardvarks...

![Baby Aardvark](./img/aardvark.jpeg)


---

| Previous | Next
|---|---
| [Lecture 18](./Lecture%2018.md) | [Lecture 20](./Lecture%2020.md)

# Distributed Systems Lecture 20

## Lecture Given by [Lindsey Kuper](https://users.soe.ucsc.edu/~lkuper/) on May 18<sup>th</sup>, 2020 via [YouTube](https://www.youtube.com/watch?v=8MOpJ4LoRpc)

| Previous | Next
|---|---
| [Lecture 19](./Lecture%2019.md) | [Lecture 21](./Lecture%2021.md)


## How is Google's [MapReduce Paper](./papers/MapReduce.pdf) Related to Distributed Systems?

### Online Systems

Up until now, we have focused on the design of systems to which you make requests, and from which you receive responses.  Key/value stores such as Amazon's Dynamo work this way; Web servers also work this way, as do databases and proxy caches.

In the case of Web Servers, you should not think only in terms of general-purpose HTTP servers such as Apache or Nginx, but also in terms of apps that have a built-in, dedicated HTTP server as the primary means for interaction.

All of these systems can be lumped together into the category of "Services" or "Online Systems".  Such systems are passive in the sense that they all wait for an incoming client request, and then try to handle it as quickly as possible (given the constraints of whatever consistency model they're implementing).  These systems typically prioritise:

* Low latency
* High availability

Under these circumstances, response times are typically in the range of a few tens to a few hundreds of milliseconds.


### Offline (Batch Processing) Systems

However, there are other types of system that take in huge amounts of data in order to analyse it in some way.  Typical examples of such analysis include restructuring user data to make it more useful to a specific user group, or to derive some form of summary.

The goal here is not to achieve low latency, but high throughput - the faster you can crunch your way through one terabyte of data, the better.  Consequently, the time taken to perform this type of distributed analysis is often significant - of the order of hundreds or even thousands of seconds.

So, the goal of an offline system is to achieve a very high degree of parallelism, as opposed to the high degree of concurrency needed by an online system.

> ***ASIDE***
> The concepts of parallelism and concurrency are often confused.  They are distinct, but related concepts that are often implemented together within the same system.
>
> * ***Concurrency***
>     Provides a high degree of scalability and fault tolerance by allowing multiple (typically small) tasks to be handled simultaneously
> * ***Parallelism***
>     Provides raw speed by allowing a single (typically very large) task to be broken down into a large number of small, independent subtasks that can all be executed simultaneously.

Google's MapReduce system and its successors are examples of offline systems that solve problems by means of high degrees of parallelism.

It should also be noted that Google published their MapReduce paper in 2004 and since then, this technology has been superseded by more generic tools.  As of 2014, Google stopped using MapReduce as their data analytics tool in favour of [Cloud Dataflow](https://www.datacenterknowledge.com/archives/2014/06/25/google-dumps-mapreduce-favor-new-hyper-scale-analytics-system/)

## Your Sharding Strategy Depends on Your Access Strategy

Up until now, we have only looked at data that is stored as simple key/value pairs and then accessed by key lookup.  However, as soon as you change either your data model or your access strategy, then the question of how your data should be sharded becomes a lot more subtle.

So, instead of having a simple key/value store, what if you had a relational database with a detailed schema?  Now, the way you shard your data would be based on the type of queries you expect.

For example, if you are Facebook end-user, then you access your data in one way, but if you are a Facebook data scientist analysing social graphs, then you need to access the same data, but in a very different way.  Here is a situation in which two user groups have very different perspectives on the same data, thus they require very different patterns of access.

As far as performance is concerned, FaceBook's priority is to ensure that their end-users experience the fastest possible response time.  But the priority of minimum end-user response time does not help the FaceBook data scientists trying to analyse how the website is being accessed, or how social graphs develop and change over time.  Therefore, in order for the both the end-users to enjoy a fast response time, and for the data scientists to be able to do their job efficiently, multiple copies of the data are needed.  You could argue that having multiple copies of the data is redundant, but the different structures used by the different datastores make a huge difference to the time taken for the different user groups to perform their work.

Google's MapReduce paper gives these two types of data different names:

* ***Raw data***
    The authoritative version of the data, usually stored according to the structure in which it was originally obtained (or created)
* ***Derived data***
    One of more copies of the raw data that have been processed and restructured in some way (for instance, some metrics have been applied in order to derive some type of summary).
    Derived data can also be created from other sets of derived data.

Google's MapReduce is a tool for transforming raw data into derived data.

## Example: Building an Inverted Index

In order to make the Web searchable, you need an index that allows people to search for a Web page on the basis of the words that page contains.  But the Web is not organised by keywords, it is organised first into websites, then each website contains multiple pages (or documents).

Google tackles this problem first by using crawlers that go out and gulp down entire websites.  Then, all these documents are stored *as-is* in what is known as a ***forward index***.

| Document | Contains the Words
|---|---
| Doc 1 | the, quick, brown, fox...
| Doc 2 | the, dog, growls, at, the, fox...

Here, the data is organised by document.  If you know the name of the document, you can discover all the words within that document.  But this is not how people search the web: people know what words they're searching for, but don't know which documents contain those words.  In other words, we need to create the style of index that is found at the back of a book, where you look up a word in order to discover the pages where that word is used.

There's nothing wrong with storing the data in the form of a forward index, it’s just that in order to be useful to people wanting to search the Web, this cannot be the ***only*** structure used to store the data.

If we restructure this data, we can produce an alphabetically sorted list of words from which we can then discover the documents containing those words.

| Word | Contained in Documents
|---|---
| at | Doc 2
| brown | Doc 1
| dog | Doc 2
| fox | Doc 1, Doc 2
| growls | Doc 2
| quick | Doc 1
| the | Doc 1, Doc 2

Compared to the forward index, we have not changed the amount of information in the inverted index.  It’s exactly the same information, only it’s been rearranged in such a way that makes a different sort of lookup very easy.

So, what type of processing is needed to transform a forward index into an inverted index?

To answer this question, we don't actually need to know anything about distributed systems.  This is a simple algorithmic question that can be answered by breaking the problem down into a couple of steps:

1. For every document in the forward index:
    * Scan that document and for every word encountered
    * Emit an intermediate key/value pair containing the word and the name of the document
1. Sort all the word/document pairs by word, collating the document names in which that word occurs

![Transform a Forward Index into an Inverted Index](./img/L20%20Inverted%20Index.png)

Now we have inverted the index and made documents discoverable on the basis of the words they contain (whereas previously, the words were only discoverable if you knew the document in which they lived)

Conceptually, this is not a complicated process&hellip;

***Q:***&nbsp;&nbsp; So why are we even talking about this in a distributed systems class?
***A:***&nbsp;&nbsp; Because when you want to perform this task on a huge dataset in as short a time as possible, it becomes a distributed systems problem

Now, in order to solve this problem on a massive scale, we need to bring in everything we've learnt about scalability, consistency and fault tolerance.

## MapReduce Functionality from the Inside

The basic observation made by Google was that although the transformations that need to be performed on the data are, in themselves, quite straight forward, that simplicity is obscured by the complexity of having to perform this task in a highly distributed, scalable and fault tolerant manner.  Therefore, wouldn't it be good if there were an easy-to-use framework that hid all the distributed systems complexity and simply allowed developers to represent their problem in a generalised manner?

This is what MapReduce was built to provide.

Due to the enormous size of the datasets involved here, there is no way that either the forward or the inverted index would ever be able to fit on a single machine, so immediately, we have to make some very important data sharding decisions.

Using the example of inverting a list of Web pages into a word index, the fact that the data making up the forward index is already split up across a large number of machines is not a problem.  Each machine can still contribute towards the overall solution by creating a set of intermediate key/value pairs from whatever subset of documents it has in its possession.  Since each document is processed in exactly the same way, it doesn't in fact matter whether an individual machine possess a large or small number of documents.  Also, since there are no dependencies between documents, the order in which they are processed is not important.

Here is an example of how a very large task can be split into a large number of independent subtasks, and then each of those subtasks executed simultaneously.  Some tasks are very hard to parallelize, but this is not one of them; in fact, this type of parallelism is known as ***embarrassingly parallel***.   In other words, it is so easy to split up the task into parallel subtasks, that it would be embarrassing not to.

For the sake of simplicity, let's imagine that every document in the forward index is allocated to a single machine, and that each machine builds its own set of intermediate key/value pairs:

![Distributed MapReduce 1](./img/L20%20Distributed%20MapReduce%201.png)

It's important to point out that so far, no network communication has been required.  All the intermediate key/value pairs are written to each machine's local hard disk.  This is what allows all the `M` machines to work independently of each other.

Well that's nice, but so far, we're only halfway to a solution.  These intermediate key/value pairs now need to be collated to form the forward index.

Let's now say that we have two machines for the second phase of the computation (<code>R<sub>1</sub></code> and <code>R<sub>2</sub></code>).  So how would we decide which machine should handle which key?

We've answered this question before when we looked at consistent hashing.  If we take the hash value of the key in the intermediate key/value pair and `mod` it by the number of available `R` machines, then we can guarantee that the same words will always be collated by the same machine.

![Distributed MapReduce 2](./img/L20%20Distributed%20MapReduce%202.png)

Several questions remain however:

1. Didn't we say in the last lecture that using `hash mod N` is not a good strategy because if `N` changes, then you have rearrange all your data around?
1. How did the data get from machines <code>M<sub>1</sub></code>, <code>M<sub>2</sub></code> and <code>M<sub>3</sub></code> over to <code>R<sub>1</sub></code> and <code>R<sub>2</sub></code>?
1. What happens to the output of the `R` machines - where does that go?

### Doesn't `hash mod N` Introduce Problems if `N` Changes?

In the case of Amazon Dynamo, a naïve implementation of `hash mod N` will certainly lead to problems if `N` changes.  This is because you are working in an online environment in which it is very difficult (impossible?) to predict the expected data volume; therefore, you must be able to scale rapidly (I.E. add new nodes, thus changing `N`) in order to handle spikes in request volume.  Contrast this however with Google's MapReduce environment and you find you're working in an offline situation where you already know exactly how much data your current batch will be processing.  Therefore, since you know you're working is a stable environment, you can scale the number of `M` and `R` machines accordingly.

There is, of course, the possibility that a machine could fail.  So, MapReduce uses a check-pointing strategy that allows for a new machine to take over the computation from the failed machine's last check point.  That way, only a minimal amount of reworking is needed in order to continue with forward progress.

### How is the Data Moved Between the Machines?

The transfer of data from the `M` machines to the `R` machines is known as the "shuffle".  This is quite a time-consuming phase because all the data accumulated on each of the `M` machines needs to be transferred over the network to the respective `R` machines &mdash; and as Google point out in their paper, network bandwidth is a rare commodity.

![Distributed MapReduce 3](./img/L20%20Distributed%20MapReduce%203.png)

### What Happens to the Output of the `R` Machines?

Once the various `R` machines have collated their portion of the data, the MapReduce framework handles writing that data to Google's distributed file system GFS.

> ***ASIDE***
> Google no longer use the GFS distributed file system, but since the paper makes reference to it, it is included here.

### MapReduce as a Framework

So, we can identify three distinct phases to this batch process:

* The ***Map*** phase
* The ***Shuffle*** phase
* The ***Reduce*** phase

![Distributed MapReduce 4](./img/L20%20Distributed%20MapReduce%204.png)


Each machine involved in the Map phase is sent a small program that, in this case, executes the following pseudo-code:

```
for each word W in document D {
  emit WordDocumentPair(W,D)
}
```

This program is known as a ***Map Function*** because the action passing every element in a list as an argument to a function is known as *"mapping"*.  The function is then said to have been *mapped* across the elements of the list.

Similarly, the machines involved in the reduce phase perform an equally simple task implemented in the ***Reduce Function***.  The reduce function takes the intermediate key/value pairs and first sorts them by key, then collates all the different values for the same key into a single list.


So Google's MapReduce system is framework into which you insert your map and reduce functions, then the framework handles all the ugliness of distributing your functionality across thousands of machines, handling all the communication, check-pointing and fault tolerance, and finally passing the data between the map, shuffle and reduce phases to generate the required output.

As the developer, in addition to providing your map and reduce functions, you also need to configure the MapReduce framework to tell it:

* How many workers you want allocated to the map phase? (E.G. 200,000)
* How many workers you want allocated to the reduce phase? (E.G. 5,000)
* On how many physical machines should all of those workers run? (E.G. 2,000)

There is a popular Open Source clone of Google's MapReduce known as [Hadoop](https://en.wikipedia.org/wiki/Apache_Hadoop) which includes its own clone of GFS known as HDFS (Hadoop Distributed Filesystem)

### Questions

***Q:***&nbsp;&nbsp; Is generating an inverted index what MapReduce is mainly used for?
***A:***&nbsp;&nbsp; The use case of the inverted index is the canonical example used to illustrate the general applicability of this technique to a wide range of problems.  MapReduce allows you to plug in your own map and reduce functions that are typically (but not exclusively) used to process large volumes of text data.

## Examples of Problems Solved Using MapReduce

Google's paper gives a variety of different problems that can all be solved using the MapReduce programming model.

* Word count
* Inverted index
* Distributed `grep`
* Distributed sort
* etc...

As long as you can find a way to express the solution to your problem in terms of a map function and reduce function, then the MapReduce framework will be able to help you.  The key points here are:

* You must be able to split your input data into units between which there are no dependencies (E.G. the individual documents retrieved by a crawler from a set of web sites)
* You must be able to write a map function that can be applied to these individual units of data ***in any order***
* The identity of the relevant reduce worker is determined when the intermediate key/value pairs are passed through the hash algorithm during the shuffle phase.
* The output of the reduce function(s) is/are the final analysed data from this run of the MapReduce framework

Additionally, you might need to provide certain configuration parameters for the number of map and reduce workers you expect to need, but in the end, the MapReduce framework implements all the plumbing code, leaving a couple of gaps into which you insert your own code.

---

| Previous | Next
|---|---
| [Lecture 19](./Lecture%2019.md) | [Lecture 21](./Lecture%2021.md)






# Distributed Systems Lecture 21

## Lecture Given by [Lindsey Kuper](https://users.soe.ucsc.edu/~lkuper/) on May 20<sup>th</sup>, 2020 via [YouTube](https://www.youtube.com/watch?v=sB9uiD-IUI0)

| Previous | Next
|---|---
| [Lecture 20](./Lecture%2020.md) | [Lecture 22](./Lecture%2022.md) |


## Recap: MapReduce Phases

The functionality of the MapReduce framework is divided into three distinct phases:

* The ***Map*** phase
* The ***Shuffle*** phase
* The ***Reduce*** phase

### The Map Phase

This is where the developer's map function is applied to all the input data.  The data types going into and coming out of the map function are typically not the data type seen in the final output.

In general, the map function's input type is some identifiable unit of data that needs to be analysed and can be supplied in the form of a key/value pair: for instance, to create an inverted index of words in a Web document, the key would be the URL of that document, and the value is the document's contents.

The map function then performs whatever analysis is required on that data and outputs a list of intermediate key/value pairs.  Initially, the output of the map function is written to local storage on each map worker machine.

#### Inverted Index Example

In the previous lecture, we used the simplified example of creating an inverted index.  Here, the input to our map function was:

```
<Doc1, <the, quick, brown, fox, jumped, over, the, lazy, dog>>
```

And the output was:

```
<the, Doc1>
<quick, Doc1>
<brown, Doc1>
<fox, Doc1>
<jumped, Doc1>
<over, Doc1>
<the, Doc1>
<lazy, Doc1>
<dog, Doc1>
```

#### Word Count Example

But MapReduce is a general-purpose framework that can perform many more tasks than simply creating inverted indices.  What if we wanted to take the same document as before and count word frequency?

So, our input data is exactly the same as before:

```
<Doc1, <the, quick, brown, fox, jumped, over, the, lazy, dog>>
```

And in the simplest case, the output could be nothing more than:

```
<the, 1>
<quick, 1>
<brown, 1>
<fox, 1>
<jumped, 1>
<over, 1>
<the, 1>
<lazy, 1>
<dog, 1>
```

Here, the word `the` occurs twice in the text, but this simple case defers the addition of multiple occurrences of the same word to the reduce phase; however, should we wish to implement this optimisation in the map function, then that would be fine.  E.G.:

```
<the, 2>
<quick, 1>
<brown, 1>
...
```

#### Distributed `grep` Example

Ok, but what about distributed `grep`?<sup id="a1">[1](#f1)</sup>

```
<Doc1, <the, quick, brown, fox, jumped, over, the, lazy, dog>>
<Doc2, <i, love, my, dog, spot>>
```

How the map function chooses to structure its output data is based entirely on what sort of results you want your `grep` function to produce.  For instance, let's say we want to search for the word `dog` in the above input data.  A naïve implementation of `grep` would output:

```
<Doc1, dog>
<Doc2, dog>
```

But a more sophisticated implementation may include the target word's context:

```
<Doc1, <lazy, dog>>
<Doc2, <my, dog, spot>>
```

or to take things a step further, the target word's context and a list of location offsets

```
<Doc1, <context, <lazy, dog>, offset, <7>>
<Doc2, <context, <my, dog, spot>, offset, <3>>
```

The point here is that the map function produces data in the form of key/value pairs.

Usually, these key/value pairs are qualified as being ***intermediate*** because they represent some halfway point in our calculation and require further processing by the reduce function.  However, in the case of distributed `grep`, the map function has already completed the required processing, either by identifying where in the document the target pattern occurs, or by returning an empty result; thus, in this case, the reduce function could be implemented as a ***do nothing*** function that simply returns whatever value it has been passed.<sup id="a2">[2](#f2)</sup>

### The Shuffle Phase

The shuffle phase is where all the intermediate key/value pairs created by the map workers are passed to the appropriate reduce workers for further processing.  But how do we decide which reduce worker is the right one?  This is decided by the partitioning function that implements some sort of hashing rule.

This partitioning function is supplied by the MapReduce framework and although Google doesn't exactly say ***how*** it has been implemented, they give the example that it could obey a rule such as `hash(key) mod N`, where `N` is the number of reduce workers.

As has already been pointed out, the `hash mod N` approach can introduce problems if `N` changes.  In the context of Amazon's Dynamo system, they are providing an online service that must be able to withstand unpredictable events such as sudden spikes in request volume, or hardware or network failure.  Under these circumstances, the likelihood of the number of nodes in a ring changing is high; consequently, Amazon mitigate the problems associated with changing `N` in `hash mod N` by using [consistent hashing](https://github.com/ChrisWhealy/DistributedSystemNotes/blob/master/Lecture%2019.md#consistent-hashing).

However, in the case of Google's MapReduce, they are working in an offline environment in which the size of the input dataset is known up front; therefore, if you are the developer of the map and reduce functions, you already have the necessary information to make an informed decision about how many workers you will need.  You then use these values to configure the MapReduce framework for the expected workload during your particular batch run.

So, altering the number of reduce workers during a batch run would only happen in the event of some sort of Byzantine error such as hardware failure or a network partition.  Under these circumstances, Google uses checkpointing for error recovery.  So, a changing value of `N` is not something you the developer really need to be concerned about.


### The Reduce Phase

***Q:***&nbsp;&nbsp; What data type does the reduce function work with?
***A:***&nbsp;&nbsp; Intermediate key/value pairs

The partitioning function provided by the MapReduce framework ensures that every key/value pair whose key hashes to the same value, is sent to the same reduce worker.  In practical terms, the reduce function accepts a set of key/value pairs whose hashed key values fall within a certain range.

Conceptually however, the data type of the reduce function is a key to which has been bound a set of values.  Whether the set of values bound to this key is created by the partitioning function or by explicit functionality within the reduce function is not strictly important here.

In the case of the word count example, the various map functions might output intermediate key/values pairs such as:

```
<the, 2>
<quick, 1>
<brown, 1>
<fox, 1>
<jumped, 1>
<over, 1>
<lazy, 1>
<dog, 1>
```

The key values go through the `hash mod N` algorithm which then determines which reduce worker will handle the next phase of the processing.  The output of a single reduce worker might then be the sum of all the word count totals received from the various map workers:

```
<the, 12>
<brown, 2>
<fox, 6>
<lazy, 4>
```

What about the distributed `grep` example?

In this case, each map worker either locates the search text in the document or it does not.  So, by the time we pass the results to the reduce function, the required processing has ***already*** been done.  So, the reduce function does not need to do anything other than write its input data directly to the output storage (GFS, for instance).

This turns out to be quite a common pattern: the reduce function is implemented as little more than the identity function (see endnote [2](#f2)).


## Handling Map Worker Failure

One detail we left out of the previous discussion was the use of a ***master*** process.  This process acts as the supervisor or scheduler for the work performed by all the workers.

The master periodically pings each of the workers and if they do not respond within a given timeout period, assumes that they have failed in some way.<sup id="a3">[3](#f3)</sup>

![MapReduce Master 1](./img/L21%20Master%201.png)

So, let's say that map worker `M1` now fails:

![MapReduce Master 2](./img/L21%20Master%202.png)

***Q:***&nbsp;&nbsp; What's happened to all the work `M1` was doing?  Is it lost or can it be salvaged?
***A:***&nbsp;&nbsp; Hmmmm, since `M1` is now unreachable, all of its work is also unreachable; therefore, it will have to be redone... :-(

Since map workers fail from time to time, what's the best way of handling this failure?  To answer this, Google had to examine the cost of the design options:

***Option 1)***
Ensure that every map worker writes its intermediate key/value pairs not to its local disk (that would become inaccessible in the event of failure), but to some external location from where it can be recovered

***Option 2)***
Risk having to redo all the work assigned to a map worker if that worker fails

The answer here is simply one of time &mdash; on average, which option will be quicker?

Option 1 means that the time penalty of writing data over the network must be paid on every ***successful*** run of a map worker.

Option 2 means that occasionally, we will have to pay a time penalty in order to redo a map worker's entire workload; however, since map workers are successful far more often than they fail, this penalty is not paid very often.

In general fault tolerance in distributed systems requires us to duplicate something.  So, in practice, we end up duplicating some combination of:

* ***Data***: by storing multiple copies
* ***Communication***: by sending multiple messages
* ***Computation (Effort)***: by occasionally having to redo some work

One of the distinguishing features of MapReduce is that it deliberately chooses to redo work in the event of worker failure because on average, this incurs a smaller time penalty than transferring data over the network.


## Combine Functions

Let's look at the word count example again.  Say we want to search for the word `dog` in the string:

```
My dog Spot is the best dog and the fastest dog
```

A naïve approach would be to scan the text and every time the target word is located, output an individual hit, resulting in:

```
<dog, 1>
<dog, 1>
<dog, 1>
```

But the downside of this is that three, identical intermediate key/value pairs must now be sent over the network to the reduce worker.  It would be far more efficient to derive a subtotal within the map function and then send only one intermediate key/value pair over the wire.

```
<dog, 3>
```

This job is performed by a ***combine function***.

A combine function performs a task very similar to that of the reduce function, but it runs inside the map worker in order to perform local optimisation.  This is perfectly valid because the overall task we're performing is associative.  `a + b` is the same as `b + a`, so the order in which additions are performed is immaterial.

So, generally speaking, if your MapReduce task is associative, then perform as much work in the map function as possible.  This has two advantages:

* It can significantly reduce the quantity of data that needs to be transferred during the shuffle phase
* The reduce function runs much faster because (in this case) it only needs to add up subtotals, rather than all the individual values discovered by the map functions.

## Map and Reduce Function Types

### Map Function

The map function needs two arguments:

1. A function that performs the required transformation on a single list item, and
1. A list of items to be transformed

The MapReduce framework then works its way down the list, passing every element in turn to your Map function and storing the results in a new list.

The datatypes used by the map function would be written like this in Haskell:

```haskell
map :: (a -> b) -> [a] -> [b]
```

Breaking this down:

* `map :: (a -> b)` means that the first argument to `map` is a function.  This function takes an input of type `a` and returns an output of type `b`
* `-> [a]` means that the second argument to `map` is a list in which all the items are of type `a`
* `-> [b]` at the end means that the final result is of type `b`

This function would then be implemented as follows:

```haskell
map _ [] = []
map f (x:xs) = f x : map f xs
```

So here, we have described how `map` should behave in two situations.  The first is:

```haskell
map _ [] = []
```

Here, if map is passed an empty list `[]`, then all we will do is respond with another empty list `[]`.  The underscore after `map` means that in the case of receiving an empty list, we don't care what type of function is supplied, because that function isn't going to be called anyway...  This is known as the ***base case*** and serves the vital role of terminating the recursive calls to the `map` function.

The second case is more interesting because this is where `map` is passed a non-empty list:

```haskell
map f (x:xs) = f x : map f xs
```

The first argument passed to `map` is a function called `f`, and second argument is the list of items over which `f` will be mapped.  This list is destructured into the variables `x` and `xs`, where `x` contains whatever value is found at the head of the list, and `xs` contains whatever else is left in the tail.

We then call function `f` passing it `x` as an argument and concatenate what we get back to the result of recursively calling `map` passing in function `f` and whatever is left over in `xs`.

This is how we can recursively call function `f` on the elements in the ever-decreasing list `xs`.  For each call to `f`, `xs` becomes one element smaller and eventually becomes the empty list.  At this point we have hit our base case and recursion terminates because the list has been fully processed.

So, a simple example would be:

```haskell
map increment [1,2,3] = [2,3,4]
```

### Reduce Function

In some programming languages, `reduce` is also known as `foldr` meaning *"fold the values in the list towards the right"*.

Whereas a map function needed two arguments, a reduce function needs three:

1. A function that does the reducing,
1. Some starting (or base) value, and
1. A list of values that need to be reduced

In Haskell, this type would be declared like this:

```haskell
reduce :: (a -> b -> b) -> b -> [a] -> b
```

Breaking this down:

* `reduce :: (a -> b -> b)` means that the first argument to `reduce` is a function.  This function takes a value of type `a` and a value of type `b` and gives back a value of type `b`.
* `-> b` means that `reduce` also takes second value of type `b`
* `-> [a]` means that `reduce` also takes a third value that is a list of values of type `a`
* `-> b`  at the end means the overall value returned by `reduce` is of type `b`

So how do we run the function passed to `reduce`?  This function needs two arguments; a value of type `a` that comes from whatever list we're reducing, and a value of type `b`.  But what is this value of type `b`?  This value is known variously as the *"identity value"* or the *"base value"* or simply the *"accumulator"*, and acts as a starting value.

In the case that we are trying to reduce an empty list, then whatever value is supplied as the identity or base value is simply returned unmodified.  Traditionally, the value supplied as the base case is known as the *"zero"* value, hence the `z` in the code sample below;

```haskell
reduce _ z [] = z
```

As with the base case of the `map` function, the underscore here means that when `reduce` is passed an empty list, we couldn't care less about what type of function we've been supplied, because it's never going to be called anyway!  So, all we do is give back the initial zero value `z`.

In the case where `reduce` is passed a list:

```haskell
reduce f z (x:xs) = f x (reduce f z xs)
```

We call function `f` passing in the first value from the list (destructured into variable `x` which is of type `a`), but from where do we get the value of type `b`?  Well, we know that the `reduce` function gives us back a value of type `b`, so we recursively call `reduce` on the tail of the list (destructured into variable `xs`) and use whatever value it returns as the required value of type `b`.

So, a simple example of the word count reduce function looks like this:

```haskell
reduce add 0 [1,1,2,1,] = 5
```

---

| Previous | Next
|---|---
| [Lecture 20](./Lecture%2020.md) | [Lecture 22](./Lecture%2022.md) |


---

***Endnotes***

<b id="f1">1</b>&nbsp;&nbsp; `grep` is often thought to be a contraction of ""***G***lobal ***Rep***lace", but the actual meaning is "***G***lobally search for a ***r***egular ***e***xpression and ***p***rint matching lines"

[↩](#a1)

<b id="f2">2</b>&nbsp;&nbsp; A function that simply returns its argument unmodified is known as the ***Identity*** function.  In JavaScript, such a function is implemented simply as

```javascript
const ident = x => x
```

[↩](#a2)

<b id="f3">3</b>&nbsp;&nbsp; Remember, in a network using asynchronous communication, a crashed process is indistinguishable from a running process that has simply stopped responding to messages.

[↩](#a3)

# Distributed Systems Lecture 22

## Lecture Given by [Lindsey Kuper](https://users.soe.ucsc.edu/~lkuper/) on May 29<sup>th</sup>, 2020 via [YouTube](https://www.youtube.com/watch?v=qmFoSeSvarA)

| Previous | Next
|---|---
| [Lecture 21](./Lecture%2021.md) | [Lecture 23](./Lecture%2023.md)


## Keeping Replicas Consistent

Consider the following scenario in which we need strong consistency, but we have:

* A datastore held across multiple replicas
* These replicas have no leader nor coordinating process (I.E. We're not using Primary Backup or Chain Replication)
* Any replica can receive an update

The challenge then concerns how to keep these replicas consistent with each other.

What approach should we adopt?

Well, we could use a consensus protocol to decide which updates should processed in which order.

![Replica Consensus 1](./img/L22%20Replica%20Consensus%201.png)

If replica `R1` receives update `A` and replica `R2` receives update `B`, then an agreement must be reached concerning the order in which these updates should be delivered.

So, even though the messages will arrive in some unpredictable order, a consensus protocol will be used to decide upon the delivery order.  In this case, both replicas operate a system of delivery slots and the consensus protocol determines that event `B` should occupy delivery slot `1` and event `A` should occupy delivery slot `2`.

***Q:***&nbsp;&nbsp; But how many messages need to be sent in order to arrive at this agreement?
***A:***&nbsp;&nbsp; Lots!

Here's an example showing the messages that need to be exchanged for replicas <code>R<sub>1</sub></code> and <code>R<sub>2</sub></code> simply to agree on a total order for delivering events `A` and `B` shown above.

![Replica Consensus 2](./img/L22%20Replica%20Consensus%202.png)

1. Replica <code>R<sub>2</sub></code> sends out a `prepare(6)` message to a majority of acceptors, who each respond with the corresponding `promise` messages.
    4 messages
1. Just a little time after <code>R<sub>2</sub></code>'s message exchange has taken place, replica <code>R<sub>1</sub></code> sends out its `prepare(5)` messages to a majority of acceptors.  Acceptor <code>A<sub>1</sub></code> happily accepts this proposal number, but acceptor <code>A<sub>2</sub></code> has already promised to ignore messages with a proposal numbers less than `6`, so this `prepare` message is ignored and replica <code>R<sub>1</sub></code> left hanging.
    3 messages (all of which turn out to be redundant)
1. Replica <code>R<sub>2</sub></code> sends out its `accept(6,(slot_1,B))` messages to the acceptors who each respond with `accepted(6,(slot_1,B))`.  So, event `B` now occupies delivery slot 1.
    4 messages
1. Replica <code>R<sub>1</sub></code> still needs to get agreement on a total order for event `A`, so it tries the prepare/promise phase again, but now with proposal number `7`.  This time, the proposal number is accepted.
    4 messages
1. Replica <code>R<sub>1</sub></code> then enters the accept/accepted phase and achieves consensus on event `A` occupying delivery slot 2.
    4 messages

So, even in this reasonably happy example where we are not sending messages to all the acceptors (only a majority), we've had to send 19 messages, 3 of which turned out to be redundant &mdash; and we haven't even accounted for sending messages out to the learners!

The point here is that consensus algorithms are really expensive; therefore, we should only implement them in situations where it's ***extremely*** important that everybody agrees on a total order.

So far however, we have not even discussed what events `A` and `B` represent.  Consensus algorithms do not care about a message's payload; they simply see an opaque (I.E. meaningless) block of data to which some metadata has been attached.  Causal Broadcast for instance, looks simply at the message's recipient and the vector clock value, and from these values, determines the delivery order.

> ***My Aside***
>
> A useful analogy here is to think of the people working in a mail sorting room.  These people are concerned with the fact that all the letters and packages have been addressed correctly, and that the correct postage has been paid for a letter or package of that weight and dimensions.
>
> It is quite irrelevant for these people to concern themselves with the contents of the letters and packages.

However, from the perspective of the human developer, we can see firstly that we're having to go to a lot of trouble simply to agree on the order in which a set of events are delivered, and secondly, the algorithm that determines the delivery order is completely agnostic to the real-life functionality that needs to be performed as a result of processing those events.

Rather than having a message-agnostic consensus algorithm then, wouldn't it be smarter to make intelligent decisions about delivery order based on our knowledge of the functionality being implemented?

### Safety Properties: Do We Really Need Strong Consistency?

Let's go back to the shopping cart scenario described in [lecture 17](./Lecture%2017.md).

![Amazon Shopping Cart 1](./img/L17%20Amazon%20Cart%201.png)

If replicas `R1` and `R2` simply represent shopping carts, then we certainly don't want to go to all the trouble of running a consensus algorithm.  But we have arrived at this conclusion based on our knowledge of the business process we are implementing.  In this case, we really don't care whether a book is added to the shopping cart before or after the pair of jeans.  From the perspective of the business logic, the order is neither here nor there.

Of course, there will be some situations in which message delivery order is critical to the logic of your business process, but what we propose here is that strong consistency is needed only in a minority of cases; the greater majority of business scenarios will function quite happily with ***strong convergence***.

Just as a reminder:

***Strong Consistency***
If replica `R1` delivers messages in the order `M1`, `M2` and `M3`, then all replicas receiving the same set of messages must deliver them in the same order.  Only then can it be known that the replicas have equivalent state.

***Strong Convergence***
All replicas delivering the same set of messages eventually have the equivalent state.

Strong convergence might still be tricky to implement, but it will be easier than strong consistency, because with strong convergence, we know that state equivalence can be achieved simply by delivering the same set of updates.  Strong consistency however requires us to deliver the same set of updates in ***precisely the same order***.

The bottom line here is that you should only implement strong consistency when you have no other choice.

## How Do We Generalise the Requirement for Strong Convergence?

To do this, we will need to look back at the definition of a partially ordered set that we covered in lectures [3](./Lecture%203.md) and [4](./Lecture%204.md).

As a reminder, a partial order allows you to compare the members of set `S` using a binary relation such as `≤` (less than or equals).  However, the word *"partial"* in the name tells us that not every pair of elements in the set is comparable.

This relation is governed by three axioms:

| Property | English Description | Mathematical Description |
|---|---|---|
| Reflexivity   | For all `a` in `S`,<br>`a` is always `≤` to itself | `∀ a ∈ S: a ≤ a`
| Anti-symmetry | For all `a` and `b` in `S`,<br>if `a ≤ b` and `b ≤ a`, then `a = b` | `∀ a, b ∈ S: a ≤ b, b ≤ a => a = b`
| Transitivity  | For all `a`, `b` and `c` in `S`,<br>if `a ≤ b` and `b ≤ c`, then `a ≤ c` | `∀ a, b, c ∈ S: a ≤ b, b ≤ c => a ≤ c`

The standard example of a partially ordered set is set inclusion &mdash; that is the set of all possible subsets of a given set.

For example, if we have a set containing:

| | |
|---|---|
| ![Book](./img/emoji_book.png) | A book
| ![jeans](./img/emoji_jeans.png) | A pair of jeans
| ![Torch](./img/emoji_torch.png) | A torch

Then the inclusion set (the set of subsets) will contain the following eight members:

![Set of Subsets](./img/L22%20Set%20of%20Subsets.png)

Our relation here is the *"less than or equals"* operator `≤`.  Using this operator, certain members of our set of subsets can be compared as follows:

![Comparable Subsets 1](./img/L22%20Comparable%20Subsets.png)

However, other members are not comparable; for instance:

![Noncomparable Subsets](./img/L22%20Noncomparable%20Subsets.png)

### Upper Bounds

If we select some elements from our set of subsets, say the singleton set containing the jeans `{👖}` and singleton set containing the torch `{🔦}`, we could ask the following question:

> Which elements of `S` are at least as big as `{👖}` and  `{🔦}`?

The answer here is:

> Any set that contains at least the union of `{👖}` and `{🔦}`.

So, this would be the sets `{👖,🔦}` and `{📓,👖,🔦}`.  These two sets are known as the ***upper bounds*** of `{👖}` and `{🔦}`.

In more formal language, the upper bound is:

> Given a partially ordered set<sup id="a1">[1](#f1)</sup> (`S`, `≤`) an upper bound of `a,b ∈ S` is an element `u ∈ S` such that `a ≤ u` and `b ≤ u`.

Notice that we talk of ***an*** upper bound.  This means it is possible that for the members `a` and `b` there could well be multiple examples of some set `u` that all satisfy the upper bound requirements.

### Which Upper Bounds are Going to Be the Most Interesting?

The upper bound set that contains all the members of the original set is not very interesting because this will always be a common upper bound for all its subsets, so we can ignore this one.

Generally speaking, the upper bounds that are the most interesting are the smallest ones.  But how do we define the smallest upper bound?  The formal definition is:

>  If `a`, `b`, `u` and `v` are all members of the inclusion set `S`, then `u` is the least upper bound<sup id="a2">[2](#f2)</sup> of `a,b ∈ S` if `u ≤ v` for each `v`

### Join-semilattice

***Q:***&nbsp;&nbsp; If `S` is the eight-member inclusion set of `{📓,👖,🔦}`, then is it true that every 2 elements of `S` will have a least upper bound (lub)?
***A:***&nbsp;&nbsp; Yes!

Any set for which this property is true is given the fancy name of a ***Join-semilattice***.

> A partially ordered set (poset) in which every 2 elements have a least upper bound (lub) is called a join-semilattice.


So, it follows therefore that if some partially ordered sets are join-semilattices, then there should also be some partially ordered sets that are not.

It's quite hard to think of a set within which every 2 elements ***do not*** have a least upper bound (I.E. think of a set that is not a join-semilattice), but a good example is a Boolean register.  This is a tri-state variable that can be either `empty`, `true` or `false`

So, the poset is simply `{empty, true, false}`.  This is a very simple set containing only three members that can be arranged as follows:

![Boolean Ordering](./img/L22%20Boolean%20Ordering.png)

These values can also be ordered using the `≤` operator:

```
empty ≤ empty
 true ≤ true
false ≤ false

empty ≤ true
empty ≤ false
```

So, is this a true partially-ordered set?  To answer this question, we must check that all the axioms are satisfied.

***Reflexivity***
Since `empty ≤ empty`, `true ≤ true` and `false ≤ false`, then this set satisfies the requirements of reflexivity.

***Anti-symmetry***
Anti-symmetry requires that if `a ≤ b` and `b ≤ a`, then `a = b`.  However, since this set contains only three members arranged in a two-layer lattice, we have already implicitly satisfied anti-symmetry by satisfying the requirements of reflexivity.

***Transitivity***
Transitivity requires that if `a ≤ b` and `b ≤ c` then `a ≤ c`.  However, no members of the set can be compared this way, so this set obeys transitivity only in a vacuous sense.

So, this Boolean Register qualifies as a true partially-ordered set; however, we can see that if we picked the elements `true` and `false` and asked *"What is their least upper bound?"*, then we can see that there isn't one.  Therefore, this set is not a join-semilattice.

### What's This Got to do with Distributed Systems?

Let's say we have a system with two replicas that hold a type of information that is very different to the shopping cart example.  Here, these replicas hold the value of our Boolean register and they then receive conflicting updates:

![Conflicting Updates](./img/L22%20Conflicting%20Updates.png)

***Q:***&nbsp;&nbsp; Why do these updates create a conflict?
***A:***&nbsp;&nbsp; Because we have no way to combine the values `true` and `false`

***Q:***&nbsp;&nbsp; Why can we not combine these values?
***A:***&nbsp;&nbsp; Because, as we can see from the lattice diagram above, `true` and `false` have no upper bound, let alone a least upper bound.

In this case, the inclusion set formed form the members `{empty, true, false}` contains only the members:

```
S = { {}
    , {empty}
    , {true}
    , {false}
    , {empty, true}
    , {empty, false}
    }
```

The inclusion set does not contain the least upper bound member `{true, false}` neither does it contain the upper bound `{empty, true, false}`.

In order to resolve such a conflict, we would need to implement some sort of consensus algorithm.  However, because consensus algorithms are expensive, we really don't want to implement one unless we really need to.

So generally, if the updates your replicas are receiving can be thought of as the members of a set this ***is*** a join-semilattice, then we can resolve the requirements of strong convergence by taking the least upper bound.  This also means we do ***not*** need to implement a consensus algorithm.

So, here's an informal claim:

> If the states that replicas can take on can be thought of as elements of a join-semilattice, then there is a natural way of resolving conflicts between replicas without needing a consensus algorithm.

This claim is described as *"informal"* because it uses unqualified words such as *"natural"*.  Nonetheless, there is a lot of interesting work being done on this type of conflict resolution.  If you're interested in this type of work, take a look at a topic called [*"Conflict-Free Replicated Datatypes"*](https://crdt.tech/) or (CRDTs).  An example implementation by Martin Kleppmann and Alastair Beresford has been described in this [paper](./papers/JSON%20CRDT.pdf) for JSON datatypes.

## Back to the Shopping Cart...

So far, we've been thinking about conflicts that can arise when different clients add members to a set. In the case of the shopping cart, the order in which items are added does not matter because the different members within the shopping cart have no dependency on each other.  Therefore, this situation is not one in which consensus is required.

This is a particularly useful property in the event of a network partition.  If communication is lost for some period of time between replicas, then the fact that the states of the shopping carts might diverge whilst the network partition exists does not create a problem.

As soon as the partition heals, the replicas can communicate with each other again, and their states will converge.

But what happens if we are allowed to remove items from the shopping cart?

Now things get more complicated.

Let's say that from your laptop, you add a book to your shopping cart, and from your phone, you add a pair of jeans.

![Shopping Cart Item Deletion 1](./img/L22%20Delete%20Cart%20Item%201.png)

Both replicas synchronise and everything is fine...

From your laptop however, you've read some reviews of the book and decide that it doesn't look so interesting, so you remove it from your shopping cart &mdash; right at the very moment a network partition appears between the replicas.

![Shopping Cart Item Deletion 2](./img/L22%20Delete%20Cart%20Item%202.png)

The remove message gets through to replica 1, but not replica 2 resulting in the shopping carts being out of sync with each other.

Now from your laptop, you want to look at the contents of your shopping cart and... huh!?  That book has popped up again!

![Shopping Cart Item Deletion 3](./img/L22%20Delete%20Cart%20Item%203.png)

Maybe it's a sign that you really should read that book... or maybe it's the situation described in the Dynamo paper where, under certain circumstances, deleted items can reappear in shopping carts.

Why did this happen?

Because the contents of the shopping carts are treated as sets, and when a conflict occurs, the solution is to take the least upper bound.  With Dynamo, this resolution happens on the client, but with CRDTs, it happens in the replica.  Either way though, this approach takes the union of the sets and this can cause a deleted item to pop up again.

So how do we avoid this problem?

We could go to all trouble of ensuring that the members of your set (I.E. the contents of your shopping cart) are always the members of a join-semilattice; however, this means that you have to throw the whole cart away as soon as any item is deleted.

But wait!  There's a trick that allows us to handle this situation.  Here, we will keep track of all additions to the shopping cart in one set and all the removals from the shopping cart in a different set known as the ***Tombstone Set***.  In this case, the least upper bound of two versions of a shopping cart can be calculated simply by taking the union of the sets.


| `R1`<br>Additions | `R1`<br>Removals | `R2`<br>Additions | `R2`<br>Removals
|---|---|---|---
| 📓 | 📓 | 👖 |
| 👖 | | 📓 |

Even though replica `R2` never found out about the removal of the book, this does not matter, because that fact has been recorded in replica `R1`.  So now we can avoid having the deleted item reappear in the shopping cart by taking a two-step approach:


1. Take the union of the addition sets
1. From this, subtract the union of the removal sets

But we still haven't solved all our problems...

Let's say that even though all those bad reviews about the book caused us to delete it, we change our mind (I mean, can a book really be that bad? Let's find out).  So you add the book again.

However, look at the addition set &mdash; it already contains the book, and our addition set can only hold single instances of an item.  And the book is still in the tombstone set because we really did delete it.  So, if we left the situation like it is, even though we added the book a second time, it would disappear from the resolved shopping cart because it's in the tombstone set...

So, under these conditions, once you remove an item, it’s never coming back!

Here is where you need to do some serious design work to decide on what behaviour you want your application to have, and then think of the scenarios that could break that behaviour.

If you know that the addition of previously deleted items will be a frequently used aspect of your application's functionality, then you will need to implement some sort resolution strategy.  For instance:

* You could have of global coordination point in which all the replicas are notified that a previously deleted item is being added again and then try to ensure that everyone agrees.
* Or you could take a simplistic approach and say that additions always win over removals.
* Or you could keep a counter against each added or removed item so that adding the same book twice sets the addition counter to `2`, and removing it sets the removal counter to `-1`. Now the desired total is simply the sum of additions total and the removals total.

The bottom line is this: this is hard to get right and has been an active area of research over the last 10 years or so.  Quite a few interesting data structures have been proposed for resolving this problem, but it does not appear that any of them have been implemented in production systems yet.

As a developer however, it is difficult to reason about the data you are working with in this abstract manner. The question *"Can I really treat my data as elements of a join-semilattice?"* is difficult to answer and typically requires the help of specialist verification tools.

This is an area of research in which Lindsey Kuper is actively involved.

---

| Previous | Next
|---|---
| [Lecture 21](./Lecture%2021.md) | [Lecture 23](./Lecture%2023.md)


---

***Endnotes***

<b id="f1">1</b>.  The name "partially ordered set" is often abbreviated to ***"poset"***

[↩](#a1)

<b id="f2">2</b>.  The "least upper bound" is known as "lub" or "join"

[↩](#a2)


# Distributed Systems Lecture 23

## Lecture Given by [Lindsey Kuper](https://users.soe.ucsc.edu/~lkuper/) on June  1<sup>st</sup>, 2020 via [YouTube](https://www.youtube.com/watch?v=tqCUDPWE0JE)

| Previous | Next
|---|---
| [Lecture 22](./Lecture%2022.md) |

## Original Plan for this Lecture

Originally, the plan for this lecture was for Lindsey to talk about her own research, but she changed her mind.  If you'd like to read/watch more about Lindsey's research, please use the following resources:

* [Abstractions for Expressive, Efficient Parallel and Distributed Computing](https://www.youtube.com/watch?v=4h7YBUXiCZE)
* [Lindsey's homepage at USCS](https://users.soe.ucsc.edu/~lkuper/)

## Recap of a Diagram Used by Chris Colohan

Let's go back to the illustration Chris Colohan used in his talk on [Blockchain Consensus](https://www.youtube.com/watch?v=m6qZY7_ingY) given to this class on May 27<sup>th</sup>, 2020.

He used a diagram that illustrates various strategies for implementing fault-tolerance.

![Fault Tolerance Hierarchy](./img/L23%20FT%20Hierarchy.png)

The point here is that everything in distributed systems is a trade-off.  In order to achieve goals such as low response times, high throughput, implementation simplicity and low running costs, you must accept the risk that if certain types of fault occur, then these will have a potentially significant impact on your system.  Depending on how significant the consequences of these faults are, you have to make an informed decision that balances the consequences of failure with the cost of protecting against such failure.

Since Paxos is the only strategy we've really talked about during this course, let's fill in a few of these gaps.

### 2-Phase Commit (2PC)

In the discussions we've had in this course, we have been talking about Primary Backup Replication and Chain Replication as the more basic forms of fault-tolerance.  These two techniques could be placed at the same location as 2-phase commit in this diagram.

2-phase commit is typically used in a database that operates with some number of replicas.  Here, everyone needs to agree on what action should be taken for the current logical unit of work (LUW).  There is typically some coordinating process that goes out to the other replicas and asks them the "go/no go" question of *"Do you want to commit or abort?"*

But why would one replica want to abort the LUW when the others are happy to commit?  Typically, this situation happens due to some hardware issue such as running out of disk space.

A key difference here between 2PC and a consensus algorithm is that the coordinator cannot accept a commit response from a majority of replicas, it must receive unanimous agreement from ***all*** the replicas before the commit can proceed.

If all the replicas respond with `commit`, then the coordinator will instruct all the replicas to commit, otherwise it instructs them to abort.

The point here is that just like Primary Backup Replication or Chain Replication, if you want fault-tolerance, then you must have a primary or coordinator process.  However, having only one coordinator process still does not provide fault-tolerance because that coordinator might crash.  Therefore, in order to implement fault-tolerance, you need a cluster of coordinator processes that can all agree on a course of action by means of some sort of consensus protocol.

Alternatively, you could use a protocol such as Paxos or RAFT in which there is no distinct "coordinator" process, but all the replicas coordinate directly with each other whilst performing at least one of the roles of proposer, acceptor or learner.

This diagram is good for illustrating the fact that 2-phase commit is typically not designed to be fault-tolerant: 2PC implementations typically have only one coordinator process.

The obvious question at this point then is this:

> Why not implement 2-phase commit ***and*** have a cluster of coordinator processes to provide fault-tolerance?

Well, this has already been done and is described in the first paper we're going to look at.

### Consensus on Transaction Commit

This is a [2006 paper](./papers/paxoscommit-tods2006.pdf) by Jim Gray and Leslie Lamport.

This paper describes a 2-phase commit system in which there is a cluster of coordinator processes that run a Paxos consensus algorithm between them on the commit/abort decision.

Here, a system is described in which `F` coordinator processes are allowed to fail, thus requiring the system to have a total of `2F + 1` coordinators up and running when it starts.

The original, single-process 2PC system described above is where `F` in the above equation equals `0`.  In other words, zero processes are permitted to fail because the system has started with only one coordinator in the first place.

One of the key points to realise here is that the concepts of consensus and replication are inextricably linked.  One of the most common reasons to implement a consensus algorithm is to perform replication.

How those replicas agree is less important.  You might choose to have a cluster of coordinator processes that tell the replicas when to commit or abort; or, you might choose to implement Paxos so the replicas can directly coordinate with each other.

### Practical Byzantine Fault-Tolerance (PBFT)

This is another [classic paper](./papers/pbft.pdf) published in 1999 by Miguel Castro and Barbara Liskov. Barbara Liskov has made some fundamental contributions to programming language design, especially in the area of object-oriented design.

PBFT is a replication technique that tolerates Byzantine faults, and in spite of having the word *"practical"* in the name, it is not used in practice that often.

The distinguishing feature of this fault-tolerance behaviour is that if you have a system with `n` replicas, then `floor((n - 1) / 3)` of those replicas are allowed to "fail".  The world "fail" is put in quotation marks because what we mean here is really *"exhibit Byzantine behaviour"*.  By this, we mean that a process could:

* Genuinely crash
* Pretend to crash
* Disappear due to a network partition
* Act in a malicious way
* Some other behaviour not listed here...

It turns out that in practical terms, PBFT requires a minimum of 5 replicas in order for the system to tolerate a single failure.

Paxos, on the other hand, can work just fine if 1 out of 3 acceptors fail, because 2 is still a majority (and here, we're simply talking about crash failures and omission failures, not Byzantine behaviour).

Since protection against Byzantine behaviour is a stronger notion of fault-tolerance, then it makes sense that we require a minimum of 5 replicas for this strategy to work.

As we saw in the diagram above however, the more replicas you have, the more expensive and complex the strategy is to implement, and the slower it runs due to the higher number of replicas that must all agree before anything can get done.  So overall, a much bigger investment is needed to protect against a type of fault that might not happen very often.

This paper was very influential when it was released because previous strategies for protecting against Byzantine faults were much slower; unfortunately, it’s still not as fast as ***not*** protecting against Byzantine faults.

### Blockchain "Consensus"

Of all the available fault-tolerance models, this one is the most expensive to run.  This is mainly because you need some seriously powerful number-crunching hardware to perform blockchain mining.  This in turn gives you very large electricity bill and increases your impact or the environment...

The term consensus is in quotes here because in strategies such as Paxos and RAFT, there is a very definite point in the algorithm where you know that consensus has been reached, and then there is no going back.  With Blockchain "consensus", the algorithm never reaches a specific milestone; instead, you only have a probabilistic guarantee that consensus is likely.


### Where Does This Leave Us?

If you can get away with not needing strong consistency between replicas, then that will be a good choice because it will save you a large amount of time, energy and money both during the implementation and at runtime.

Overall, go for the weakest safety property you can reasonably tolerate.  Hence the suggestion to use strong convergence instead of strong consistency, or the development of techniques such as Conflict-Free Replicated Datatypes (CRDTs).

## Discovering Who Invented Vector Clocks

It is not clear who first invented vector clocks, and in many respects, attribution of this concept to a single person or group is not of much consequence; however, it is interesting to trace the development of this idea.

Firstly, we can place a lower bound on the date by referring to the first paper to treat distributed systems as a science.  This paper was written by Leslie Lamport in 1978 and was called [Time, Clocks and the Ordering of Events in Distributed Systems](./papers/TCOEDS.pdf).  In it, the concept of the *"happens before"* relation was properly defined as was the notion of a Logical or Lamport Clock.

A couple of interesting things to notice about the space-time diagrams (now known as "Lamport Diagrams") shown in this paper are:

1. Stylistically, they bear a passing resemblance to Feynman Diagrams (maybe there is an influence from physics because the final section of this paper on physical clocks seems only to make sense to physicists; and even then, that proposition is not entirely sound...)
1. He has time going upwards; which does tend to make them harder to read

Later, these diagrams have been drawn to show time going left, right or down.  Lamport however, is one of the few people to draw these diagrams with time going up.

### Concepts Introduced in Lamport's First Paper

* Logical, or Lamport Clocks
* The *"Happens Before"* relation denoted by the arrow `->` syntax
* The idea of the *"clock condition"* that can test whether the happens before relation is satisfied for a pair of events.
    For events `a` and `b`, if `a -> b` then `C(a) < C(b)` where `C(a)` and `C(b)` are the respective *"clock conditions"* of events `a` and `b` - in other words, the value of the Lamport Clock associated with each event.
* Initial proposition for turning the partial order implemented by Lamport Clocks into a total order.  This idea, however, requires that if two events have the same clock value, then an arbitrary algorithm is used to decide the outcome; for instance: events happening on process `P1` might always be assumed to have happened before events on process `P2`.
* Distributed Mutual Exclusion Algorithm.  This controls how to manage exclusive access to a shared resource for a group of processes. However, no one actually uses this algorithm for the simple reason that it's not fault-tolerant.
* The observation that distributed processes simulate the execution of State Machines

### The "Holy Grail" Paper

Although the idea of vector clocks was developed by several researchers independently, and certainly before the publication of this paper, the ["Holy Grail" paper](./papers/holygrail.pdf) is worth reading because it describes how to detect causal relationships in distributed systems.

It covers topics such as:

* How in certain circumstances, vector clocks provide a better mechanism than Lamport Clocks for determining causal relationships
* Are vector clocks even the best solution?

Footnote 3 of this paper makes an interesting comment:

> Actually, the concept of vector time cannot be attributed to a single person. Several authors “re-invented” time vectors for their purposes, with different motivation, and often without knowing of each other. To the best of our knowledge, the first applications of “dependency tracking” vectors [70] appeared in the early 80’s in the field of distributed database management [21, 74]. In [17] and [44], however, vector time is introduced as a generalization of Lamport’s logical time, and its mathematical structure and its general properties are analysed.

At the end of this footnote, two references are given to a paper by Colin Fidge [17] and a paper by Friedemann Mattern [44]

### Colin Fidge's Paper: "Timestamps in Message-Passing Systems That Preserve the Partial Ordering"

[This paper](./papers/fidge88timestamps.pdf) was published by Colin Fidge in 1988 and without calling them *"vector clocks"* he invented the same concept by saying:

> Rather than a single integer value, timestamps are represented as an array
>
> <code>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<i>[C<sub>1</sub>,C<sub>2</sub>,&hellip;,C<sub>n</sub>]</i>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</code>
>
> with an integer clock value for every process in the network.



### Friedemann Mattern's Paper: "Virtual Time and Global States in Distributed Systems"

[This paper](./papers/VirtTime_GlobState.pdf) was published by Friedemann Mattern also in 1988 where, on the second page, he states:

> In this paper, we aim at improving Lamport's virtual time concept. We argue that a linearly ordered structure of time is not always adequate for distributed systems and that a ***partially ordered system of vectors*** forming a lattice structure is a natural representation of time in a distributed system

There's the use of vectors again to hold a set of individual clock values.

Then in section 3, Mattern talks about *Consistent Cuts* that we have already looked at in the context of snapshots and the Chandy-Lamport Algorithm.  The interesting thing here is that although the Chandy-Lamport algorithm predates Mattern's paper by a few years, at the time Chandy and Lamport devised their snapshot algorithm, vector clocks had not yet been invented.

Here, Mattern now ties together (apparently for the first time), the use of consistent cuts with the use of clock values held in vectors.

### Frank Schmuck's 1988 PhD Paper

In 1988, a German PhD student at Cornell by the name of Frank Schmuck<sup id="a1">[1](#f1)</sup> published his thesis on ["The Use of Efficient Broadcast protocols in Distributed Systems"](./papers/Frank%20Schmuck%20PhD%20Paper.pdf)

On page 53, Schmuck states:

> In [Lam78] Lamport introduced *logical timestamps*, integers assigned to each event in such a way that if all events are ordered by their timestamp this order is consistent with "`->`". We can generalize this idea to timestamps which are ***vectors of integers*** [Sch85].<sup>2</sup>  Such timestamps are useful for keeping track of the partial order of events as the system executes.
>
> A timestamp *`t`* for an event <code>e = event<sub>R</sub>⟨i,j⟩ ∈ R</code> is a vector of *`n`* integers with the following meaning:
>
> <code>t<sub>e</sub>[k]= || {event<sub>R</sub>(k,l) ∈ <sub>k</sub> | event<sub>R</sub>(k,Z) → e} ||</code>
>
> i.e., <code>t<sub>e</sub>[k]</code> is the number of events at *`k`* that precede *`e`* in the partial order.

There's that phrase again *"vectors of integers"* and a citation to his own, unpublished manuscript of 1985.  However, footnote 2 says the following:

> <sup>2</sup> The idea of vector timestamps was developed independently by Ladin and Liskov [LL86].

So, let's chase after the paper referenced as LL86.

### Ladin & Liskov's Paper: "Highly-Available Distributed Services and Fault-Tolerant Distributed Garbage Collection"

[This 1986 paper](./papers/Ladin%20and%20Liskov.pdf) by Rivka Ladin and Barbara Liskov did not use the precise name *"vector clock"*; however, it did use the name *multipart timestamps*:

> We solve this problem by using multipart timestamps, where there is one part for each replica. Thus, if there are `n` replicas, a timestamp `t` is
>
> <code>t = &lt;t<sub>1</sub>, &hellip;, t<sub>n</sub>&gt;</code>
>
> where each part is a positive integer. Since there will typically be a small number of replicas (e.g., 3 to 7), using such a timestamp is practical.

### Skipping Forward to 1991 and Causal Broadcast

Frank Schmuck's doctoral supervisor was Ken Birman, and in 1991, he published a paper called [Lightweight Causal and Atomic Group Multicast](./papers/birman91multicast.pdf).  In section 4.3 called *"Vector Time"*, they now start to talk about vector clocks, and their description is exactly what we discussed in [lecture 5](./Lecture%205.md#vector-clocks).  This discussion of vector clocks then forms the foundation of the paper's main subject, which is Causal Broadcast.

The key part of the Causal Broadcast discussion then states in section 5.1 that after a message has been received, its delivery is delayed until various conditions have been fulfilled concerning the vector clock values in the message and the vector clock values held in the receiving process.

In class we spoke of the rule that when a message is delivered, the vector clock value in the sender's position should be incremented; but here in Birman's paper, he says effectively *"just merge the sender and receiver's clocks using a pointwise maximum"*.  Although this sounds like a discrepancy, it turns out that these two approaches are functionally equivalent.

### The Chandy-Lamport Paper

In 1985, K. Mani Chandy and Leslie Lamport published a paper that we've already looked at in [Lecture 8](./Lecture%208.md) called ["Distributed Snapshots: Determining Global States in a Distributed System"](./papers/chandy.pdf).

There is a really nice quote in the introduction that helps summarise what they are trying to achieve. They describe their algorithm as a *state-detection* algorithm that allows them to understand the global state of a distributed system:

> The state-detection algorithm plays the role of a group of photographers observing a panoramic, dynamic scene, such as a sky filled with migrating birds-
a scene so vast that it cannot be captured by a single photograph. The photographers must take several snapshots and piece the snapshots together to form a picture of the overall scene. The snapshots cannot all be taken at precisely the same instant because of synchronization problems. Furthermore, the photographers should not disturb the process that is being photographed; for instance, they cannot get all the birds in the heavens to remain motionless while the photographs are taken. Yet, the composite picture should be meaningful. The problem before us is to define “meaningful” and then to determine how the photographs should be taken.

Using the analogy of photographing a vast number of migrating birds, this paragraph encapsulates several key concepts:

1. The overall view of the system is too big to be captured in a single snapshot event, so multiple snapshots must be taken and pieced together
1. For practical reasons of synchronization, these multiple snapshots cannot all be taken at the precisely the same point in time
1. The act of taking a snapshot must not disturb the running system

## Who Was the First to Come Up with Primary Backup Replication?

### Alsberg and Day

The paper that tends to be cited the most here is called ["A Principle for Resilient Sharing of Distributed Resources"](./papers/Alsberg%20and%20Day.pdf) by Peter Alsberg and John Day, first published in October 1976.  However, the methodology described in the paper does not look very much like what we now call primary backup; nonetheless, Alsberg and Day did produce a working system that operated in the packet switched networks of the day, where data packets sent over the network really could get lost.

When reading these old papers that were written when the nearest thing to the "internet" was [ARPANET](https://en.wikipedia.org/wiki/ARPANET) or [CYCLADES](https://en.wikipedia.org/wiki/CYCLADES), you have to admire the ingenuity of these people and their ability to solve hard problems in what we would now describe as a very hostile environment.  Many (though not all) of the assumptions they made 40+ years ago are still valid today.


### Reliable, Autonomic Distributed Store (RADOS)

This is part of the now Open-Source system called [Ceph](https://en.wikipedia.org/wiki/Ceph_(software)).

Moving closer to home, the 2007 paper called ["RADOS: A Scalable, Reliable Storage Service for Petabyte-scale Storage Clusters"](./papers/rados.pdf) contains a nice diagram that shows a hybrid of Primary Backup Replication and Chain Replication, that they call "splay replication".

![RADOS Paper Figure 2](./img/L23%20Rados%20Fig%202.png)

This has the features of Primary Backup (also known as Primary Copy) in that the writes are received at the primary node and broadcast in parallel to the other replicas.  However, the principles of Chain Replication are now used insomuch as the last replica in the chain is responsible for sending an `ack` back to the client, and all reads are directed to the tail replica.

So, the interesting thing here is that even in 2007, people were still working towards improving strongly consistent replication strategies.

## Consensus

What is interesting about both these papers (and many others not mentioned here) is that anytime someone sets out to talk about replication, they end up needing to talk about consensus.  However, rather than using a general purpose consensus algorithm such as Paxos, they always talk of a consensus algorithm that has been specially tailored for their particular use case.

Paxos, on the other hand, is a general purpose, one-size-fits-all consensus algorithm.  However, the general problem with the one-size-fits-all approach is that everyone ends up wearing size XXXL.  This is the same with Paxos: in order to make it efficient in a replication scenario, you need to implement optimisations such as multi-Paxos.  With the following algorithms however, they simply assume that you want to do replication and provide you with a consensus algorithm already customised for that use-case.

See the ["Vive la Différence"](./papers/Paxos%20vs%20VSR%20vs%20ZAB.pdf) paper for a comparison of these various strategies.  The great thing about this paper is that at the top of page 6, there is a table of equivalent terminology across the different replication protocols.  What this demonstrates is that while different terms are used, the same basic concepts always pop up.

![Equivalent Terminology Across Different Replication Protocols](./img/L23%20Equivalent%20Terms.png)

### The RAFT Paper

The [RAFT paper](./papers/raft.pdf) came out in 2014 and emphasises understandability over Paxos's complexity.  They have a user study in which they compare users' impressions of how easy RAFT is to use compared to Paxos.

This system is very well documented on their website <https://raft.github.io/>

The authors cite that the RAFT consensus algorithm is similar to the earlier consensus protocol called Viewstamped Replication.

### Viewstamped Replication

The [Viewstamped Replication](./papers/VS520Replication.pdf) paper immediately places us in situation where in one breath we are calling it a replication strategy, and then in the next, we are calling it a consensus algorithm.

Aren't these different things?

Well, yes - in a no kind of way.

Many of the replication strategies that we’ve looked can only work because under the surface, they implement a consensus protocol.  So generally speaking, replication needs consensus, and consensus is used primarily to facilitate replication.


### Are Paxos and RAFT So Different?

Very recently in April 2020, a [comparison paper](./papers/Paxos%20vs%20RAFT.pdf) was published by Heidi Howard and Richard Martier in which a simplified version of Paxos was described using the terminology of RAFT.  The paper concludes that Paxos and RAFT contain a lot of similarities, but RAFT has become more popular because it is easier to understand.  For example, RAFT is very easy to implement from its paper, whereas it is very challenging to implement Paxos from its paper.


---

| Previous | Next
|---|---
| [Lecture 22](./Lecture%2022.md) |


---

***Endnotes***

<b id="f1">1</b>  Stop giggling... Just in case your mind has fixated on the [Yiddish meaning](https://en.wikipedia.org/wiki/Schmuck_(pejorative)) of this word, ["Schmuck"](https://dict.leo.org/german-english/Schmuck) is the German word for "jewellery" or "decoration" or "ornament"...

[↩](#a1)

