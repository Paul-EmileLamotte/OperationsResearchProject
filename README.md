 OperationsResearchProject


 Description

This Python program allows you to explore different network flow algorithms:

- Ford-Fulkerson algorithm for maximum flow
- Push-Relabel algorithm for maximum flow
- Minimum-Cost Flow algorithm
- Experimental complexity analysis with runtime visualizations

The program features an interactive command-line interface and automatically saves execution traces to text files.

 Features

- Compute maximum flow using Ford-Fulkerson
- Compute maximum flow using Push-Relabel
- Compute minimum-cost flow for a given demand
- Generate and display runtime graphs (scatter plots, worst-case behavior)
- Automatically save traces to output files
- Simple terminal-based interaction

 Requirements

- Python 3.7 or higher
- Required Python modules:
  - `matplotlib`
  - `numpy`

Install dependencies with pip:


pip install matplotlib numpy


 File Structure


.
├── code.ipynb                         Main program file
├── proposal1.txt to proposal10.txt   Input graph files
├── README.md


 How to Run

Execute the program using:


python code.ipnyb


You will be prompted to:
1. Enter your group (e.g., B)
2. Enter your team number (e.g., 4)
3. Choose one of the following options:
   - 1: Max Flow with Ford-Fulkerson
   - 2: Max Flow with Push-Relabel
   - 3: Min-Cost Flow
   - 4: Complexity Analysis

Results and traces will be shown in the console and saved to a trace file (e.g., `B4-trace2-FF.txt`).

 Input File Format

Files `proposal1.txt` to `proposal10.txt` contain adjacency matrices.

- Files 1 to 5: capacity matrices only (for max flow)
- Files 6 to 10: capacity matrices followed by cost matrices (for min-cost flow)

Example (3x3 capacity matrix):

```
3
0 5 0
0 0 8
0 0 0
```

For Min-Cost Flow (3x3):

```
3
0 4 0
0 0 6
0 0 0
0 2 0
0 0 3
0 0 0
```

(3 lines for capacity, followed by 3 lines for cost)

 Complexity Analysis

The analysis includes:
- Scatter plots of execution times
- Log-scale plots for the worst-case runtimes
- A comparison graph between Ford-Fulkerson and Push-Relabel

 Output Traces

Output files contain full execution traces. Filenames follow this format:


<group><team>-trace<number>-<method>.txt


Examples:
- `B4-trace3-FF.txt` (Ford-Fulkerson)
- `A2-trace5-PR.txt` (Push-Relabel)
- `C1-trace7-MIN.txt` (Min-Cost Flow)

 Authors
Lamotte--Chapon Paul-Emile, Iness Bennai
Project developed for the Operations Research course (SM602I).



