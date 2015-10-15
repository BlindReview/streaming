# streaming

Experiment Details and Code Repository

There are two main entries in the codes:

1. _featureGeneration.py: Python programs to generate the training features and testing features.

Help: _featureGeneration.py < upperbound | lowerbound | lable_threshold | t | support > 

     [upperbound]: Option, select cascades with length over the upperbound
     [lowerbound]: Option, select cascades with length under the lowerbound
     [lable_threshold]: Option, classification bound, the lable of cascade with length larger than lable_threshold is set to "1"; otherwise "-1"
     [t]: Option, select a subcascade with time delay less than t in each cascade
     [support]: Option, the support threshold used in the sequetial pattern mining

Example: python _featureGeneration.py 400 100 300 363250 70

2. mainEntry.m: The matlab programs which include optimazation part and classification part.

The results will be written into SSF.dat, OSF.dat, MSF.data and RSF.dat respectively.

Example: (the exampleData.dat)
1. python _featureGeneration.py 35 15 36 5 12
2. run mainEntry.m
