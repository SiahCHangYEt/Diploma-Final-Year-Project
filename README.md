Genetic Algorithm for Solving the Berlin52 TSP
This project implements a Genetic Algorithm (GA) from scratch to solve the Traveling Salesman Problem (TSP) using the Berlin52 dataset. The goal is to find the shortest possible route that visits 52 cities in Berlin exactly once and returns to the starting point.

🚀 Performance Summary
Best Distance Achieved: 7777.54

Global Optimum (Berlin52): 7542.00

Error Margin: ~3.1%

🛠️ Implementation Details
The algorithm utilizes the following evolutionary components:

Encoding: Permutation Encoding (52 City IDs).

Fitness Function: Total Euclidean distance between coordinates.

Selection: Tournament Selection (Size 3).

Crossover: Ordered Crossover (OX) to ensure valid permutations.

Mutation: Swap Mutation (Rate: 0.1).

Elitism: Preserves the best individual in each generation.

📋 Experimental Setup
Population Size: 1,000

Generations: 1,000

Dataset: TSPLIB Berlin52 (52 cities)

Environment: Python 3 (Google Colab)

📂 File Structure
TSP_Genetic_Algorithm.ipynb: The main notebook containing the code, data dictionary, and visualization.

history: A list logging the best distance found in each generation.

graph: Matplotlib output showing the convergence of the algorithm over 1,000 generations.

⚙️ How to Run
Open the file in Google Colab or Jupyter Notebook.

Ensure matplotlib and numpy are installed.

Run all cells sequentially.

The final output will display the best distance found and a convergence plot.

📊 Observations
The algorithm demonstrates a rapid initial improvement, followed by plateaus. The 0.1 mutation rate was found to be optimal for fine-tuning the results, outperforming higher mutation rates by allowing for better exploitation of high-quality path segments without excessive disruption.
