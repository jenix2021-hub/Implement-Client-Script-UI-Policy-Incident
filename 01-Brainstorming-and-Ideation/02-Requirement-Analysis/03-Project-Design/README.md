# Phase 3 – Project Design

## Project Title

**Implement Client Script & UI Policy (Incident)**

## 1. Design Overview

The project design defines how the Client Script and UI Policy will be configured in the ServiceNow Incident application.

The design focuses on controlling the Assignment group field based on the Impact value selected in the Incident form.

## 2. ServiceNow Application

The implementation will be performed in the:

**Incident Management application**

The Incident form will be used to configure and test the required behaviour.

## 3. UI Policy Design

A UI Policy named:

**High Impact Control**

will be created on the Incident table.

### UI Policy Configuration

| Property | Configuration |
|---|---|
| Name | High Impact Control |
| Table | Incident |
| Condition | Impact is 1 - High |
| Reverse if false | True |
| Active | True |

## 4. UI Policy Action

A UI Policy Action will be created for the:

**Assignment group**

field.

The field will be configured as:

**Mandatory = True**

When the UI Policy condition is satisfied, the Assignment group field will therefore become mandatory.

## 5. Condition Design

The main condition is:

**Impact is 1 - High**

The system will evaluate the selected Impact value on the Incident form.

### When condition is true

If:

**Impact = 1 - High**

then:

**Assignment group = Mandatory**

### When condition is false

If the Impact is changed to a value other than **1 - High**, the reverse behaviour will be applied because **Reverse if false** is enabled.

## 6. Client Script Design

A Client Script will also be implemented as part of the project.

The Client Script will demonstrate client-side control of the Incident form and support the required project behaviour.

The script will be configured according to the appropriate Incident form event required during implementation and testing.

## 7. Form Behaviour Design

The designed flow is:

1. User opens an Incident form.
2. User selects an Impact value.
3. ServiceNow evaluates the configured condition.
4. If Impact is **1 - High**, the Assignment group becomes mandatory.
5. If the condition becomes false, the reverse configuration is applied.
6. The form behaviour is tested to confirm the expected result.

## 8. Implementation Components

The project will contain the following ServiceNow components:

- Incident table
- Incident form
- Client Script
- UI Policy
- UI Policy Action
- Assignment group field
- Impact field

## 9. Testing Design

The implementation will be tested using different Impact values.

### Test Case 1

**Impact:** 1 - High

**Expected Result:** Assignment group becomes mandatory.

### Test Case 2

**Impact:** A value other than 1 - High

**Expected Result:** Reverse behaviour is applied and the Assignment group is no longer mandatory because of this UI Policy.

## 10. Expected Design Outcome

The final design will provide dynamic Incident form behaviour based on the selected Impact value.

The configuration will demonstrate how ServiceNow Client Scripts and UI Policies can be used together to control form behaviour.
