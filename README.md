# APEACH - Korean Hate Speech Evaluation Datasets

We provide the first crowd-generated Korean evaluation dataset for hate speech detection.

The sentences of our dataset are created by unspecified workers, moderated by a crowd-sourcing platform [DeepNatural AI](https://www.deepnatural.ai/).

## Download

- APEACH2021 : You can download benchmark set **APEACH2021**.  `APEACH2021/test.csv`  in this repository.

## Dataset Description

- APEACH2021

### Guidelines

[APEACH-GUIDELINE](https://docs.google.com/document/d/1XqJ5E-OXK3ULX9WCbc10Bj0k9vTfJqQ6E7D2QHP9DWU/edit?usp=drivesdk)

### Topics

![](resource/dist_topics.png)

### Lengths

![](resource/dist_lengths.png)

### Demographics

![resource/figure7.png](resource/figure7.png)


## Experiment Results

| Name               | Beep! Dev Dataset | Apeach-2021 (Ours) |
| ------------------ | ----------------- | ------------------ |
| SoongsilBERT-Base | 0.8260774883      | 0.8424406845       |
| SoongsilBERT-Small | 0.8148655904      | 0.8227619749       |
| KcBERT-base        | 0.8087641117      | 0.8086445881       |
| KcBERT-large       | 0.8295103829      | 0.8116314931       |
| KoDistillBERT      | 0.756979624       | 0.7715461816       |
| KoELECTRA-V3       | 0.792013485       | 0.8100758509       |
| KoBERT             | 0.8029963116      | 0.7884561101       |

We also share SOTA model of our dataset which we trained in this experiment as checkpoint, [demo webite](https://master-soongsil-bert-base-beep-deploy-jason9693.endpoint.ainize.ai) and [api](https://github.com/jason9693/SoongsilBERT-base-beep-deploy).



## Contributors

The main contributors of the work (* : equal contribution) : 

- Kichang Yang *([Kakao Enterprise](https://www.kakaoenterprise.com/), [Soongsil University](https://eng.ssu.ac.kr))**
- Wonjun Jang *([Soongsil University](https://eng.ssu.ac.kr))**
- Won Ik Cho *([Seoul National University](https://en.snu.ac.kr/index.html))**

## License

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/).

## Reference