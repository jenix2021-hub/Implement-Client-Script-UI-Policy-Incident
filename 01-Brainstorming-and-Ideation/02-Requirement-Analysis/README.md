# Phase 2 – Requirement Analysis

## Project Title

**Implement Client Script & UI Policy (Incident)**

## 1. Requirement Overview

The project requires the implementation of client-side behaviour and form control in the ServiceNow Incident application.

The main requirement is to dynamically control the Assignment group field based on the selected Impact value.

## 2. Functional Requirements

The system should satisfy the following functional requirements:

1. The project must use the ServiceNow Incident application.
2. The Incident form must contain the Impact field.
3. The Incident form must contain the Assignment group field.
4. A UI Policy named **High Impact Control** must be created.
5. The UI Policy condition must check whether Impact is **1 - High**.
6. When Impact is **1 - High**, the Assignment group field must become mandatory.
7. The UI Policy must have **Reverse if false** enabled.
8. The configured behaviour must be tested when the Impact value changes.

## 3. Client Script Requirement

A Client Script is required as part of the project to demonstrate client-side form behaviour in ServiceNow.

The Client Script should be configured for the appropriate Incident form event according to the project implementation requirements.

## 4. UI Policy Requirement

The UI Policy must be configured with the following details:

| Property | Required Value |
|---|---|
| Name | High Impact Control |
| Table | Incident |
| Condition | Impact is 1 - High |
| Reverse if false | True |
| Field affected | Assignment group |
| Mandatory | True |

## 5. Input

The primary input for the configured behaviour is the **Impact** value selected by the user on the Incident form.

The important condition is:

**Impact = 1 - High**

## 6. Expected System Behaviour

When the user selects **1 - High** in the Impact field:

- The Assignment group field should become mandatory.
- The Incident form should enforce the configured field behaviour.

When the Impact condition becomes false:

- The reverse behaviour configured in the UI Policy should be applied.
- The Assignment group field should no longer remain mandatory because of this UI Policy.

## 7. Non-Functional Requirements

The implementation should:

- Work within the ServiceNow Incident application.
- Follow ServiceNow configuration standards.
- Be simple to test and demonstrate.
- Produce consistent form behaviour.
- Be properly documented.

## 8. Tools and Technologies

- ServiceNow Developer Instance
- ServiceNow Incident Management
- Client Script
- UI Policy
- Incident Form

## 9. Requirement Summary

The project will implement and test a ServiceNow Incident form configuration where the Assignment group field becomes mandatory when the Impact is set to **1 - High**.

The configuration will use the **High Impact Control** UI Policy and the required Client Script implementation.
