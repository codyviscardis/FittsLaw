## 🕹️ Interactive Experiment
<p align="center">
  <iframe 
    src="https://editor.p5js.org/codyviscardis/full/ggoWuNvm1" 
    width="100%" 
    height="500px" 
    style="border: none;">
  </iframe>
</p>

# FittsLaw
This project implements an experiment to validate Fitts' Law: $MT = a + b \cdot \log_2(\frac{2D}{W} + 1)$. Using a p5.js interface, user interaction data (Movement Time, Distance, Target Width) to calculate the Index of Difficulty and perform linear regression to determine the constants: delay and acceleration

# Workflow
## Data Collection
1. Open the p5.js web editor link
2. The user clicks start and then clicks a target that programmatically changes in size and distance
3. Once the trials are completed, the user automatically triggers a download of "fitts_law_data.csv"

## Data Analysis
1. Move fitts_law_data into the /data directory of this repo
2. Run fitts_law.ipynb to process the logs, filter out "warm-up" trials, and generate the models
