# NEAT-Super-Mario
The classic game of Super Mario. But make AI play it.
Using pygame and NEAT.

# Instructions
Ensure you have the following installed on your local machine:
- Python 3 or above
- Suitable IDE

### Setup

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/harini-1597/NEAT-Super-Mario.git
   ```

2. Navigate to the project directory:

   ```bash
   cd NEAT-Super-Mario
   ```

3. Create a Python Virtual Environment (if you use VSCode, you can create one using the Command palette itself)

    ```bash
    python3 -m venv <myenvname>
    ```

3. Install requirements.txt:

   ```bash
   pip install -r requirements.txt
   ```


# Video Demo
https://github.com/harini-1597/NEAT-Super-Mario/assets/128628820/b4fee8a1-de32-4e24-b284-55d12719d660

# How it works
### Why NEAT?
NEAT, is an advanced Neural Network. Usually, neural networks are of this form:


![nn](https://github.com/harini-1597/NEAT-Super-Mario/assets/128628820/9149cc31-bd8a-4a12-a582-8c833800c543)


NN's modify and optimize the functionality by modifying their weights, based on the result of the activation function.

NEAT on the other hand, has the ability to *mutate*, meaning, it can either:
- add nodes
- add connections to other nodes
thus being able to vary its topology to identify the most suitable topology.


![neat](https://github.com/harini-1597/NEAT-Super-Mario/assets/128628820/aef13bf7-e66c-4ec5-95d7-ceabd7810ef1)


This is more suitable as the algorithm can tailor itself to be as complex or simple as the problem requires. For ex, Super Mario, a simple game, the NEAT can formulate a very simple Topology

But for more complex problems like User Based Recommendation systems, where each user is a different human, NEAT can evolve to be more complex.

### Fitness Function
To evolve a suitable solution to the problem, the user must provide a *fitness_function* something which tells the indivisula genome, in this case Mario, how well it performs. 

In this case the best Mario is someone who reaches the higest level. Through a user specified amount of generations, wherein each generation of a Mario is produced by mutation of the most fit individuals of the previous generations.

The reproduction and mutation operations may add nodes and/or connections to the NN. When the preset number of generations is reached, or when at least one individual's fitness value exceeds the user-specified threshold, the algorithm terminates.

Read more about NEAT here: [NEAT Official Docs](https://neat-python.readthedocs.io/en/latest/neat_overview.html)!

<!-- [![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/) -->
