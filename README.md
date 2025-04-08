COVID-19 Vaccine Allocation Optimization

This repository contains the code and data for a research project that focuses on optimizing the allocation of COVID-19 vaccines across U.S. counties. The model integrates real-world epidemiological data, vaccine supply, and demand to inform strategic distribution policies. The main components include a Jupyter Notebook titled "Paper1-Implementation Code.ipynb" and an Excel file "Paper 1-Updated Data 1.29.25.xlsx". The notebook performs data preprocessing, parameter setup, infection rate calculations, and optimization using Gurobi, along with generating visualizations using Folium and Matplotlib. The Excel file contains COVID-19 case data by state and county, vaccine demand estimates, and regional demographic breakdowns.

To run the code, the following Python libraries are required: pandas, numpy, matplotlib, folium, gurobipy, requests, and openpyxl. These can be installed using pip. Gurobi also requires a valid license, which is available for free to academics at gurobi.com.

The optimization model is designed to minimize the total number of effective infections over a 12-period time horizon by allocating vaccines across U.S. counties. Key features of the model include reinfection modeling with a rate of 0.01, time progression over 12 two-week periods, a fixed vaccine effectiveness (e.g., 20%), and regional aggregation of counties. The objective is to minimize the sum of infections adjusted for vaccination impact, while constraints include vaccine supply limits per period, regional demand caps, and epidemiological dynamics including delayed immunity.

The notebook also includes visualizations. Folium maps display county-level vaccine allocations on interactive maps, while Matplotlib charts illustrate infection rate trends, vaccine distribution over time, and regional comparisons between baseline and optimized results.

To get started, clone the repository, open the notebook in Jupyter, and run all cells. This will load the data, execute the model, and generate all visual outputs.

This project is intended for academic and educational use only. Please contact the authors for reuse, citation, or collaboration.

Special thanks to the Gurobi team and providers of public COVID-19 datasets.
