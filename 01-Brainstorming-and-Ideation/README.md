# Phase 1 – Brainstorming and Ideation

## Project Title

**Implement Client Script & UI Policy (Incident)**

## 1. Introduction

This project focuses on implementing a Client Script and UI Policy in the ServiceNow Incident Management application.

The project demonstrates how ServiceNow client-side configuration can be used to improve form behaviour and enforce required field conditions dynamically.

## 2. Problem Statement

In the Incident form, certain fields need to be controlled based on the selected Impact value.

When the Impact is set to **1 - High**, the Assignment group field should become mandatory.

The project aims to implement this behaviour using ServiceNow configuration features.

## 3. Proposed Solution

The proposed solution is to configure a Client Script and a UI Policy in the ServiceNow Incident application.

The UI Policy named **High Impact Control** will control the Assignment group field when the Impact is **1 - High**.

## 4. Project Goals

- Configure the ServiceNow Incident environment.
- Implement the required Client Script.
- Create the **High Impact Control** UI Policy.
- Configure the Impact condition.
- Make the Assignment group field mandatory when Impact is 1 - High.
- Test the implemented behaviour.
- Document the project implementation and results.

## 5. Expected Outcome

The Incident form should dynamically respond to the selected Impact value.

When Impact is **1 - High**, the Assignment group field should become mandatory.

When the condition is no longer satisfied, the configured reverse behaviour should be applied.

## 6. Technologies Used

- ServiceNow
- Incident Management
- Client Script
- UI Policy
- ServiceNow Developer Instance
