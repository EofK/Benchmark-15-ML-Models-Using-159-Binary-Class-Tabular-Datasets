Benchmarking Classical Machine Learning Models on Tabular Binary Classification
This repository contains the reproducible code and results for a benchmarking study evaluating the performance of 15 classical machine learning model families across 159 tabular binary‑classification datasets. The project emphasizes methodological transparency, reproducibility, and clear documentation.

This repository includes the final report and supporting Python notebooks for the analysis and comparison of 15 machine learning models on a supervised classification task. The project addresses four core questions: 
1.  Which models perform best overall? 
2.  What makes datasets difficult to classify? 
3.  Which models handle specific complexity types most effectively? 
4.  How do accuracy and speed trade off across models?

The final report documents model performance and throughput, dataset characteristics, and tradeoffs between performance and efficiency. Using the Lorena et al. framework, the report characterizes each of the 159 datasets across 22 complexity dimensions spanning feature discriminability, class separability, geometric structure, and neighborhood cohesion. By correlating these complexity measures with the performance of 15 diverse models, the analysis identifies not only which models perform best overall, but also which algorithms are best suited to handle specific types of dataset difficulty.

Repository Structure

•	notebooks Cleaned Jupyter notebooks used for data preparation, feature processing, model training, and model evaluation. Each notebook is numbered to reflect the recommended execution order.
    
•	results 
    
    Contains the consolidated Excel file with 2,384 model–dataset pairs, including accuracy, throughput, and metadata used in the analysis.
    
•	requirements.txt 
    Python package dependencies required to reproduce the environment used for all experiments.
    
•	LICENSE 

    MIT license information governing use, distribution, and modification of this repository.
    
•	README 

    This document


Project Overview

The goal of this project is to systematically evaluate how well different classical machine learning model families perform on heterogeneous tabular datasets. The study includes:

    •	22 dataset complexity measures

    •	8 model families

    •	2,384 model–dataset evaluations

    •	Accuracy and throughput metrics

    •	Correlation analyses between complexity and performance.


The analysis is designed to support reproducible benchmarking and to provide insight into how dataset characteristics relate to model performance.

Complexity Analysis 

Dataset complexity was measured using the `problexity` library implementation of Lorena et al. (2019) measures. See `notebooks/08_calculate_dataset_complexity.ipynb` for the complete calculation workflow. 

The `problexity` library requires specific data formatting. Refer to the notebook for working example.


How to Use This Repository

1.	Clone the repository
git clone https://github.com/<your-username>/<repo-name>.git

2.	Install dependencies
pip install -r requirements.txt

3.	Open the notebooks Launch Jupyter or VS Code and run the notebooks in the order listed in the notebooks/ directory.

4.	Explore results The Excel file in results/ contains all model–dataset outcomes used in the analysis.

Reproducibility Notes

•	All experiments were run using a fixed Python environment defined in requirements.txt.

•	Random seeds were set where applicable to support reproducibility.

•	The 159 raw datasets  used for this project are listed in Appendix D of the Final Report, including a link to each dataset. The datasets are not included in this repository.


Citation

If you use this repository or its results in academic work, please cite it appropriately: Ed Kaempf, Benchmarking 15 Machine Learning Models for Binary Classification: Accuracy, Complexity, and Speed, January 2026.

License

    This project is licensed under the MIT License.  Refer to the “LICENSE” file for details.
    
Contact Information

For questions or suggestions, feel free to contact:

    •	Name: Ed Kaempf

    •	Email: edkaempf@gmail.com 

    •	GitHub: github.com/EofK 

    •	Linkedin: https://www.linkedin.com/in/ed-kaempf-4887839b/ 











