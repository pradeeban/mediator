*********************
MEDIator RESTful APIs
*********************

If you are hosting MEDIator for public access, you need to start it and expose its RESTful APIs. Execute the
MEDIatorEngine class. The implementation of the RESTful invocations can be found at TciaReplicaSetManager.

You may access MEDIator's RESTful APIs directly or through your application that consumes the MEDIator APIs.


You may extend or leverage the exposed APIs. To begin with, you may consume the MEDIator RESTful APIs through a REST
client such as the Postman plugin of the Chrome browser.


.. image:: arch.png
   :scale: 80
   :align: center


Contents
########

.. toctree::
   :maxdepth: 1

   restapi/Create
   restapi/Retrieve
   restapi/Update
   restapi/Delete

