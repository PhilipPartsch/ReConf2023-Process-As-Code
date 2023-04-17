#######
Testing
#######


.. contents:: Content


*******
Process
*******

.. process:: Test the product
   :id: PROC_TEST_PRODUCT
   :activities: ACT_PRODUCT, ACT_PRODUCT2

   The purpose of this process is ensure functionality of a feature / requirmeent
   with tests.


******************
Process activities
******************

This process contains the following `process activities`:

.. activity:: Develop Test Specification
   :id: ACT_TEST_SPEC
   :responsible: ROLE_DEV
   :input: ART_SW_REQ
   :output: ART_TEST_SPEC
   :successor: ACT_DEV_TEST_CASE

   Entry criteria
   --------------

   Task
   ----

   Exit criteria
   -------------



.. activity:: Develop Test Case
   :id: ACT_DEV_TEST_CASE
   :responsible: ROLE_DEV
   :input: ART_TEST_SPEC
   :output: ART_TEST_CASE
   :successor: ACT_AUTO_TEST

   Entry criteria
   --------------

   Task
   ----

   Exit criteria
   -------------



.. activity:: Automate Tests
   :id: ACT_AUTO_TEST
   :responsible: ROLE_DEV
   :input: ART_TEST_CASE
   :output: ART_TEST_LOG, ART_TEST_RESULT, ART_TEST_COVERAGE
   :instruction: INST_AUTO_TEST

   Entry criteria
   --------------

   Task
   ----

   Exit criteria
   -------------
