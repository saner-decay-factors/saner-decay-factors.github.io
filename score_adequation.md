[Back](https://saner-decay-factors.github.io/)

# Additional Analysis - Score Adequation

We executed an additional analysis, in order to observe whether the method used to calculate the decay score was adequate for our context, which is to improve maintainability. As such, we investigate instances of refactoring that might represent an attempt by the developer to remove or mitigate design problems, thus improving design quality and, consequently, maintainability. We computed the frequency in which each type of refactoring considered in this work modified the four IQAs considered when calculating decay score. Moreover, the following table displays the results from this analysis.

|    Project   | Refactoring Type | Cohesion | Coupling | Complexity | Inheritance | Total #
|-|-|-|-|-|-|-|
| dubbo        | Extraction       | 24% | 37% | 34% | 5% | 1719
|              | Move             | 26% | 35% | 33% | 5% | 1173
|              | Rename           | 25% | 36% | 35% | 4% | 588
|              | Hierarchical     | 24% | 40% | 27% | 8% | 62
| fresco       | Extraction       | 25% | 31% | 41% | 3% | 1830
|              | Move             | 25% | 36% | 37% | 2% | 806
|              | Rename           | 30% | 32% | 36% | 2% | 543
|              | Hierarchical     | 20% | 33% | 38% | 9% | 66
| RxJava       | Extraction       | 11% | 57% | 14% | 18% | 122
|              | Move             | 0% | 0% | 0% | 0% | 0
|              | Rename           | 26% | 33% | 28% | 14% | 58
|              | Hierarchical     | 0% | 0% | 0% | 0% | 0
| netty        | Extraction       | 24% | 41% | 30% | 5% | 7141
|              | Move             | 25% | 40% | 28% | 7% | 13017
|              | Rename           | 25% | 40% | 31% | 5% | 1865
|              | Hierarchical     | 25% | 40% | 29% | 6% | 166
| presto       | Extraction       | 23% | 44% | 31% | 2% | 17572
|              | Move             | 25% | 44% | 30% | 1% | 19786
|              | Rename           | 22% | 42% | 33% | 3% | 7922
|              | Hierarchical     | 22% | 41% | 35% | 3% | 666
| okhttp       | Extraction       | 27% | 34% | 38% | 1% | 1741
|              | Move             | 25% | 37% | 37% | 1% | 1741
|              | Rename           | 27% | 34% | 38% | 1% | 606
|              | Hierarchical     | 0% | 0% | 0% | 0% | 0
| All Projects | Extraction       | 24% | 41% | 32% | 3% | 30125
|              | Move             | 25% | 41% | 30% | 3% | 37424
|              | Rename           | 23% | 40% | 33% | 3% | 11582
|              | Hierarchical     | 23% | 40% | 33% | 4% | 960

Overall, all refactoring types consistently changed the four IQAs, albeit at different frequencies. While changes to cohesion, coupling, and complexity were more common (23\% to 41\% of instances), inheritance stood out as it was only changes in 3\% to 4\% of instances.

Since each attribute contributes to 25\% of the decay score computation, this result is a possible explanation for why classes with decay score bigger than 0.8 are very infrequent (see [Additional Analysis - Score Distribution](https://saner-decay-factors.github.io/visualization_score.html)).

This result is in line with the rationale behind the decay score and with previous results that investigated the relationship between IQAs and co-occurrences of code smells [1].

[1] J. Martins, C. Bezerra, A. Uchôa, and A. Garcia, “How do code smell co-occurrences removal impact internal quality attributes? a developers’ perspective,” in 35th SBES, 2021.