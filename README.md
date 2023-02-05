# APEACH - Korean Hate Speech Evaluation Datasets

**APEACH** is the first crowd-generated Korean evaluation dataset for hate speech detection. Sentences of the dataset are created by anonymous participants using an online crowdsourcing platform [DeepNatural AI](https://www.deepnatural.ai/).

* Sample Code : <a href="https://colab.research.google.com/drive/1djd0fuoMYIaf7VCHaLQIziJi4_yBJruP#scrollTo=VPR24ysr5Q7k"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="base"/></a>

## Download

You can download benchmark set **APEACH**.  `APEACH/test.csv`  in this repository.

## Dataset Description

- APEACH : A hate-speech evaluation dataset generated in 2021, using generation method followd by APEACH paper.

### Guidelines

[APEACH-GUIDELINE](https://docs.google.com/document/d/1XqJ5E-OXK3ULX9WCbc10Bj0k9vTfJqQ6E7D2QHP9DWU/edit?usp=drivesdk)

### Topics

![](resource/dist_topics.png)

### Lengths

![](resource/dist_lengths.png)

## Paper
- https://aclanthology.org/2022.findings-emnlp.525/

## Experiment Code
<a href="https://colab.research.google.com/drive/1djd0fuoMYIaf7VCHaLQIziJi4_yBJruP#scrollTo=VPR24ysr5Q7k"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="base"/></a>

## Experiment Results

| Name               | Beep! Dev Dataset | Apeach (Ours) |
| ------------------ | ----------------- | ------------------ |
| SoongsilBERT-Base | 0.8261 | **0.8424** |
| SoongsilBERT-Small | 0.8149            | 0.8228 |
| KcBERT-base        | 0.8088 | 0.8086 |
| KcBERT-large       | **0.8295** | 0.8116 |
| DistillKoBERT | 0.7570 | 0.7715 |
| KoELECTRA-V3       | 0.7920 | 0.8101 |
| KoBERT             | 0.8030 | 0.7885 |

We also share BEST model of our dataset which we trained in this experiment as checkpoint, [demo webite](https://master-soongsil-bert-base-beep-deploy-jason9693.endpoint.ainize.ai) and [api](https://github.com/jason9693/SoongsilBERT-base-beep-deploy).

## Citation
```
@inproceedings{yang-etal-2022-apeach,
    title = "{APEACH}: Attacking Pejorative Expressions with Analysis on Crowd-Generated Hate Speech Evaluation Datasets",
    author = "Yang, Kichang  and
      Jang, Wonjun  and
      Cho, Won Ik",
    booktitle = "Findings of the Association for Computational Linguistics: EMNLP 2022",
    month = dec,
    year = "2022",
    address = "Abu Dhabi, United Arab Emirates",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2022.findings-emnlp.525",
    pages = "7076--7086",
    abstract = "In hate speech detection, developing training and evaluation datasets across various domains is the critical issue. Whereas, major approaches crawl social media texts and hire crowd-workers to annotate the data. Following this convention often restricts the scope of pejorative expressions to a single domain lacking generalization. Sometimes domain overlap between training corpus and evaluation set overestimate the prediction performance when pretraining language models on low-data language. To alleviate these problems in Korean, we propose APEACH that asks unspecified users to generate hate speech examples followed by minimal post-labeling. We find that APEACH can collect useful datasets that are less sensitive to the lexical overlaps between the pretraining corpus and the evaluation set, thereby properly measuring the model performance.",
}
```

## Contributors

The main contributors of the work ( * : equal contribution) : 

- [Kichang Yang](https://github.com/jason9693)* ([*Kakao Corp.*](https://www.kakaocorp.com/), [*Kakao Enterprise Corp.*](https://www.kakaoenterprise.com/), [*Soongsil University*](https://eng.ssu.ac.kr))
- [Wonjun Jang](https://github.com/strutive07)* ([*Kakao Corp.*](https://www.kakaocorp.com/), [*Soongsil University*](https://eng.ssu.ac.kr))
- [Won Ik Cho](https://github.com/warnikchow)* ([*Seoul National University*](https://en.snu.ac.kr/index.html))

## License

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/).
