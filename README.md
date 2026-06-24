# BA2-Digital-Korea-final-paper-Breukers

final paper data

Project description

This project applies computational text analysis to a corpus of 615 poems written by five Korean poets who lived during the Japanese colonial period: 한용운, 김소월, 임화, 이상, and 윤동주. The study combines sentiment analysis and document embedding techniques to investigate both emotional expression and semantic similarity within the corpus. Specifically, it examines whether poets differ in their use of positive and negative language and whether poems by the same poet form distinct semantic clusters when represented using contextual document embeddings.

Sentiment scores were generated using the KNU Sentiment Dictionary, allowing comparisons of emotional tone across poets. To explore semantic relationships between poems, Q-BERT document embeddings were created from the original texts. The corpus was preprocessed using KiwiPiePy for Korean morphological analysis and tokenization before being integrated with the embedding and sentiment data. K-means clustering was then applied to identify groups of similar poems, and t-distributed Stochastic Neighbour Embedding (t-SNE) was used to visualize relationships between poems in a reduced two-dimensional space.

The project evaluates the extent to which emotional expression and semantic organization correspond to individual authorship versus broader historical and thematic influences. Because all five poets wrote during the colonial period, the corpus provides an opportunity to examine how shared historical experiences interact with distinctive authorial styles.

Reseach Question

Which poets exhibit the most positive and most negative affect according to the KNU Sentiment Dictionary, and do poems by the same poet cluster together when represented using document embeddings?

Headline Finding

The analysis found meaningful differences in sentiment between poets. Earlier-born poets, particularly 한용운, tended to receive more positive sentiment scores, whereas later-born poets such as 이상 and 윤동주 exhibited more negative average sentiment. This pattern suggests a possible generational shift in emotional expression during the colonial period.

However, the clustering analysis revealed substantial overlap between poets. Rather than forming clearly separated author-based groups, most semantic clusters contained poems from multiple authors. This indicates that shared historical experiences and thematic concerns—including identity, loss, nature, and personal reflection—played a significant role in shaping the corpus. While some evidence of author-specific patterns remained visible, thematic similarity appeared to be a stronger organizing force than authorship alone.

Overall, the results suggest that colonial-era Korean poetry contains both distinctive emotional tendencies across poets and substantial thematic commonality across authors.

Instructions to reproduce

Software Requirements
Orange Data Mining
Orange Text Mining Add-on
KiwiPiePy (if preprocessing outside Orange)
Corpus dataset containing 615 poems

Workflow
1. Load the Korean poetry corpus (615 poems) into the Orange Corpus widget.
2. Preprocess the texts using KiwiPiePy morphological analysis to tokenize the poems and prepare them for computational analysis.
3. Generate sentiment scores using the Sentiment Analysis widget with the KNU Sentiment Dictionary.
4. Create contextual document representations using the Q-BERT Embedding widget.
5. Merge the embedding vectors, sentiment scores, and metadata into a combined dataset.
6. Apply K-means Clustering to identify groups of semantically similar poems.
7. Visualize the resulting clusters using t-SNE.
8. Explore cluster composition and poet distributions using:
-t-SNE visualization
-Corpus Viewer
-Data Table
-Distance Map / Hierarchical Clustering (optional)
9. Compare:
-Sentiment distributions across poets
-Cluster membership by poet
-Relationships between sentiment scores and cluster structure
10.Interpret whether observed patterns reflect individual authorship, shared themes, or broader historical influences associated with the Japanese colonial period.
