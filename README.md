# Knights

- [Introduction](#introduction)
- [Complexity](#complexity)
- [How To Run](#how-to-run)

-----------------------------------------------------------------------------
## Introduction

In a Knights and Knaves puzzle, each character is either a knight or a knave. A knight will always tell the truth. Conversely, a knave will always lie. The objective of the puzzle is, given a set of sentences spoken by each of the characters, determine, for each character, whether that character is a knight or a knave. With several characters and several sentences, the puzzles can get trickier!

-----------------------------------------------------------------------------
## Complexity 

At `logic.py` there are several classes for different types of logical connectives. These classes can be composed within each other.

The `model_check` function takes a knowledge base and a query. The knowledge base is a single logical sentence. model_check recursively considers all possible models, and returns True if the knowledge base entails the query, and returns False otherwise.

At the top of `puzzle.py` six symbols are defined. Then there are four sentences. Each sentence must convert to a knowledge base.

For each knowledge base, we should convert all our basical knowledge: e.g. (if A is knight then A says true sentence) and (if A is knave then A says not true sentence)

The main function of this `puzzle.py` loops over all puzzles, and uses model checking to compute, given the knowledge for that puzzle, whether each character is a knight or a knave, printing out any conclusions that the model checking algorithm is able to make.

-----------------------------------------------------------------------------
## How To Run

Follow these steps to set up and run the knights.py:

- Navigate to the project directory: cd /workspaces/KNIGHTS/knights
- Run the program: python puzzle.py
