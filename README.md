# llm-multinews-summarization

This project fine-tunes the pre-trained `facebook/bart-base` model for abstractive summarization on the [Multi-News](https://github.com/Alex-Fabbri/Multi-News) dataset. The entire pipeline—from preprocessing to training and evaluation—is implemented in a single Jupyter notebook.

---

## Project Overview

- **Dataset**: Multi-News (multi-document news summarization)
- **Model**: `facebook/bart-base`
- **Task**: Abstractive Summarization
- **Metrics**: ROUGE, BLEU, BERTScore

---

## Files

| File/Folder                     | Description                       |
| ------------------------------- | --------------------------------- |
| `summarization_multinews.ipynb` | Main notebook containing all code |
| `results/`                      | Stores predictions and reference  |
| `assets/`                       | Sample summary outputs            |
| `config/`                       | Training Configs and Eval Results |
| `requirements.txt`              | Python dependencies               |
| `README.md`                     | This file                         |

---

## Evaluation

The model was evaluated using:
- ROUGE-1, ROUGE-2, ROUGE-L
- BLEU
- BERTScore

You can find the evaluation logic and scores at the end of the notebook.

## Scores 

| Metric    | Score |
| --------- | ----- |
| ROGUE-1   | 44.48 |
| ROGUE-2   | 16.46 |
| ROGUE-L   | 22.89 |
| BLEU      | 22.69 |
| BERTScore | 86.24 |

## Example Output

```
{
        "Predicted Summary": – Taylor Swift may be about to reveal something big and \"Swifties\" may be the latest victim of hacking, CNN reports. The pop star has wiped out her internet presence—her Instagram, Twitter, Tumblr, YouTube, and website have gone black. The purge arrives on the three-year anniversary of the premiere of \"Shake It Off,\" which served as the chart-topping lead single to Swift's last album, 1989. Coincidence? Possibly. A rep for Swift did not immediately respond to CNN's request for comment. The dramatic move sent fans into a frenzy on social media, using the trending topic \"#TS6IsComing\" to announce their anticipation for Swift's sixth studio album. \"Taylor: *does something for just an hour*#TS6isComing,\" tweeted one user.",

        "Actual Summary": "– Three years after dropping her Grammy-winning album 1989, speculation over when fans will get a new record from Taylor Swift has reached a fever pitch. According to Pitchfork, the pop star mysteriously blacked out her online presence—all photos and posts on Swift’s Instagram, Twitter, and Facebook accounts have been removed, leaving her profiles completely blank. Meanwhile, visitors to the musician’s official site will find a blank, black screen. Per CNN, the “purge” arrived three years to the date of the release of her chart-topping hit, Shake It Off. The move also comes ahead of the MTV Video Music Awards (airing August 27), where Swift is rumored to make an appearance and squash her beef with host Katy Perry. (Swift recently made headlines after winning a groping case against a former DJ.)"
}
```