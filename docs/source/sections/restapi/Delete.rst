*************************
Deleting the Replica Sets
*************************

An existing replica set can be deleted by invoking the relevant DELETE REST API, following the format of,

/DELETE

/replicaset/:id"


The replica set with the given ID would be deleted.



**Sample DELETE request**

http://lion.bmi.emory.edu/replicaset/12?replicaSetID=-9176938584709039161


**Sample DELETE response**

*true*

or

*false*


True, if successfully deleted the replica set with the given ID, and false if the delete failed for some reason.
