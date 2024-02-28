##### NAME - Ritika Reddy 
##### DATE - Feb 28 2024

# Lab7 

## TASK1 - Visualization of missingness results
#### 1- submission script 
The script missingnessPlot.sh is used to run the R script and generate the missingness plot. It helps SLURM scheduler known the parameters and run the ‘hist_miss.R’ script: 

Code: 
#!/bin/bash
#SBATCH --account=msbi32400
#SBATCH --time=00:30:00
#SBATCH --nodes=1
#SBATCH --ntasks-per-node=1
#SBATCH --mem-per-cpu=2000
#SBATCH --job-name=MissingnessPlot
#SBATCH --output=/home/ritika11/lab7/results/MissingnessPlot-%j.out
#SBATCH --error=/home/ritika11/lab7/results/MissingnessPlot-%j.err
module load R
Rscript --no-save /home/ritika11/lab7/src/hist_miss.R

#### 2 - The generated plots

