# Readme

This repository contains the datives corpus introduced in:

Goodwin, E., Levin, B., & Morgan, E. (2025). Syntactic Choice Is Shaped by Fine-Grained, Item-Specific Knowledge. Proceedings of the Annual Meeting of the Cognitive Science Society, 47.

To reproduce the plots and analyses in the paper, see the [code repository](https://github.com/emilygoodwin/dativeCorpusAnalyses).

**Note**:

A central goal of this corpus was to investigate the distribution of "dative" and "nondative" uses of dative verbs. Non-dative examples include spatial goals, like the one in (2):

(1) *Throw the ball to the girl/ throw the girl the ball* (Dative Use)

(2) *Throw the ball to the ground/ \*Throw the ground the ball.* (Nondative Use)

**The distribution of dative and non-dative uses in the corpus is not representative of their true distribution in the larger text that we sampled from**. This is because we sampled and annotated more examples of verbs that had lower relative rates of dative uses: to get enough 'true datives' of these verbs, we had to sample more instances of them, and thus they are overrepresented in the corpus. Also, for *take,* which is extremely frequent and has many non-dative senses, we found that we had to automatically filtered the most common non-dative senses (e.g. *take the bus/train/taxi to somewhere*) before annotating.

Thus, **if you want an estimate of a verbs' frequency** (in a dative or non-dative structure) **please use the** `gold_structural_preferences` **dataframe**, rather than calculating directly from the corpus.

## Naming convention in Structure Preferences Dataframe:

**Surface metrics**: means the metric is calculated over things with dative surface syntax, but not necessarily dative semantics (Stanza parsed it into a V NP NP or V NP to-PP, but it could have been for example a spatial goal like "throw the glass to the floor").

**Imputed dative metrics**: are estimated metrics for the datives-only, based on the dative yield we had after sampling and annotating for dative status.

**Nondative DO skew**: Of the examples which were judged nondative, the proportion that had the V NP NP syntax

**Frequency**: is the instances per billion words

**Projected instances by college age**: We multiply the estimated frequency per billion words by \*.35, which assumes that by roughly age 20 speakers have heard roughly 350 million words. This is the more generous estimate used in Levy et al., 2012 (see footnote 9):

Levy, R., Fedorenko, E., Breen, M., & Gibson, E. (2012). The processing of extraposed structures in English. *Cognition*, *122*(1), 12–36. <https://doi.org/10.1016/j.cognition.2011.07.012>

The CSV is the same data as the RDS file- I just added this for convenience.
