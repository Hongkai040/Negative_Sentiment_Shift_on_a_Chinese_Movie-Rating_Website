# Negative Sentiment Shift on a Chinese  Movie-rating Website

### Abstract:

Shifting to negativity is more and more prevalent in online communities and may play a key role in group polarization. While current research indicates a close relationship between group polarization and negative sentiment, they often link negative sentiment shifts with echo chambers and misinformation within echo chambers. In this work, we explore the sentiment drift using over 4 million comments from a Chinese online movie-rating community that is less affected by misinformation than other mainstream online communities and has no echo chamber structures. We measure the sentiment shift of the community and users of different engagement levels. Our analysis reveals that while the community doesn’t show a tendency toward negativity, users of higher engagement levels are generally more negative, considering factors like the different movies they consume. The results indicate a fitting-in process, suggesting the possible mechanism of group identity on sentiment shift on social media platforms. These findings also provide guidance on web design to tackle the negativity issue and expand sentiment shift analysis to non-English contexts.

### Data:

The whole dataset is over 800MB(over 4 million comments), making it unsuitable for storing on Github. So here a sample of 5000 movie comments is uploaded). The data used for fine-tuning BERT is also included. 

**Link to scraping program and full-size dataset**:https://github.com/csuldw/AntSpider

### Code:

**Sentiment_analysis**: `Analyze_comments.ipynb`

The sentiment-based analysis could be run locally. The code is written in python 3.8.5. and all of its dependencies can be installed by running the following in the terminal (with the `requirements_analysis.txt` file included in this repository):

```
pip install -r requirements_analysis.txt
```



**Fine-tuning BERT and getting sentiment labels**:`Fine_tune_BERT.ipynb`

The code run on Colab is written in python 3.8.5.  All of its dependencies can be installed by running the following in the terminal (with the `requirements_fine_tuning.txt` file included in this repository):

```
pip install -r requirements_fine_tuning.txt
```



Then you can download all the datasets and replace the directories specified in the code with your own directories, and run all the cell in sequence to reproduce all the results. Noting that data set contains over 4 million comments, getting labels and analyze may take over 100 hours. Future code may parallelize the computing process. 

The model is availale at: https://drive.google.com/drive/folders/1ohCavBYxXE3iapZduPAocLGTqY_rnE6d?usp=sharing



### How to cite:

```
@software{Hongkai040,
  author       = {Hongkai Mao},
  title        = {Negative Sentiment Shift on a Chinese  Movie-rating Website},
  month        = July,
  year         = 2023,
  publisher    = {Github},
  journal      = {Github repository},
  howpublished = {\url{https://github.com/Hongkai040/Negative_Sentiment_Shift_in_Online_Community}},
  commit       = {}
}
```
