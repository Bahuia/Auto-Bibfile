# Auto-Bibfile
Auto-Bibfile is an automatic toolkit for README.md generation based on bibtex file.

This repository is maintained by [Tongtong Wu](https://wutong8023.site). Please don't hesitate to collaborate or fix some entries. The automation script of this repo is partially adapted from [Automatic_Awesome_Bibliography](https://github.com/TLESORT/Automatic_Awesome_Bibliography).

## Quick Start
- Install: 
```pip install bibtexparser```

- Run: 
```python scripts/bibtex_to_md.py```

- Add a new paper: 
paste a bib entry to [bibtex.bib](https://github.com/wutong8023/Auto-Bibfile/blob/master/bibtex.bib).

- Categorize:
Add ```keywords``` to each entry and write down your note within ```@String()```. For example,

```latex
@inproceedings{WuLLHQZX21,
    author = {Tongtong Wu and
        Xuekai Li and
        Yuan{-}Fang Li and
        Gholamreza Haffari and
        Guilin Qi and
        Yujin Zhu and
        Guoqiang Xu},
    title = {Curriculum-Meta Learning for Order-Robust Continual Relation Extraction},
    booktitle = {Proceedings of AAAI},
    pages = {10363--10369},
    year = {2021},
    url = {https://ojs.aaai.org/index.php/AAAI/article/view/17241},
    keywords = {
        New Method,
        NLP,
        Supervised Learning,
        Event Extraction,
        Rehearsal, Meta-learning,
        w/ External Knowledge,
        Class Incremental,
        Catastrophic Forgetting, Order Sensitivity,
        RNNs,
        Fewrel, SimpleQuestion, Tacred,
        Accuracy
    },
}
@String(WuLLHQZX21="Add a brief note behind the bib entry")
```




Click [here](https://github.com/wutong8023/Auto-Bibfile/tree/master/your_topic4all) for an exemplar.

## Instruction
1. check [bibtex.bib](https://github.com/wutong8023/Auto-Bibfile/blob/master/bibtex.bib): Auto-Bibfile will parse the keywords and meta-info of each entry.
2. the keywords should be predefined in [scripts/bibtext_to_md.py # fined_taxonomy](https://github.com/wutong8023/Auto-Bibfile/tree/master/scripts/bibtex_to_md.py#L84-L137).
3. check ```TODOs``` in [scripts/bibtext_to_md.py](https://github.com/wutong8023/Auto-Bibfile/blob/master/scripts/bibtex_to_md.py) and [scripts/utils.py](https://github.com/wutong8023/Auto-Bibfile/blob/master/scripts/utils.py) for customization.

## How to Contribute
Please feel free to use and share [Auto-Bibfile](https://github.com/wutong8023/Auto-Bibfile.git). It would be great 
if you mention it in your own repository by adding:
> The automation script of this repo is <br> powered by \[Auto-Bibfile\](https://github.com/wutong8023/Auto-Bibfile.git).
