# FilterNet (NeurIPS 2024)

The repo is the official implementation for the paper: "FilterNet: Harnessing Frequency Filters for
Time Series Forecasting".

## Updates
🚩News [2024.09]: [**FilterNet: Harnessing Frequency Filters for Time Series Forecasting**](https://neurips.cc/virtual/2024/poster/93257) has been accepted by NeurIPS 2024.

🚩News [2024.04]: [**Deep Frequency Derivative Learning for Non-stationary Time Series Forecasting**](https://arxiv.org/abs/2407.00502) has been accepted by IJCAI 2024.

🚩News [2024.03]: [**Deep Coupling Network For Multivariate Time Series Forecasting**](https://dl.acm.org/doi/abs/10.1145/3653447) has been accepted by TOIS.

🚩News [2023.09]: [**Frequency-domain MLPs are more effective learners in time series forecasting**](https://proceedings.neurips.cc/paper_files/paper/2023/hash/f1d16af76939f476b5f040fd1398c0a3-Abstract-Conference.html) and
[**FourierGNN: Rethinking Multivariate Time Series Forecasting from a Pure Graph Perspective**](https://proceedings.neurips.cc/paper_files/paper/2023/hash/dc1e32dd3eb381dbc71482f6a96cbf86-Abstract-Conference.html) 
have been accepted by NeurIPS 2023.

## Getting Started

### 1、Environment Requirements

To get started, ensure you have Conda installed on your system and follow these steps to set up the environment:

```
conda create -n FilterNet python=3.8
conda activate FilterNet
pip install -r requirements.txt
```

### 2、Download Data
All the datasets needed for FilterNet can be obtained from the [Google Drive](https://drive.google.com/drive/folders/1ZOYpTUa82_jCcxIdTmyr0LXQfvaM9vIy) provided in Autoformer. 

### 3、Training Example

For datasets with a small number of variables, such as ETTh, ETTm, and Exchange, we recommend using **PaiFilter** as follows:
```
bash ./scripts/PaiFilter/ETTm1.sh
bash ./scripts/PaiFilter/ETTm2.sh
bash ./scripts/PaiFilter/ETTh2.sh
```

For datasets with a large number of variables such as ECL, Traffic, and weather, it is recommended to use **TexFilter** as follows:
```
bash ./scripts/PaiFilter/ECL.sh
bash ./scripts/PaiFilter/Traffic.sh
bash ./scripts/PaiFilter/Weather.sh
```

## Acknowledgement

We appreciate the following GitHub repositories for providing valuable code bases and datasets:


https://github.com/aikunyi/FreTS

https://github.com/VEWOXIC/FITS

https://github.com/wanghq21/MICN

https://github.com/thuml/TimesNet

https://github.com/plumprc/RTSF

https://github.com/cure-lab/LTSF-Linear

https://github.com/zhouhaoyi/Informer2020

https://github.com/thuml/Autoformer

https://github.com/ant-research/Pyraformer

https://github.com/MAZiqing/FEDformer

https://github.com/yuqinie98/PatchTST

https://github.com/thuml/iTransformer