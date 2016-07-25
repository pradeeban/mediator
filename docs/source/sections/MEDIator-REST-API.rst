*********************
MEDIator RESTful APIs
*********************

If you are hosting MEDIator for public access, you need to start it and expose its RESTful APIs. Execute the
MEDIatorEngine class. The implementation of the RESTful invocations can be found at TciaReplicaSetManager.

You may access MEDIator's RESTful APIs directly or through your application that consumes the MEDIator APIs.


You may extend or leverage the exposed APIs. To begin with, you may consume the MEDIator RESTful APIs through a REST
client such as the Postman plugin of the Chrome browser.


**MEDIator Client**

A sample Python client developed with Unirest has been included in MEDIator root directory.

You may just run it, after running the MEDIatorEngine, the core initialization class of the MEDIator server -

$ ./MEDIator_Client.py


You may have to change the execution mode of the client application prior to running it though.

$ chmod u+x MEDIator_Client.py



.. image:: arch.png
   :scale: 65
   :align: center


RESTful Invocations of MEDIator
###############################

.. toctree::
   :maxdepth: 1

   restapi/Create
   restapi/Retrieve
   restapi/Update
   restapi/Delete

