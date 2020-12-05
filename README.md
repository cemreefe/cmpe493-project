# CMPE 493 Information Retrieval Term Project

In this project, you will work on information retrieval from the Covid-19 related scientific literature. This task has been recently addressed in the [TREC-COVID Challange](https://ir.nist.gov/covidSubmit/).

![clippy](https://i.gifer.com/origin/c6/c6afab251a20e6d0eb80b983450bc66e_w200.gif)

### Dataset

1. [Documents](https://ir.nist.gov/covidSubmit/data.html)

   3.7 GB

   You will use the odd numbered topics (i.e., 1, 3, 5, 7,..., 49) for developing your systems and the even numbered topics (i.e., 2, 4, 6, 8,...,50) for evaluation.

   ```
   curl https://ai2-semanticscholar-cord-19.s3-us-west-2.amazonaws.com/historical_releases/cord-19_2020-07-16.tar.gz --output data/cord-19_2020-07-16.tar.gz
   ```

2. [Topics](./data/topics-rnd5.xml)

   in the data folder

3. [Relevance Judgements](./data/qrels-covid_d5_j0.5-5.txt)

   in the data folder

   | **topic-id** | iteration* | **document-id** | **relevance-judgement**** |
   | ------------ | ---------- | --------------- | ------------------------- |
   | 1            | 4.5        | 005b2j4b        | 2                         |

   \*: won't be used

   \**: relevance judgement values

   0. not relevant

   1. partially relevant

   2. fully relevant



### Evaluation Metric

See the [official evaluation tool](https://github.com/usnistgov/trec_eval).

* `MAP` (Mean Average Precision)
* `NDCG` (Normalized Discounted Cumulative Gain)
* `P@10` (Precision of Top 10 Results)



### Deliverables: 

1. Project progress presentation (December 28, 2020 (in the lecture hour); 30% of your project score): You should prepare a 10 min. presentation describing what you have done so far and what your plan is for the remaining time period. You should have completed at least the preprocessing of the data set and implemented and tested a baseline approach (such as `TFIDF` based cosine similarity). You should also have clear plans about how you will improve your system by the end of the semester. 
2. Project final presentation (On the final exam date/slot; 70% of your project score): You should prepare a 10 min. presentation describing your final system and your results. I also suggest you to include an error analysis.
3. Prior to each presentation (latest 1 hour before the presentations start) you should send me by email your slides and all source code and accompanying `readme` documents. 



### Honor Code

You should work in teams of two or three people. Each team member should contribute equally to the development of the project and to the presentations. All team members will get the same score. You are allowed to use external libraries/resources for the project. **However, you SHOULD properly acknowledge and cite these in your presentations and source code**. Late Submission: Late submissions are NOT allowed.



### Relevant Work

See papers suggested by Arzucan Özgür [here](https://ir.nist.gov/covidSubmit/bib.html).



