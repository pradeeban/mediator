******************
Delete Replica Set
******************

An existing replica set can be deleted by invoking the relevant DELETE REST API, following the format of,

/DELETE

/replicaset/:id"


The replica set with the given ID would be deleted.


**Sample DELETE request**

http://localhost:9090/replicaset/12?replicaSetID=-9176938584709039161


**Sample DELETE response**

true

or

false


True, if successfully deleted the replica set with the given ID, and false if the delete failed for some reason.
