# roundingsat

roundingsat is a pseudo-boolean SAT solver for optimization and decision problems.

## Compilation

The solver currently consists of a single file which can be compiled on Linux. It uses some c++11 constructs.

    g++ -o roundingsat roundingsat.cc -std=c++11 -O3

## Usage

For the input format, see [here](InputFormats.md).

Download OPB files:

    curl http://www.cril.univ-artois.fr/PB12/bench12/PB12-DEC-SMALLINT-LIN.tar | tar xv
    
Try on an example instance which is solved quickly:

    bzcat ./PB12/normalized-PB12/DEC-SMALLINT-LIN/sroussel/ShortestPathBA/normalized-BeauxArts_K76.opb.bz2 | ./roundingsat

## References on PB SAT solving

- [Dixon et al., 2004] H. E. Dixon, M. L. Ginsberg, and A. J. Parkes. Generalizing Boolean satisfiability I: Background and survey of existing work. *JAIR*, 21:193–243, 2004.
- [Chai and Kuehlmann, 2005] D. Chai and A. Kuehlmann. A fast pseudo-Boolean constraint solver. *IEEE Trans. Computer-Aided
Design of Integrated Circuits and Systems*, 24(3):305–317, 2005.
- [Elffers and Nordström, 2018] J. Elffers and J. Nordström. Divide and Conquer: Towards Faster Pseudo-Boolean Solving. *IJCAI 2018*, 1291-1299.
