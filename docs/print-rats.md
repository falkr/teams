---
---

# Print RATs

When you print a RAT, Teampy creates a shuffled version of the questions for
each student, and shuffles the answers for the teams so that they match any
scratch cards that you may want to use.

    rat print --teamsolution abcdabcdab questions.txt

If you have defined the solutions of existing scratch cards in the [scratch cards file](setup.html), you just give the code of the scratch card:

    rat print --teamsolution D013 questions.txt

The result of this operation are two files:

* The file `questions.pdf` with the quizzes ready for printing. If you use the command line option `--nopdf`, Teampy creates a *.tex file instead that you can translate with LaTeX.
* The file `solutions.teampy`. This file contains the correct solution for each team and student. Teampy needs this file later when the RATs are evaluated, so **do not delete this file.**
