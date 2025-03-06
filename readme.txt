No. Nodes:    Total No. Processes:    Mean time (average of 3 runs) in seconds:    Parallel speed-up, S:
==========    ====================    =========================================    =====================
1            1                        0.007451                                    1.00
1            2                        0.004094                                    1.82
1            4                        0.001984                                    3.76
1            8                        0.001143                                    6.52
2            16                       0.001100                                    6.77
2            32                       0.001322                                    5.64

STATE IN WHICH CASES "-oversubscribe" WAS USED:
The "--oversubscribe" flag was used for p = 16 and p = 32.

A BRIEF INTERPRETATION OF MY RESULTS:
1. Performance Scaling: The execution time decreases as the number of processes increases, showing good parallel speed-up up to p = 8.
2. Diminishing Returns: Beyond p = 8, speed-up gains start to level off due to communication overhead.
3. Communication Overhead: The drop in efficiency for p = 32 indicates that inter-process communication is a limiting factor.
4. Optimal Performance: The best performance gain is observed around p = 8 or p = 16 before diminishing returns set in.
