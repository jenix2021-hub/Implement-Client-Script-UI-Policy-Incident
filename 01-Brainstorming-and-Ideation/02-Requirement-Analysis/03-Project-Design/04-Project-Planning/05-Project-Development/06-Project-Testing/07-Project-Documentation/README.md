# Phase 7 – Project Documentation

## Project Title

**Implement Client Script & UI Policy (Incident)**

## 1. Project Overview

This project demonstrates the implementation of a Client Script and UI Policy in the ServiceNow Incident Management application.

The project focuses on improving Incident form behaviour by dynamically controlling the Assignment group field based on the selected Impact value.

## 2. Problem Statement

Incident records may require specific fields to be completed depending on the severity or impact of the incident.

To improve data consistency, the Assignment group field needs to become mandatory when the Impact is set to **1 - High**.

## 3. Proposed Solution

The project uses ServiceNow Client Script and UI Policy functionality.

A UI Policy named **High Impact Control** is configured on the Incident table.

When:

**Impact = 1 - High**

the:

**Assignment group**

field becomes mandatory.

The **Reverse if false** option is enabled to reverse the configured behaviour when the condition is no longer satisfied.

## 4. Technologies Used

- ServiceNow
- ServiceNow Developer Instance
- Incident Management
- Client Script
- UI Policy
- UI Policy Action
- GitHub

## 5. Project Requirements

The project requires:

- Incident table
- Incident form
- Impact field
- Assignment group field
- Client Script
- UI Policy
- UI Policy Action

## 6. UI Policy Configuration

### UI Policy Name

**High Impact Control**

### Table

**Incident**

### Condition

**Impact is 1 - High**

### UI Policy Action

**Assignment group → Mandatory**

### Reverse if False

**True**

## 7. Client Script

A Client Script is implemented on the Incident form to provide client-side functionality according to the project requirements.

The Client Script is configured for the required Incident form event and is tested to verify its behaviour.

## 8. System Workflow

The overall workflow is:

```text
User opens Incident
        ↓
User selects Impact
        ↓
ServiceNow evaluates condition
        ↓
Impact = 1 - High?
        ↓
       YES
        ↓
Assignment group becomes Mandatory
        ↓
User provides Assignment group
        ↓
Incident can be completed
