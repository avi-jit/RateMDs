# TL;DR
This repository contains data and scripts pertaining to work done by [Avijit Thawani](https://sites.google.com/view/avijit-thawani/home) while at Northeastern University (summer 2018) under the guidance of [Dr. Byron C. Wallace](http://www.byronwallace.com/) (College of Computer and Information Science, Northeastern University, Boston, MA).


# [Link to paper](https://www.mlforhc.org/s/Thawani.pdf) 
```
Thawani A. Paul M J. Sarkar U. Wallace B C. 
Are Online Reviews of Physicians Biased Against Female Providers? 
In Proceedings of Machine Learning Research. 106:1-17, 2019.
```

The paper was presented at MLHC 2019 ([Machine Learning for Healthcare](https://www.mlforhc.org)) Conference, Ann Arbor, Michigan. Here's a [poster](https://github.com/avi-jit/RateMDs/blob/master/poster3.pdf) summarizing our work, [slides](https://github.com/avi-jit/RateMDs/blob/master/3_72.pdf) from the talk and a [video presentation](https://github.com/avi-jit/RateMDs/blob/master/livestream.mp4) for the same.

Please cite us and mail me at [thawani@usc.edu](mailto:thawani@usc.edu) for feedback, errors, ideas for future work, or just to say Hi!

# [Google Colab code](https://colab.research.google.com/drive/1SAI9Mukbm3_CpsX94ODXCTSv5l-C_wzx#scrollTo=fmbi9OQjeqDw)
The easiest way to explore our project, without installing or downloading anything. Just copy our `RateMDs/` folder from [Google Drive](https://drive.google.com/drive/folders/1sX_Z02psZcFdZe4yqH5NxxiQ2mKKsEXZ?usp=sharing) link and give its access to this Google Colab Notebook.

# [Data on Google Drive](https://drive.google.com/drive/folders/1sX_Z02psZcFdZe4yqH5NxxiQ2mKKsEXZ?usp=sharing)
1. `processed_1.csv*`: clean data containing 37646 reviews and ratings along with `specialty` and `gender`.
2. `ratemds.model`: Pretrained word embedding (gensim) model. Scripts to play are in the `scripts/` folder as well as on [Google Colab](https://colab.research.google.com/drive/1SAI9Mukbm3_CpsX94ODXCTSv5l-C_wzx#scrollTo=fmbi9OQjeqDw).

# This Repository
1. `raw data`: parsed HTML files from [RateMDs.com](http://ratemds.com)
2. `unclean.csv`: id, review, physician specialty, physician gender, physician name, document label
3. `processed_1.csv`: review id, physician id, physician specialty, physician gender, rating staff, rating punctuality, rating helpfulness, rating knowledgeability, review text (tokenized)
4. `all_Github.csv`: physician_id.review_id, physician_id, physician name, physician specialty, physician gender, rating staff, rating punctuality, rating helpfulness, rating knowledgeability, review text
5. `scripts`: Jupyter Notebooks to reproduce our results (corresponding section from the [paper]((https://www.mlforhc.org/s/Thawani.pdf) ) in parantheses): 
- `clean.ipynb`: Data preprocessing (Section 2.1)
- `regression.ipynb`: Rating Analysis (Section 2.2)
- `LR.ipynb`: Lexical Regression (Section 2.3.1) 
- `match.ipynb`: Embeddings (Section 2.3.2)

# Contributors
Avijit Thawani, University of Southern California (work done when interning at Northeastern in Summer 2018). <br>
Michael J. Paul, University of Colorado Boulder. <br>
Urmimala Sarkar, University of California San Francisco. <br>
Byron C. Wallace, Northeastern University.
