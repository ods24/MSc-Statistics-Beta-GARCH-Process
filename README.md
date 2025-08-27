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

- `Beta Distribution Convergence Graph.ipynb` - Used for producing the Beta covergence graphs (figure 1 in the report).

### Mathematica Notebooks

- `Predictive_distributions.nb` - Used for generating plots for the predictive time steps at 0 (innovations), 1, 2; provides normalisation and first, second moments calculations.

### Figures

The following were generated using Jupyter notebooks:

- `FIG1-BetaNormalConvergence.png` - Figure 1 in the report: shows the Beta innovations converging to Gaussian in the a-parameter limit; generated using `Beta Distribution Convergence Graph.ipynb`.

The following were generated using `mathematica_notebooks/Predictive_distributions.nb`:

- `h0_h1_h2_main.pdf` – Figure XX in the report: predictive distributions for fixed parameters, at time steps 0 (innovations), 1, 2.
- `h0_h1_h2_tails.pdf` – As above, looking only at tails.





