# Large language models in biomedical natural language processing: benchmarks, baselines, and recommendations
This repository provides datasets, baselines, and results for the paper titled 'Large language models in biomedical natural language processing: benchmarks, baselines, and recommendations'. The following provides the basis and we will actively update the repository.

## Datasets
The datasets are biomedical natural language processing (BioNLP) benchmarks commonly adopted for benchmarking BioNLP lanuage models. It consists of the following:
1. The sampled testset: under each dataset, there is a sample file consists of 200 samples from the testing set. This is used to evaluate the accuracy of BioNLP language models in this study. For instance, [the HoC sampled file](https://github.com/qingyu-qc/gpt_bionlp_benchmark/blob/main/Data_Results/Hoc/datasets/hoc-sample200.tsv) provides the 200 samples from the HoC dataset.
2. The original full dataset: the original complete train, dev, test sets under the full_set folder prepared by the existing studies.
   1. The train and dev files are used to train a PubMedBERT model as a baseline
   2. The train file was used to randomly select samples for one-shot learning

## Prompts
A prompt file is also provided under each dataset.

## Results
The zero-shot and one-shot learning results are provided under each dataset.

## NCBI's Disclaimer
This tool shows the results of research conducted in the [Computational Biology Branch](https://www.ncbi.nlm.nih.gov/research/), [NCBI](https://www.ncbi.nlm.nih.gov/home/about). 

The information produced on this website is not intended for direct diagnostic use or medical decision-making without review and oversight by a clinical professional. Individuals should not change their health behavior solely on the basis of information produced on this website. NIH does not independently verify the validity or utility of the information produced by this tool. If you have questions about the information produced on this website, please see a health care professional. 

More information about [NCBI's disclaimer policy](https://www.ncbi.nlm.nih.gov/home/about/policies.shtml) is available.

## Acknowledgment 
This study is supported by the following National Institutes of Health grants: R01AG078154, 1K99LM01402, and the Intramural Research Program of the National Library of Medicine (NLM).
