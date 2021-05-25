# Adv-OLM: Generating Textual Adversaries via OLM
This repository will contain the code for our EACL 2021 paper:<br><br>
Adv-OLM: Generating Textual Adversaries via OLM <a href="https://www.aclweb.org/anthology/2021.eacl-main.71.pdf"> [Link to Paper]</a>

### Environment setup
- For running in your system:
```bash
conda create -n advolm python=3.6
conda activate advolm
pip install -r requirements.txt
```
- For running on colab:
```bash
pip install -r requirements.txt
```

### Example code run
```bash
python attack_main.py --recipe advolm --batch-size 8 --num-examples 5 --model bert-base-uncased-imdb
```
- For running other attacks like Textfooler, Bae, Pwws, etc., use [TextAttack](https://github.com/QData/TextAttack) 

### Citation
```cite
@inproceedings{malik-etal-2021-adv,
    title = "Adv-{OLM}: Generating Textual Adversaries via {OLM}",
    author = "Malik, Vijit  and
      Bhat, Ashwani  and
      Modi, Ashutosh",
    booktitle = "Proceedings of the 16th Conference of the European Chapter of the Association for Computational Linguistics: Main Volume",
    month = apr,
    year = "2021",
    address = "Online",
    publisher = "Association for Computational Linguistics",
    url = "https://www.aclweb.org/anthology/2021.eacl-main.71",
    pages = "841--849",
    abstract = "Deep learning models are susceptible to adversarial examples that have imperceptible perturbations in the original input, resulting in adversarial attacks against these models. Analysis of these attacks on the state of the art transformers in NLP can help improve the robustness of these models against such adversarial inputs. In this paper, we present Adv-OLM, a black-box attack method that adapts the idea of Occlusion and Language Models (OLM) to the current state of the art attack methods. OLM is used to rank words of a sentence, which are later substituted using word replacement strategies. We experimentally show that our approach outperforms other attack methods for several text classification tasks.",
}
```
