# Distributed-Fairness-Matching-Engine-with-Timestamp-Ordering-Results
This repository contains the remaining result of the paper of the same title 

# Figure 1 
The increase in fairness is at the expense of increased waiting time, as depicted in Figures 1. The increase in average additional latency was approximately equal to half of the window size for all cases tried. Longer windows resulted in higher tail latencies, such that the mean p95 in case of jitter increased from 90.2 ms to 253.2 ms using 200 ms window size. This is an example that shows the average waiting time cannot be used to determine the cost of correction.

<img width="520" height="462" alt="image" src="https://github.com/user-attachments/assets/8226f2d1-c078-4d7e-a4cf-f4901d1d9ee9" />  
Fig. 1 p95 end-to-end latency versus correction window 

# Figure 2
Fig. 2 merges the fairness benefit with the latency cost. Using the jitter, bigger windows from 100 ms to 200 ms contributed 50.2 ms to the mean waiting time and lowered true-order unfairness from 1.63% to 0.80%. If such a delay is acceptable depends on the application. With the clock offsets, bigger windows ultimately caused bigger waiting time and bigger true-order unfairness.

<img width="827" height="553" alt="image" src="https://github.com/user-attachments/assets/f704313c-127b-4ba0-a962-dcc58fd14ba5" />  
Fig. 2 Latency-fairness tradeoff

# Figure 3
Fig. 3 shows the measured end-to-end processing rate for the local durable pipeline. 5.44 to 6.97 orders per second are possible with asymmetric delays, and 6.47 to 7.67 with jitter. These are quantities measured for one particular load; some larger-window runs showed performance approaching those numbers. The performance increased quite significantly with larger windows, but because we did so few samples, and because the execution is deterministic, we cannot know whether that difference is a reproducible result.

<img width="520" height="462" alt="image" src="https://github.com/user-attachments/assets/4f3a3987-ff89-482b-b204-daaa85a326b9" />  
Fig. 3 end-to-end rate of processed workload in local pipeline

