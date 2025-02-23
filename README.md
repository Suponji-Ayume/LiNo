<div align="center">
  <!-- <h1><b> Time-LLM </b></h1> -->
  <!-- <h2><b> Time-LLM </b></h2> -->
  <h2><b> Code for ICML2025 Submission:</b></h2>
  <h2><b> LiNo: Advancing Recursive Residual Decomposition of Linear and Nonlinear Patterns for Robust Time Series Forecasting. </b></h2>
</div>

## Get Started

1. Install requirements. ```pip install -r requirements.txt```
2. Download data. You can download the all datasets from iTransformer: [datasets](https://drive.google.com/u/0/uc?id=1NF7VEefXCmXuWNbnNe858WvQAkJ_7wuP&export=download). **All the datasets are well pre-processed** and can be used easily.
3. Train the model. We provide the experiment scripts of all benchmarks under the folder `./scripts`. You can replicate the benchmark results of **LiNo** from the paper by:
   
  ```python run_script.py```

4. Alternatively, you can use bash commands to individually run scripts in the 'scripts' folder from the command line to obtain results for individual datasets, take for example, you can use the below command line to obtain the multivariate forecasting result of  **input-96-predict-96** on ETTh1:
   
  ```bash ./scripts/Multivariate/ETTh1/96.sh ```

You can find:

The training history and results under './logs' folder.

The test results (MSE and MAE) under './test_dicts' folder.

The visualization of the overall prediction and prediction of each Li and No block under './visual_prediction' folder.

The visualization of the weight of each Li and No block under './visual_weight' folder.  **PS: The method used for getting the weight follows the approach outlined in [An Analysis of Linear Time Series Forecasting Models](https://arxiv.org/abs/2403.14587).**

## Several examples for better understanding the proposed LiNo in the paper (Multivariate forecasting case).

Within the storage limits of a GitHub repository, We provide training log files of tasks **input-96-predict-96** on **ETTh1&2, ETTm1&2, PEMS04&08, Weather, and ECL**, to assist readers in reproducing the results from the paper. 

Additionally, we offer visualizations of LiNo's prediction results on **ECL** and **ETTh2** datasets, showcasing the forecasting of each Li block and No block. 

Furthermore, we also provide visualizations of the overall weights of each Li block and No block on **ECL** and **ETTh2** datasets. 
