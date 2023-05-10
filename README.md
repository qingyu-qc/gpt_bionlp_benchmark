# Large language models in biomedical natural language processing: benchmarks, baselines, and recommendations
This repository provides datasets, baselines, and results for the paper titled 'Large language models in biomedical natural language processing: benchmarks, baselines, and recommendations'. The following provides the basis and we will actively update the repository.

## Benchmarks
The datasets are biomedical natural language processing (BioNLP) benchmarks commonly adopted for benchmarking BioNLP lanuage models. It consists of the following:
1. The sampled testset: under each dataset, there is a sample file consists of 200 samples from the testing set. This is used to evaluate the accuracy of BioNLP language models in this study. For instance, [the HoC sampled file](https://github.com/qingyu-qc/gpt_bionlp_benchmark/blob/main/Benchmarks/Hoc/datasets/hoc-sample200.tsv) provides the 200 samples from the HoC dataset.
2. The original full dataset: the original complete train, dev, test sets under the full_set folder prepared by the existing studies.
   1. The train and dev files are used to fine-tune a PubMedBERT model as a baseline
   2. The train file was used to randomly select samples for one-shot learning

## Prompts
A prompt sample is also provided under each benchmark.

## Results
| Sampled dataset | Evaluation metric | Fine-tuned PubMedBERT (min-max) | Zero-shot GPT-3 |One-shot GPT-3 |Zero-shot GPT-4 |One-shot GPT-4 |
| :------ | --------: | --------: | -----: |-----: |-----: |-----: |
| BC5CDR-chemical | Entity-level F1 |0.9028-0.9350|0.2925|0.1803|0.7443|0.8207
| NCBI-disease | Entity-level F1 |0.8336-0.8986|0.2405|0.1273|0.5673|0.4837
| ChemProt | Macro F1|0.6653-0.7832|0.5743|0.6191|0.6618|0.6543
| DDI2013 | Macro F1|0.6673-0.8023|0.3349|0.3440|0.6325|0.6558
| HoC | Label-wise macro F1|0.6991-0.8915|0.6572|0.6932|0.7474|0.7402
|LitCovid| Label-wise macro F1|0.8024-0.8724|0.6390|0.6531|0.6746|0.6839
|PubMedQA|Pearson correlation|0.2237-0.3676|0.3553|0.3011|0.4374|0.5361
|BIOSSES|Macro F1|0.6870-0.9332|0.8786|0.9194|0.8832|0.8922

## NCBI's Disclaimer
This tool shows the results of research conducted in the [Computational Biology Branch](https://www.ncbi.nlm.nih.gov/research/), [NCBI](https://www.ncbi.nlm.nih.gov/home/about). 

The information produced on this website is not intended for direct diagnostic use or medical decision-making without review and oversight by a clinical professional. Individuals should not change their health behavior solely on the basis of information produced on this website. NIH does not independently verify the validity or utility of the information produced by this tool. If you have questions about the information produced on this website, please see a health care professional. 

More information about [NCBI's disclaimer policy](https://www.ncbi.nlm.nih.gov/home/about/policies.shtml) is available.

## Acknowledgment 
This study is supported by the following National Institutes of Health grants: R01AG078154, 1K99LM01402, and the Intramural Research Program of the National Library of Medicine (NLM).
