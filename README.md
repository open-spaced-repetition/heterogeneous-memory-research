# Introduction

I have many ideas and hypotheses about the memory model in the spaced repetition. This repository is a public record for my thoughts, which are still rough drafts. Maybe I will enrich them in the future.

Here are some key points that I want to drive into.

## Heterogeneity

- A person can only memorize a card once at a given time, making multiple memorizations under identical conditions impossible. This irreproducibility makes accurate memory state measurement unachievable.
- If we disregard the difference in card content and treat cards with similar review histories as one entity, the stability and difficulty we measure only represents an average of the group, not addressing the issue of heterogeneity.
- Due to data heterogeneity, any memory model trained on review logs essentially estimates the mean memory states (stability, difficulty, and more). The laws governing changes in the mean may not necessarily apply to individual memory changes. Changes in distribution may be the primary factor behind mean transformations.

The good news is that stability tends to converge under the same review history, and each rating effectively filters heterogeneous memories, thereby possibly reducing long-term memory heterogeneity.

## Everything is a distribution

The stability of a group is a distribution, so the forgetting curve is an average of multiple exponential fucntion, whose shape is more similar to power function.

The difficulty of a group is a distribution, and the difficult cards are more likely to forget, so the average difficulty of forgotten cards are higher.

The rating of a group is a distribution. The higher the retrievability, the greater the rating. However, according to the poor metamemory judgement of human, the relation is not very strong.

## Expected failures & Ease hell

[Simple spaced repetition algorithms mistreat expected failures (andymatuschak.org)](https://notes.andymatuschak.org/zPFEkvYDUnJzewccCQs4z6fULuozcMyHZnc)

[Ease Hell in Anki | Broca (readbroca.com)](https://readbroca.com/anki/ease-hell/)

To be continued.