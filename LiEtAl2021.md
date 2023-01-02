# [Dynamics of Disruption and Recovery in Air Transportation Networks](https://dinamo-archive.mit.edu/sites/default/files/documents/Li-etal-CEAS2021.pdf)

## By: 

Max Z. Li (1), Karthik Gopalakrishnan (1), Hamsa Balakrishnan (1), Sang Shin (2), Darsh Jalan (2), Aritro Nandi (2), Lavanya Marla (2)

1. MIT AeroAstro
2. University of Illinois at Urbana-Champaign Department of Industrial and Enterprise Systems Engineering

## Conference:

CEAS 2021

## The Transcendentals:

### The True:

Give a 1-5 sentence summary and/or

- Total Variation (TV) = sum over all combinations of two airports of the correlation coefficient of historical airport delays times the squared difference of average delay between those airports for that hour. If the two airports are highly correlated, a bigger difference in delays will make this value higher for that airport combo, while a smaller difference will make this value lower. If two airports are uncorrelated, this value will be a lot lower no matter what.
- $||\textbf{x}(t)||$ = the total delay at a certain time
- Plot TD on x axis and TV on y axis for a particular time
  - Uses $\hat{\theta}$ to identify upper and lower bounds for what is expected
  - Uses $f$ to denote a large TD value
  - Creates a partition of TD-TV space: nominal (in theta bounds, less than f), scale (in theta bounds, greater than f, meaning there's a lot of delay but the spatial distribution is expected), and distribution (outside of theta bounds, unexpected spatial distribution of delay).
  - Note that, at any given time, the delay in the system falls into one of these three areas
  - Can then plot a trajectory of some time sequence where the network starts in nominal, transitions through states then ends up in distribution, then transitions some more and ends up in nominal again. Thi s sequence is known as a disruption-recover trajectory and is one way of characterizing a disruption in the network.
- Each maneuver (t to t + 1) can be a trade-off (TV and TD change in opposite directions) or symbiotic (TV and TD change in the same direction).
- A transition is a maneuver where the region changes

### The Good:

Despite the massive economic and personal effects they have, airport disruption events are surpisingly not particularly well understood. More light can be shed on these events by utilizing graph signal processing techniques.

### The Beautiful:

- Unveils error caused by unusual spacial distribution of errors that isn't generally captured by total delay-related metrics.

## Key Contribution(s):

- Use graph signal processing to define the start, progressing, and end of disruption cycles in a tranportation network.
- Use disruption-rcovery trajectories to develop features to cluster these disruptions
- Two observations from applying these techniques to operational data


## Other important details:

- Really interesting tidbit: "Further investigation would be needed to determine what specific initiatives and policies might have caused this shift in disruption-recovery dynamics in 2017." What happened in 2017? Did this continue in ensuing years?

## Other papers that might be of interest:

-  **"Modelling the resilience, friability and costs of an air transport network
affected by a large-scale disruptive event"** and **"Network adaptability from disaster disruptions and cascading failures"**: analyzing disruptions and recoveries in a networked system is a growing field of study, and is closely related to understanding system resilience. Significant prior work has focused on developing models for such systems, and then analyzing them theoretically or through simulations [8,12]

