# IoT25-HW07
## Screenshots of Arduino
### Server
### Client
## Demo photo
## Test and Analyze
### Table
| Actual Distance (m) | Average Measured Distance (m) | Error (m) | Error Margin (%) |
|---------------------|-------------------------------|-----------|------------------|
| 0.3                 | 0.300667                      | 0.000667  | 0.22             |
| 0.5                 | 0.602                         | 0.102     | 20.40            |
| 0.8                 | 0.918                         | 0.118     | 14.75            |
| 1.0                 | 0.916                         | 0.084     | 8.40             |
| 1.5                 | 2.696                         | 1.196     | 79.73            |
### Bar Chart
![barChart](https://github.com/missyou2/IoT25-HW07/blob/main/barChart.png)
### Discuss

At a distance of **0.3 m**, the system showed high accuracy with an error of less than **0.0007 m**, corresponding to an error margin of approximately **0.22%**.  
- At **0.5 m**, the error was **0.102 m** (20.4%),
- at **0.8 m**, **0.118 m** (14.75%),
- at **1.0 m**, **0.084 m** (8.4%),
- and at **1.5 m**, the error increased significantly to **1.196 m**, resulting in an error margin of **approximately 79.74%**.

These results indicate that the error margin generally increased with distance.

Additionally, it was observed that RSSI values varied even at the same distance depending on the orientation and placement of the ESP32.  
When the ESP32 was not placed horizontally but at a diagonal angle, the RSSI signal became significantly weaker even at close range.

Fluctuations in RSSI were more noticeable at longer distances, but some degree of noise was also present even at shorter distances.  
Using techniques such as noise filtering could help reduce measurement spikes and provide more stable and reliable results.
