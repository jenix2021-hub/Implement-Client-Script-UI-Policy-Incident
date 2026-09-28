# Phase 4 – Project Planning

## Project Title

**Implement Client Script & UI Policy (Incident)**

## 1. Planning Overview

The project planning phase defines the activities, resources, implementation sequence, testing activities, documentation, and final demonstration required to complete the project.

The project will be implemented using the ServiceNow Incident application.

## 2. Project Objectives

The project aims to:

- Implement a Client Script in ServiceNow.
- Create and configure a UI Policy.
- Configure the UI Policy named **High Impact Control**.
- Apply the UI Policy to the Incident table.
- Configure the condition **Impact is 1 - High**.
- Make the Assignment group field mandatory when the condition is true.
- Enable Reverse if false.
- Test the configured behaviour.
- Document the implementation.
- Prepare the final project demonstration.

## 3. Project Development Plan

| Activity | Description |
|---|---|
| Requirement Review | Understand the project requirements |
| Design | Plan the Client Script and UI Policy configuration |
| Development | Implement the ServiceNow configurations |
| Testing | Verify the configured behaviour |
| Documentation | Record implementation and testing details |
| Demonstration | Demonstrate the completed project |

## 4. Implementation Plan

### Step 1 – ServiceNow Environment

Use the authorized ServiceNow Developer Instance for project development.

### Step 2 – Incident Application

Open the Incident application and identify the required Incident form and fields.

### Step 3 – Client Script

Create and configure the required Client Script according to the project requirements.

### Step 4 – UI Policy

Create a UI Policy with the following configuration:

**Name:** High Impact Control

**Table:** Incident

**Condition:** Impact is 1 - High

**Reverse if false:** True

### Step 5 – UI Policy Action

Configure the Assignment group field as mandatory when the UI Policy condition is satisfied.

### Step 6 – Verification

Open an Incident record and verify the configured form behaviour.

## 5. Testing Plan

The following scenarios will be tested:

### Test Case 1

**Condition:** Impact = 1 - High

**Expected Result:** Assignment group becomes mandatory.

### Test Case 2

**Condition:** Impact is not 1 - High

**Expected Result:** Reverse if false behaviour is applied.

### Test Case 3

**Condition:** Client Script trigger occurs

**Expected Result:** The configured Client Script behaviour executes correctly.

## 6. Required Resources

The project requires:

- ServiceNow Developer Instance
- Web browser
- Internet connection
- Incident Management application
- ServiceNow configuration access
- GitHub repository
- Project documentation

## 7. Project Deliverables

The planned deliverables are:

1. Client Script configuration.
2. UI Policy configuration.
3. Testing evidence.
4. Project documentation.
5. Phase-wise GitHub repository.
6. Project demonstration video.

## 8. Risk Management

Possible implementation issues include:

- Incorrect Client Script configuration.
- Incorrect UI Policy condition.
- Incorrect field selection.
- Unexpected form behaviour.
- Configuration errors during testing.

These issues will be identified and corrected during the testing phase.

## 9. Project Completion Criteria

The project will be considered complete when:

- Client Script is implemented.
- UI Policy is implemented.
- High Impact condition works correctly.
- Assignment group becomes mandatory when required.
- Reverse behaviour works correctly.
- Testing is completed.
- Documentation is prepared.
- Final demonstration is recorded.

## 10. Project Timeline

The project will be completed through the following sequence:

1. Brainstorming and Ideation
2. Requirement Analysis
3. Project Design
4. Project Planning
5. Project Development
6. Project Testing
7. Project Documentation
8. Project Demonstration

## 11. Conclusion

The Project Planning phase establishes the activities, resources, implementation process, testing approach, deliverables, and completion criteria required to successfully develop the ServiceNow Incident project.

The next phase will focus on the actual Project Development and implementation activities.
