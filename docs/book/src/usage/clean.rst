.. _CAPE-clean:

===========================
Clean all Tasks and Samples
===========================

To clean your setup, run `-h` to see available options::

    $ ./utils/cleaners.py -h

To sum up, this command does the following:

* Delete analysis results.
* Delete submitted binaries.
* Delete all associated information of the tasks and samples in the configured database.
* Delete all data in the configured MongoDB (if configured and enabled in reporting.conf).
* Delete all data in ElasticSearch (if configured and enabled in reporting.conf).

.. warning::
   If you use this command you will delete permanently all data stored by CAPE in all
   storages: file system, SQL database and MongoDB/ElasticSearch database. Use it only
   if you are sure you would clean up all the data.
