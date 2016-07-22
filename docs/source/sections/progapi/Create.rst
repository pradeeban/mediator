Create Replica Set
******************

Replica sets can be created using a POST call.

Sample POST request
###################

http://localhost:9090/replicasets?iUserID=12&iCollection=TCGA-GBM&iPatientID=TCGA-06-6701%2CTCGA-08-0831&iStudyInstanceUID=1.3.6.1.4.1.14519.5.2.1.4591.4001.151679082681232740021018262895&iSeriesInstanceUID=1.3.6.1.4.1.14519.5.2.1.4591.4001.179004339156422100336233996679

This creates a replica set for the user with the user ID 12, with the given attributes of the images hosted in TCIA.


Sample POST response
####################

The expected response of the REST call is the ID of the replica set that was created in the previous replica set
creation POST request.

This is a random generated number.

-4764762120292626164


