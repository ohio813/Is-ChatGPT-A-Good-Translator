# Is ChatGPT A Good Translator? A Preliminary Study

A preliminary evaluation of ChatGPT for machine translation. [[V1]](https://wxjiao.github.io/downloads/tech_chatgpt_arxiv.pdf)  [[V2-arXiv]](https://arxiv.org/abs/2301.08745)

We should admit that the report is far from complete with various aspects to make it more reliable in the future:
- **Coverage of Test Data**: Currently, we randomly select 50 samples from each test set for evaluation due to the response delay of ChatGPT. Automating the testing pipeline or upgrading the ChatGPT version may help. 
- **Translation Abilities**: We only focus on multilingual translation and translation robustness in this report. But there are some other translation abilities to be evaluated, e.g., constrained machine translation and document-level machine translation.


## Test Data
Please kindly cite the papers of the data sources if you use any of them.
- **Flores**: The FLORES-101  Evaluation Benchmark for Low-Resource and Multilingual Machine Translation
- **WMT19 Biomedical**: Findings of the WMT 2019 Biomedical Translation Shared Task: Evaluation for Medline Abstracts and Biomedical Terminologies
- **WMT20 Robustness**: Findings of the WMT 2020 Shared Task on Machine Translation Robustness


## Translation Prompt

<div align="center">
    <img width="70%" alt="Templates-by-ChatGPT" src="https://user-images.githubusercontent.com/31032829/213847658-fc977b1f-2ebd-4f2e-91b0-8df337d0a27e.png">
    <p class="image-caption">Figure 1: Prompts advised by ChatGPT for machine translation (Date: 2022.12.16).</p>
</div>

Summarized prompts:
- Tp1: `Translate these sentences from [SRC] to [TGT]:`
- Tp2: `Answer with no quotes. What do these sentences mean in [TGT]?`
- Tp3: `Please provide the [TGT] translation for these sentences:`

<div align="center">
    <img width="40%" alt="image" src="https://user-images.githubusercontent.com/31032829/213848303-4aa969c5-61d7-4dc8-b675-5a539657db67.png">
    <p class="image-caption">Table 1: Comparison of different prompts for ChatGPT to perform Chinese-to-English (Zh⇒En) translation.</p>
</div>


## Multilingual Translation

<div align="center">
    <img width="70%" alt="image" src="https://user-images.githubusercontent.com/31032829/213848377-8c4d40d4-04de-4735-87fe-d22fd3f70dd9.png">
    <p class="image-caption">Table 2: Performance of ChatGPT for multilingual translation.</p>
</div>

## Translation Robustness

<div align="center">
    <img width="50%" alt="image" src="https://user-images.githubusercontent.com/31032829/213848428-069891f5-4de0-4922-83f8-2f0c1b163d26.png">
    <p class="image-caption">Table 3: Performance of ChatGPT for translation robustness.</p>
</div>


## Public Impact
### Citation
Please kindly cite our report if you find it helpful:

```ruby
@inproceedings{jiao2023ischatgpt,
  title={Is ChatGPT A Good Translator? A Preliminary Study},
  author={Wenxiang Jiao and Wenxuan Wang and Jen-tse Huang and Xing Wang and Zhaopeng Tu},
  booktitle = {ArXiv},
  year      = {2023}
}
```
