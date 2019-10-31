# thalassa
A small virus in bash with a DNA sequence that evolves as it propagates.

## DISCLAIMER
This bash script _will_ infect all bash files in the folder where it is, and all subfolders. Once they're infected, those bash files will (upon running) also infect all files in their folder and subfolders (unless they're already infected, in which case nothing happens).

I've done everything possible to ensure that the virus doesn't spread into parent folders (just to keep it more contained), and that it does not write itself into the same files over and over again. So, it should not inflate your bash files eternally.

# General description
thalassa.sh is a harmless virus-like script in bash, with a synthetic biology twist.

It has its own 1000 bp DNA sequence (variable CURRENT_SEQUENCE), and every time the code copy-pastes itself into a new file, the sequence mutates in exactly one random nucleotide, which changes into another random nucleotide. It kind of resembles a Jukes-Cantor (JC) model.

It also includes the original, ancestral sequence (variable ANCESTRAL_SEQUENCE), in case anyone would like to compare it.

The idea is that as it spreads, the sequence evolves, and at any one time, the infection (i.e. evolutionary) history can be reconstructed with a simple phylogenetic analysis under the JC model.

As you can see in the code, that's all it does.

The code I've uploaded already has a random mutation in its CURRENT_SEQUENCE, so any further infections will bear the mark of the 'GitHub bash version'. I plan to make a python version of the code, and that will also have another random mutation so it can be traced back to the 'GitHub python version'.

Have fun!
