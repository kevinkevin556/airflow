 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
    distributed with this work for additional information
    regarding copyright ownership.  The ASF licenses this file
    to you under the Apache License, Version 2.0 (the
    "License"); you may not use this file except in compliance
    with the License.  You may obtain a copy of the License at

 ..   http://www.apache.org/licenses/LICENSE-2.0

 .. Unless required by applicable law or agreed to in writing,
    software distributed under the License is distributed on an
    "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.

===================
Amazon Redshift SQL
===================

`Amazon Redshift <https://aws.amazon.com/redshift/>`__ manages all the work of setting up, operating, and scaling a data warehouse:
provisioning capacity, monitoring and backing up the cluster, and applying patches and upgrades to
the Amazon Redshift engine. You can focus on using your data to acquire new insights for your
business and customers.

Prerequisite Tasks
------------------

.. include:: ../../_partials/prerequisite_tasks.rst

Operators
---------

Execute a SQL query
===================

The generic ``SQLExecuteQueryOperator`` can be used to execute SQL queries against an Amazon Redshift cluster using a :ref:`howto/connection:redshift`.

To execute a SQL query against an Amazon Redshift cluster without using a Redshift connection,
please check ``RedshiftDataOperator``.

.. exampleinclude:: /../../common/sql/tests/system/common/sql/example_sql_execute_query.py
    :language: python
    :dedent: 4
    :start-after: [START howto_operator_sql_execute_query]
    :end-before: [END howto_operator_sql_execute_query]

Reference
---------

* `AWS boto3 library documentation for Amazon Redshift <https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html>`__
* `Amazon Redshift Python connector <https://docs.aws.amazon.com/redshift/latest/mgmt/python-connect-examples.html>`__
