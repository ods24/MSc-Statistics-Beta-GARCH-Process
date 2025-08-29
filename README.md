# MSs-Statistics-Beta-GARCH-Process
Repository for MSc in Statistics 2025 Masters Dissertation: Analysing GARCH Processes with Beta-Distributed Innovations.

This contains the Jupyter notebooks and Mathematica notebooks for constructing the report, as well as all figures for further examination.

## Structure
- `jupyter_notebooks/` – Jupyter notebooks (`.ipynb`) used for analysis
- `mathematica_notebooks/` – Wolfram Mathematica notebooks (`.nb`) used for predictive densities
- `figures/` – Figures exported from notebooks and included in the LaTeX report
- `requirements.txt` – Python dependencies needed to run the notebooks

A comprehensive file list is provided below.

## How to run the Jupyter notebooks
1. Install Python (the version I used: 3.10.0).

2. Create a virtual environment:

   ```bash
   python -m venv .venv
   source .venv/bin/activate  # On Windows: .venv\Scripts\activate
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Launch Jupyter and open any notebook:

   ```bash
   jupyter notebook
   ```
   
## How to run the Mathematica notebooks

The `mathematica/` folder contains Wolfram Mathematica notebooks (`.nb`) used in this report.  

To open them:

1. If you have Wolfram Mathematica installed locally, just open the `.nb` file via Wolfram, making sure it has saved with the correct filename extension.  
2. Alternatively, you can upload the file to [Wolfram Cloud](https://www.wolframcloud.com/) to view it in browser.

## Comprehensive File list

### Jupyter Notebooks

- `SP500 Returns.ipynb` - Used for producing the Beta covergence graphs (figure 1 in the report).
- `Beta Distribution Convergence Graph.ipynb` - Used for producing the Beta covergence graphs (figure 2 in the report).
- `GJR-GARCH Generations.ipynb` - Used for producing simulated Beta-GARCH and Gaussian processes (figures 6, 7 in the report).

### Mathematica Notebooks

- `Predictive_densities.nb` - Used for generating plots for the predictive time steps at 0 (innovations), 1, 2 (figures 3, 4, 5 in the report); provides normalisation and first, second moments calculations . 

### Figures

- `SP500-log-returns.png` - Figure 1 in the report: shows the log-returns of the S&P500 index; generated using `Beta Distribution Convergence Graph.ipynb`.
- `BetaNormalConvergence.png` - Figure 2 in the report: shows the Beta innovations converging to Gaussian in the a-parameter limit; generated using `Beta Distribution Convergence Graph.ipynb`.
- `h0_h1_h2_h3_main.pdf` - Figure 3 in the report: shows the whole h=0,1,2,3 predictive densities; generated using `predictive_densities.nb`.
- `h0_h1_h2_h3_tails.pdf` - Figure 3 in the report: shows the tails of the h=0,1,2,3 predictive densities; generated using `predictive_densities.nb`.
- `h2_different_alpha_beta_main.pdf` - Figure 4 in the report: shows the whole h=2 predictive densities for different alpha, beta parameters; generated using `predictive_densities.nb`.
- `h2_different_alpha_beta_tails.pdf` - Figure 4 in the report: shows the tails of the h=2 predictive densities for different alpha, beta parameters; generated using `predictive_densities.nb`.
- `h2_different_lambda_main.pdf` - Figure 5 in the report: shows the whole h=2 predictive densities for different alpha, beta parameters; generated using `predictive_densities.nb`.
- `h2_different_lambda_main.pdf` - Figure 5 in the report: shows the tails of the h=2 predictive densities for different alpha, beta parameters; generated using `predictive_densities.nb`.
- `Different-Beta-Generations-2_4_10_100.png` - Figure 6 in the report: shows GARCH generations for different a parameters; generated using `GJR-GARCH Generations.ipynb`.
- `GARCH-density-sims-Normal_2_4_10_100.png` - Figure 7 in the report: shows unconditional returns generations for different a parameters; generated using `GJR-GARCH Generations.ipynb`.





