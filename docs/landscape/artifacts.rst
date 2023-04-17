.. _artifacts:

#########
Artifacts
#########


Content
=======

.. contents:: Content



.. artifact:: Issues
   :id: ART_ISSUES
   :stored_in: REPO_CM
   :status: draft

   With :need:`ART_ISSUES` we communicate with :need:`ROLE_STK`,
   :need:`ROLE_DEV` and :need:`ROLE_MAIN`.



.. artifact:: Stakeholder Requirement Specification
   :id: ART_STAKE_REQ_SPEC
   :stored_in: REPO_GIT

   A :need:`ART_STAKE_REQ_SPEC` is a file containing :need:`ART_STAKE_REQ`.



.. artifact:: Product Requirement Specification
   :id: ART_PROD_REQ_SPEC
   :stored_in: REPO_GIT

   A :need:`ART_PROD_REQ_SPEC` is a file containing :need:`ART_PROD_REQ`.



.. artifact:: Software Requirement Specification
   :id: ART_SW_REQ_SPEC
   :stored_in: REPO_GIT

   A :need:`ART_SW_REQ_SPEC` is a file containing :need:`ART_SW_REQ`.



.. artifact:: Stakeholder Requirement
   :id: ART_STAKE_REQ
   :stored_in: ART_STAKE_REQ_SPEC

   A :need:`ART_STAKE_REQ` is a part of a :need:`ART_STAKE_REQ_SPEC`.
   A :need:`ART_STAKE_REQ` has bidirectional traceability to:

      - :need:`ART_PROD_REQ`



.. artifact:: Product Requirement
   :id: ART_PROD_REQ
   :stored_in: ART_PROD_REQ_SPEC

   A :need:`ART_PROD_REQ` is a part of a :need:`ART_PROD_REQ_SPEC`.
   A :need:`ART_PROD_REQ` contains a verification criteria.
   A :need:`ART_PROD_REQ` has bidirectional traceability to:

      - :need:`ART_STAKE_REQ`



.. artifact:: Software Requirement
   :id: ART_SW_REQ
   :stored_in: ART_SW_REQ_SPEC

   A :need:`ART_SW_REQ` is a part of a :need:`ART_SW_REQ_SPEC`.



.. artifact:: Software Architecture
   :id: ART_SW_ARC
   :stored_in: REPO_GIT

   A :need:`ART_SW_ARC` is containing :need:`ART_SW_ARC_ELE`
   to model the software.



.. artifact:: Software Architecture Element
   :id: ART_SW_ARC_ELE
   :stored_in: ART_SW_ARC

   A :need:`ART_SW_ARC_ELE` is a part of :need:`ART_SW_ARC`
   to model the software.



.. artifact:: Software Design
   :id: ART_SW_DESIGN
   :stored_in: REPO_GIT
   :status: draft

   Todo



.. artifact:: Software Unit
   :id: ART_SW_Unit
   :stored_in: REPO_GIT
   :status: draft

   Todo



.. artifact:: Software Component
   :id: ART_SW_Comp
   :stored_in: REPO_GIT
   :status: draft

   Todo



.. artifact:: Software Binary
   :id: ART_SW_Binary
   :stored_in: REPO_WEB
   :status: draft

   Todo



.. artifact:: User Software Documentation
   :id: ART_SW_DOCU
   :stored_in: REPO_WEB

   The :need:`ART_SW_DOCU` is documenting how to use
   :need:`ART_SW_Binary`.



.. artifact:: Developer Documentation
   :id: ART_DEV_DOCU
   :stored_in: REPO_WEB

   The :need:`ART_DEV_DOCU` is covering the engineering domains like
   - requirements engineering
   - Architecture
   - Test Specifications
   - Test Results



.. artifact:: Software Integration Specification
   :id: ART_INT_SPC
   :stored_in: REPO_GIT

   The :need:`ART_INT_SPC` is specifying what shall be integrated to a
   :need:`ART_SW_Binary`.
   During integration we expect to get a :need:`ART_INT_RPRT`.



.. artifact:: Software Integration Report
   :id: ART_INT_RPRT
   :stored_in: ART_DEV_DOCU

   The :need:`ART_INT_RPRT` is reported after a :need:`ART_INT_SPC` was been build
   to :need:`ART_SW_Binary`.



.. artifact:: Software Test Specification
   :id: ART_TEST_SPEC
   :stored_in: REPO_GIT

   The :need:`ART_TEST_SPEC` is specifying how a :need:`ART_SW_Unit`,
   :need:`ART_SW_Comp` or :need:`ART_SW_Binary` shall be tested.
   During testing we expect to get a :need:`ART_TEST_RESULT`.



.. artifact:: Software Test Case
   :id: ART_TEST_CASE
   :stored_in: REPO_GIT

   The :need:`ART_TEST_CASE` is implmenting a :need:`ART_TEST_SPEC`.
   During testing we expect to get a :need:`ART_TEST_RESULT`.



.. artifact:: Software Test Result
   :id: ART_TEST_RESULT
   :stored_in: ART_DEV_DOCU

   The :need:`ART_TEST_RESULT` is the result of a Software Test Execution specified by
   :need:`ART_TEST_SPEC`.



.. artifact:: Software Test Log
   :id: ART_TEST_LOG
   :stored_in: ART_DEV_DOCU

   The :need:`ART_TEST_LOG` is the log of a Software Test Execution specified by
   :need:`ART_TEST_SPEC` and implemented in :need:`ART_TEST_CASE`.



.. artifact::  Release Notes
   :id: ART_REL_NOTE
   :stored_in: ART_SW_DOCU
   :status: draft

   Todo

.. artifact::  Release Branch
   :id: ART_REL_BR
   :stored_in: REPO_GIT
   :status: draft

   Todo



