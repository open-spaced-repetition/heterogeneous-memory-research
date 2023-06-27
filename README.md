# Introduction

I have many ideas and hypotheses about the memory model in the spaced repetition. This repository is a public record for my thoughts, which are still rough drafts. Maybe I will enrich them in the future.

Here are some key points that I want to drive into.

## Heterogeneity

- A person can only memorize a card once at a given time, making multiple memorizations under identical conditions impossible. This irreproducibility makes accurate memory state measurement unachievable.
- If we disregard the difference in card content and treat cards with similar review histories as one entity, the stability and difficulty we measure only represents an average, not addressing the issue of heterogeneity.
- Due to data heterogeneity, any memory model trained on review logs essentially estimates the mean memory states (stability, difficulty, and more). The laws governing changes in the mean may not necessarily apply to individual memory changes. Changes in distribution may be the primary factor behind mean variations.

The good news is that stability tends to converge under the same review history, and each recall score effectively segregates heterogeneous memories, thereby possibly reducing long-term memory heterogeneity significantly.