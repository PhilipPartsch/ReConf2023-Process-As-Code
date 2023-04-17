##############
Create Product
##############


.. contents:: Content


*******
Process
*******

.. process:: Create Product
   :id: PROC_CREATE_PRODUCT
   :activities: ACT_PRODUCT, ACT_PRODUCT2

   The purpose of this process is to develop from feature requests via ticket
   working software solutions.

   .. needarch::

      actor Developer

      package content{
      file Requirements
      file Architecture
      file SC as "Source code"
      file Test
      file Documentation

      Requirements -down[hidden]-> Architecture
      Architecture -down[hidden]-> SC
      SC -down[hidden]-> Test
      Test -down[hidden]-> Documentation

      }

      database git

      storage PR as "Pull Request"

      storage CI as "CI-Pipeline"

      package Web{
      node PA as "Process Artifacts"
      node Docu as "User Documentation"
      node Binary

      PA -down[hidden]-> Docu
      Docu -down[hidden]-> Binary
      }

      actor User

      Developer -right-> content: authors
      content -right-> git: "stored in"
      git -right-> PR: "Reviewed by"
      PR -right-> CI: "Build in"
      CI -right-> Web: "Delivered As"
      Web <-right- User: "Consums"


******************
Process activities
******************

This process contains the following `process activities`:

.. activity:: placeholder
   :id: ACT_PRODUCT
   :responsible: ROLE_DEV
   :input: ART_ISSUES
   :output: ART_SW_REQ
   :successor: ACT_PRODUCT2

   Entry criteria
   --------------

   Task
   ----

   Exit criteria
   -------------



.. activity:: placeholder
   :id: ACT_PRODUCT2
   :responsible: ROLE_DEV
   :input: ART_ISSUES
   :output: ART_SW_REQ

   Entry criteria
   --------------

   Task
   ----

   Exit criteria
   -------------