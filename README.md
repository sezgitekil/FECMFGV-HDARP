# FECMFGV-HDARP

"Solving a Hybrid Mixed Fleet Heterogeneous Dial-a-Ride Problem in Delay-Sensitive Container Transportation"
 

Sezgi Tekil-Ergün 1, Erwin Pesch 2,1*, Katarzyna Anna Kuzmicz 3

1 Center for Advanced Studies in Management, HHL Leipzig Graduate School of Management, Leipzig 04109, Germany
2 Institute of Information Systems, Faculty III, University of Siegen, Siegen 57068, Germany
3 Faculty of Engineering Management, Bialystok University of Technology, 15-351 Bialystok, Poland
*Corresponding author: erwin.pesch@uni-siegen.de

Here you find definitions of the small and medium sized instances for 8, 12, 16, 20, 24, 28, 32 requests to eveluate the performance of 
the Full and Empty Container Mixed Fleet Green Vehicle Heterogeneous Dial-a-Ride Problem (FECMFGV-HDARP). The instances for each group of data are named by an 
alternating pattern of letters and numbers, e.g., in 3f1p1d2s(A), the number of full container pick-up requests (3), the number of empty container pick-up requests (1), 
the number of empty container delivery requests (1), the number of AFSs (2),and letter A indicates the data type A (i.e., for A-type data, the number of full container 
requests is slightly more than the number of empty container requests, while the quantity of full and empty container requests is assumed to be the same in the B-type 
data).The name of each data group has the same format, e.g., in 2f2p2d2s1nB, except that the two positions before the data type B indicated sample number (1).

The objective of the problem is minimizing the total distance. Distance is Euclidean, and the value of travel time is not equal to the value of distance between two 
nodes and the average vehicle speed is assumed to be constant and set to 50 (km/h). The position of each client and AFS is randomly generated, assuming integer coordinates 
randomly selected from the interval [50,..,300] km with equal probability. Besides, we generate a narrow grid as each vehicle has a limited capacity of its fuel tank, and 
each vehicle needs to be refueled after 370 miles (about 600 km).Fuel tank capacity and consumption rate of both loaded and unloaded natural gas-powered trucks are set to 
285 liters and 0.45 liters/km, respectively.The service time is assumed to be 10 minutes for a full or empty container pick-up/drop-off. 

The instances are classified into two groups “A” and “B”, with different degrees of heterogeneity of full and empty container requests. Then, we analyze the 
impact of the time windows, the number of vehicles, and AFSs for each group of instances by considering six scenarios. For A-type data, the percentage of the 
full container pick-up requests, the full container drop-off requests, and the empty container requests are set to 40%, 40%, and 20%, respectively. Furthermore, 
for B-type data the full container pick-up and drop-off requests contribute to 25% each of the total requests and the empty container requests have a share of 50% of 
the total requests. Notably, in each data instance, the percentage of the empty container pick-up requests and empty container drop-off requests is set to 60% and 40% 
of the total quantity of empty container requests, respectively. The characteristics of these instances are summarized in Table 4. The influence of the AFSs on the 
solutions is analyzed by varying the number of fuel stations (2, 4, and 6) for each instance. In the scenario “T1”, all clients are served by 4 (k1, k2, k3, k4) operating
vehicles each of a different type (truck with a 20-foot container (k1); tractor with two 20-foot containers (k2); tractor with a 40-foot container (k3); tractor with 20-40 foot 
containers (k4)) with time windows ranging from 15 to 150 hours, and the maximum length of a route (Tmax) varies between 17-160 hours based on the data sets. 
The impact of the number of vehicles has been compared to the original value of four vehicles of different types by setting the number of vehicles to 6 (k1, 2k2, k3, 2k4),
and 8 (2k1, 2k2, 2k3, 2k4) in the scenario “T2” and “T3”, respectively, without changing time windows. Indeed, narrow time windows for each client can make a solution
infeasible and have an impact on the run time.Therefore, in the scenarios “T4”, “T5”, “T6”, time windows are fairly narrow ranging from 1 to 5h, and Tmax differs in 
between 15-160 hours, for scenarios “T4”, “T5”, “T6” which resemble the scenarios “T1”, “T2”, “T3”, respectively.  We generate client data as a pair of locations and 
requests.  In case a client demands several full/empty containers we generate dummy locations to allow visiting the same location more than once.

Below is a description of the text files for instance 2f2p2d2sB. 

DistanceMatrix2_F2_P2_D_2S_No1.txt includes the Euclidean Distance Matrix of 8 locations (the number of full container pick-up requests (2), the number of empty container
pick-up requests (2), the number of empty container delivery requests (2)) and 2 stations (the number of AFSs (2))for sample number 1 (No1).

TimeMatrix2_F2_P2_D_2S_No1.txt includes the Time Matrix of the 8 locations and 2 stations for sample number 1.

FuelLevel4_T.txt, Resource4_T.txt, Truck4_T.txt flies include the data about fuel capacity, resource capacity, and the total capacity of 4 different types of Truck, respectively.

demand2_F2_P2_D.txt provides demand data for 8 requests(2 full container pick-up requests, 2 empty container pick-up requests, and 2 empty container delivery requests)

In the variables8_N900_T2_P_No1.txt file, the first row shows the service time of requests and 0 denotes the service time of the depot. The second row is the earliest and the third
row is the latest visiting times of the 8 locations. The maximum length of the route (Tmax) is 900 min. 

2f2p2d2s1nB.txt is generated for benchmarking and below is a description of the format of the text file. 

'NumNodes' is the number of requests in total.
'NumPicNodes' is the total number of pick-up requests.	
'NumTrucks' is the number of trucks.	
'NumStations' denotes the number of stations.
'NumPicFull' is the number of pick-up full container requests.
'NumPicEmpty' is the number of pick-up empty container requests.	
'NumDelEmpty' is the number of drop-off empty container requests.	
'Tmax'is the maximum length of the route. 
'DistanceMatrix' is the number of the sample.





