# [Efficient and Fair Traffic Flow Management for On-demand Air Mobility](https://dinamo-archive.mit.edu/sites/default/files/documents/CEAS_UTM_final.pdf)



## By: 

Christopher Chin (1), Karthik Gopalakrishnan (1), Hamsa Balakrishnan (1), Maxim Egorov (2), Antony Evans (2)

1. MIT AeroAstro
2. Airbus UTM

## Conference:

CEAS Aeronautical Journal

## The Transcendentals:

### The True:

- Fairness metrics:
  - Schedule reversal: flight $f_1$ is originally scheduled to arrive before $f_2$, but then then the schedule changes such that $f_2$ is scheduled to arrive first. (fewer reversals == more fair)
  - Overtaking: the magnitude of the reversal, measured by difference in arrival times. (less overtaking == more fair)
  - Time-order deviation: each flight should expect some delay according to the most constrained resource (i.e., veriport or air sector) along its route. Delay beyond this contribute to time order delay and should be equalized along multiple flights (this is the most confusing one).

### The Good:

Unmanned aerial systems (UAS) usage will be increasing significantly in the next decade. This increase will require both tactical (real-time) and strategic (minutes to hours in advance) scheduling. This paper explores the tradeoffs between fairness and efficiency in such a scheduling space, and finds that fairness can be improved with little loss in efficiency. It also seems like, because this paper has to account for on-demand scheduling that is not well-known in advance, that it could give insight on the normal TFMP in a highly disrupted (e.g., irregular operations) environment.

### The Beautiful:

Coolest finding, IMO: Finds that time-order deviation appears to be a promising metric because it is robust in its parameters and does not significantly compromise efficiency. It can also improve overtakes and reversals while optimizing for those other two does not improve time-order deviation.

## Key Contribution(s):

- Identifies nuances of UTM that prevent application of ATFM solutions
- Finds that:
  - Big gains in fairness can be achieved for all three metrics observed with little decrease in efficiency.
  - Depending on the fairness metric incorporated, it may increase the others or decrease the others (this is interesting!)
  - Pop-up flights can be incorporated into the optimization problem with a rolling horizon.


## Other important details:
- Evaluated using package delivery scenario simulation created by Airbus
- Use experiements with and without pop-up flights

## Acronyms:
- **ATFM**: Air Traffic Flow Management
- **UAS**: Unmanned Aircraft Systems
- **UTM**: Unmanned Aircraft Systems Traffic Management
