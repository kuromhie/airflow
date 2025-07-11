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


Apache Kafka Triggers
=====================

.. _howto/triggers:AwaitMessageTrigger:

AwaitMessageTrigger
------------------------

The ``AwaitMessageTrigger`` is a trigger that will consume messages polled from a Kafka topic and process them with a provided callable.
If the callable returns any data, a TriggerEvent is raised.

For parameter definitions take a look at :class:`~airflow.providers.apache.kafka.triggers.await_message.AwaitMessageTrigger`.


KafkaMessageQueueTrigger
----------------------------------

The ``KafkaMessageQueueTrigger`` is a dedicated interface class for Kafka message queues that extends
the common :class:`~airflow.providers.common.messaging.trigger.msg_queue.MessageQueueTrigger`. It is designed to work with the ``KafkaMessageQueueProvider`` and provides
a more specific interface for Kafka message queue operations while leveraging the unified messaging framework.

For parameter definitions take a look at :class:`~airflow.providers.apache.kafka.triggers.msg_queue.KafkaMessageQueueTrigger`

For how to use the trigger, refer to the documentation of the :ref:`Apache Kafka Message Queue Trigger <howto/triggers:KafkaMessageQueueTrigger>`
