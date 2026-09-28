# Phase 5 – Project Development

## Project Title

**Implement Client Script & UI Policy (Incident)**

## 1. Development Overview

The Project Development phase focuses on implementing the required Client Script and UI Policy in the ServiceNow Incident application.

The implementation converts the requirements, design, and project plan into a working ServiceNow configuration.

## 2. Development Environment

The project is developed using:

- ServiceNow Developer Instance
- ServiceNow Incident Management
- Incident table
- Incident form
- Client Script
- UI Policy
- UI Policy Action

## 3. Incident Form

The Incident form is used as the main interface for implementing and testing the project functionality.

The important fields used in this project are:

- Impact
- Assignment group

## 4. Client Script Implementation

A Client Script is implemented on the Incident form to provide client-side behaviour.

The Client Script is configured according to the required Incident form event and project requirements.

The Client Script is tested to verify that the configured client-side functionality executes correctly.

## 5. UI Policy Implementation

A UI Policy is created for the Incident table.

### UI Policy Configuration

**Name:** High Impact Control

**Table:** Incident

**Condition:** Impact is 1 - High

**Reverse if false:** True

## 6. UI Policy Action

A UI Policy Action is configured for the Assignment group field.

The field is configured as:

**Mandatory = True**

Therefore, when the UI Policy condition is satisfied, the Assignment group field becomes mandatory.

## 7. Implementation Logic

The main implementation flow is:

```text
Open Incident Form
        ↓
Select or change Impact
        ↓
Check UI Policy condition
        ↓
Is Impact = 1 - High?
        ↓
       YES
        ↓
Assignment group becomes Mandatory
        ↓
User provides Assignment group
        ↓
Incident can be completed
