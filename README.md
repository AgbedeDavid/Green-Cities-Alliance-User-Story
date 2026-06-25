# Green-Cities-Alliance-User-Story

 # User Story Development

Requirements were decomposed into User Stories and supported by Behaviour-Driven Development (BDD) acceptance criteria to ensure requirements remained testable, measurable, and unambiguous.

# US-01 – Resident Registration

*User Story*

As a resident, I want to register on the platform so that I can browse and vote for environmentally friendly products and services.

*Acceptance Criteria*

*Scenario 1*: Successful Registration

Given the resident is on the registration page

When they complete all mandatory fields with valid information and submit the form

Then the resident record should be created successfully

And a confirmation message should be displayed

--

*Scenario 2*: Mandatory Field Validation

Given the resident is completing the registration form

When one or more mandatory fields are left blank

Then the registration should not be submitted

And an appropriate validation message should be displayed

# US-02 – Associate Resident to Area

*User Story*

As a resident, I want to select my residing area so that my activity can be associated with my local community.

*Acceptance Criteria*

*Scenario 1*: Area Selection

Given the resident is registering on the platform

When they select an area from the available list

Then the resident should be associated with the selected area

And the area information should be stored against their profile

--

*Scenario 2*: Area Not Available

Given the resident is registering on the platform

When their residing area is not available in the list

Then they should not be able to complete area selection

And they should be informed that the area has not yet been configured

# US-03 – Product Browsing & Filtering

*User Story*

As a resident, I want to filter products by environmental benefit and price category so that I can quickly find products that meet my needs.

*Acceptance Criteria*

*Scenario 1*: Filter by Environmental Benefit

Given products are available on the platform

When the resident selects an environmental benefit category

Then only products matching that category should be displayed

--

*Scenario 2*: Filter by Price Tier

Given products are available on the platform

When the resident selects a price tier

Then only products within the selected price tier should be displayed

--

*Scenario 3*: Combined Filtering

Given products are available on the platform

When the resident selects both an environmental benefit category and a price tier

Then only products matching both criteria should be displayed

# US-04 – Product Management

*User Story*

As an SME representative, I want to add and manage products so that residents can discover and vote on sustainable solutions.

*Acceptance Criteria*

*Scenario 1*: Add Product

Given the SME is registered on the platform

When they provide valid product information and submit the form

Then the product should be created successfully

And it should become available to residents

--

*Scenario 2*: Edit Product

Given an existing product is registered on the platform

When the SME updates the product information

Then the changes should be saved successfully

And the updated information should be displayed

# US-05 – Vote for a Product

*User Story*

As a resident, I want to vote for a product so that I can express my preference for sustainable products and services.

*Acceptance Criteria*

*Scenario 1*: Successful Vote Submission

Given the resident is registered

And the resident has not previously voted for the selected product

When they submit a vote

Then the vote should be recorded successfully

And the product ranking should be updated

--

*Scenario 2*: Duplicate Vote Prevention

Given the resident has already voted for a product

When they attempt to vote for the same product again

Then the vote should not be recorded

And an appropriate error message should be displayed

# US-06 – Ranked Product View

*User Story*

As an SME or Local Council representative, I want to view product rankings so that I can understand community demand and trends.

*Acceptance Criteria*

*Scenario 1*: View Rankings

Given products have received votes

When the ranking page is accessed

Then products should be displayed in descending order of vote count

And the highest voted product should appear first

--

*Scenario 2*: Ranking Refresh

Given a new vote has been successfully recorded

When the ranking view is refreshed

Then the latest vote totals should be reflected in the ranking order

--

# Business Process Analysis

Process analysis was conducted to understand stakeholder interactions and identify opportunities for optimisation.

*Process Models Produced*
--------------------------
Resident Registration Workflow

Product Browsing Workflow

Vote Casting Workflow

SME Product Management Workflow

Local Council Administration Workflow


*The process models enabled*:

Identification of decision points

Validation of business rules

Clarification of stakeholder responsibilities

Traceability between requirements and workflows


# Data Modelling
-----------------------
An Entity Relationship Model (ERD) was produced to validate solution feasibility and support development activities.

Core Entities
--

Resident

Product

SME

Vote

Area

Title


# Key Business Rules
-------
BR-01

A resident must belong to a registered area.

BR-02

A product can only be associated with one SME.

BR-03

A resident may vote only once per product.

BR-04

Product rankings must reflect cumulative vote totals.

BR-05

Mandatory registration fields must be validated before submission.

# Requirements Traceability
---

A Requirements Traceability Matrix (RTM) was created to ensure complete coverage across:

Requirements → User Stories → Acceptance Criteria → Test Cases → Validation → Sign Off

*Benefits included*:
-
Improved change impact assessment

Enhanced validation coverage

Reduced delivery risk

Improved stakeholder confidence

# Quality Assurance Alignment
---

Business requirements were validated through:

*Functional Testing*
-

Resident Registration

Product Management

Voting Functionality

Filtering Capabilities

*Non-Functional Testing*
-

Error Prevention

Error Recovery

System Status Visibility

Usability Validation

*Regression Testing*
-

Conducted throughout sprint delivery to ensure solution stability.


# Agile Delivery Approach
--

*Methodology*:

Scrum / Kanban Hybrid

*Tools*:

Trello

Discord

MySQL

PHP

GitHub

*Activities*:

Sprint Planning

Backlog Refinement

Daily Stand-Ups

Sprint Reviews

Retrospectives

# Key Business Analysis Deliverables
----

Stakeholder Register

RACI Matrix

User Stories

Acceptance Criteria

BPMN Process Models

Entity Relationship Diagram (ERD)

Requirements Traceability Matrix

Test Plan

Test Cases

Defect Analysis Documentation

# Lessons Learned

Requirements Clarity Reduces Rework

Investing time in requirements discovery and stakeholder alignment significantly reduces ambiguity during delivery.

Traceability Drives Quality

Maintaining traceability throughout the project lifecycle improves visibility, reduces risk, and supports effective change management.

Business Rules Must Be Explicit

Critical rules such as duplicate vote prevention should be documented as business requirements rather than assumed technical constraints.

Collaboration Improves Outcomes

Continuous engagement between stakeholders, developers, testers, and analysts leads to stronger solution alignment and more successful delivery outcomes.


