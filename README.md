# The Best of BERT Worlds: Improving minBERT with multi-task extensions

This paper aims to enhance BERT’s performance across various NLP tasks, including sentiment analysis, paraphrase detection and semantic textual similarity, amongst others by leveraging the SBERT architecture as proposed by Reimers and Gurevych (2019). It thereby demonstrates SBERT’s utility in generating sentence embeddings for a broader range of tasks.

<p align="center">
  <img width="229" alt="image" src="https://github.com/julezzhub/multitaskBERT/assets/55262654/7b2636e6-7877-42ba-afb1-7007ec9ceeea"><br>
  <i>Architecture for STS prediction, adapted from Reimers and Gurevych (2019)</i>
</p>





Through a combination of experiments, I manage to significantly improve BERT’s scores on the three tasks and enable it to effectively multitask. These improvements are mainly driven by (a) cosine-similarity fine tuning, (b) using a mean-pooling strategy to generate sentence embeddings, (c) concatenating embeddings for para- phrase detection, and (d) summing individual losses for multi-task learning (Bi et al., 2022). I find that these adjustments prove to be particularly effective for paraphrase detection and semantic textual similarity, while doing little to improve sentiment analysis.
