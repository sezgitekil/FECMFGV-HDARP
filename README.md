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

For a detailed description please see the aformentioned reference. 


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





