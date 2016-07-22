*******************
MEDIator Interfaces
*******************

MEDIator consists of 3 interfaces for data source management and replica set management.


Data Source Management
######################

Data source management refers to the management of the original data sources replicated by MEDIator. The implementation
of the data source management is often offered by the data source providers themselves.

Relevant classes can be found in the package: ds_mgmt.

Data source management module manages the data sources themselves.

The relevant interfaces and implementations are often provided by the data sources or the data providers, and hence
orthogonal to MEDIator. However, a TCIA data source management RESTful interface and implementation are included.


Replica Set Management
######################

Relevant classes can be found in the package: rs_mgmt.

Replicaset management module manages the replica sets pointing to each of the data sources.

ReplicaSetHandlers are implemented for each of the data sources that are federated by MEDIator. The ReplicaSetHandlers
offer an internal implementation of the replica sets management.

ReplicaSetManagers are the core REST APIs of MEDIator. They leverage the ReplicaSetHandlers to manage the replica sets
of each of the data sources. There is a one-to-one mapping between the ReplicaSetManager api implementations and the
data sources.

TciaReplicaSetManager provides the REST API for managing the TCIA replica sets. Relevant documentation can be found in
the class as the method-level comments.


Integrator
##########
Relevant classes can be found in the package: integrator.

ReplicaSetsIntegrator is a singleton that manages integration of all the data sources for the replica set management.

Hence, ReplicaSetsIntegrator is a single entity that has a one-to-many relationship with the data sources of MEDIator
for the replicaset management.
