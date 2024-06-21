# UTDRM: Unsupervised Method for Training Debunked-Narrative Retrieval Models

This repository contains the models and code for [UTDRM](https://epjdatascience.springeropen.com/articles/10.1140/epjds/s13688-023-00437-y), an unsupervised method for training debunked-narrative retrieval models. The approach involves generating topical claims using T5 and ChatGPT claim generators and training the dense retrieval model using MNR loss.

## Usage Instructions:

1. **Generate Claims:**
   - Utilize the T5 and ChatGPT claim generators located in the `generators/` directory to generate claims.
   - T5 and ChatGPT generated claims can be downloaded from [Zenodo](https://zenodo.org/records/12167870).

2. **Convert Dataset and Mine Hard Negatives:**
   - Convert the dataset into BIER format and mine hard negatives using the scripts available at [GPL](https://github.com/UKPLab/gpl). This process will generate the `hard-negatives.jsonl` file.

3. **Train the Model:**
   - Find the script for training the dense retrieval model using MNR loss in the `training/` directory.

## Best Performing Models:

The best performing models can be accessed via the following Hugging Face model repositories:

- [UTDRM-MPNet](https://huggingface.co/iknoor/UTDRM-MPNet)
- [UTDRM-RoBERTa](https://huggingface.co/iknoor/UTDRM-RoBERTa)


## Citation:

If you use the code or models from this repository, please consider citing the following paper:

```
@article{singh2023utdrm,
  title={UTDRM: unsupervised method for training debunked-narrative retrieval models},
  author={Singh, Iknoor and Scarton, Carolina and Bontcheva, Kalina},
  journal={EPJ Data Science},
  volume={12},
  number={1},
  pages={59},
  year={2023},
  publisher={Springer}
}
```

Feel free to reach out if you have any questions or need further assistance.
