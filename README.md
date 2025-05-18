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
