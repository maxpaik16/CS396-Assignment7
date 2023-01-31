# Assignment 7
Max Paik's  Repo for Assignment 7 for CS 396 Artificial Life at Northwestern University Winter 2023

Usage: run "python generate_body.py"

Description of how bodies/brains are generated:

My code begins by selecting the total number of blocks in the body. It then iterates through each block and flips a fair coin to decide whether or not that block will have a sensor. Next, it creates bodies block by block. At each step in the algorithm, a randomly shaped block (with x, y, z lengths randomly chosen between 0 and 1) is created. Then, another random number is generated that places the next block either in the +x, -x, +y, or -y direction relative to the last block. That same number also decides if the block is placed at the same z position as the last one or moved upward, ensuring that the bodies are created in three dimensions. After doing this, the brain is created by adding a sensor neuron for every block with a sensor. The brain is then made fully connected so every motor neuron (present at every joint) is connected to every sensor neuron. 
