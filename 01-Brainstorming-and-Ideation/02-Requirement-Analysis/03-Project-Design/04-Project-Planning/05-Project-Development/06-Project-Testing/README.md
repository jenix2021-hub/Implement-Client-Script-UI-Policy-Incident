# Phase 6 – Project Testing

## Project Title

**Implement Client Script & UI Policy (Incident)**

## 1. Testing Overview

The testing phase verifies whether the Client Script and UI Policy implemented in the ServiceNow Incident application work according to the defined requirements.

Testing is performed using the Incident form in the ServiceNow Developer Instance.

## 2. Testing Objectives

The objectives of testing are:

- Verify the Client Script behaviour.
- Verify the UI Policy condition.
- Verify the Assignment group mandatory behaviour.
- Verify the Reverse if false behaviour.
- Identify configuration errors.
- Confirm that the Incident form behaves as expected.

## 3. Test Environment

The testing is performed using:

- ServiceNow Developer Instance
- Incident Management application
- Incident table
- Incident form
- Client Script
- UI Policy

## 4. Test Cases

### Test Case 1 – High Impact

**Test Condition:**

Impact = 1 - High

**Expected Result:**

The Assignment group field becomes mandatory.

**Status:**

Pass / Fail – To be recorded during testing.

---

### Test Case 2 – Impact Condition Becomes False

**Test Condition:**

Change Impact from 1 - High to another value.

**Expected Result:**

The Reverse if false behaviour is applied and the Assignment group field is no longer mandatory because of this UI Policy.

**Status:**

Pass / Fail – To be recorded during testing.

---

### Test Case 3 – Client Script

**Test Condition:**

Perform the action that triggers the configured Client Script.

**Expected Result:**

The configured Client Script behaviour executes correctly.

**Status:**

Pass / Fail – To be recorded during testing.

---

### Test Case 4 – Incident Form Validation

**Test Condition:**

Open and use an Incident form with different Impact values.

**Expected Result:**

The Incident form responds according to the configured Client Script and UI Policy.

**Status:**

Pass / Fail – To be recorded during testing.

## 5. Testing Process

The testing process is:

1. Open the ServiceNow Developer Instance.
2. Open the Incident application.
3. Open an Incident record.
4. Set Impact to **1 - High**.
5. Verify that Assignment group becomes mandatory.
6. Change the Impact value to another value.
7. Verify the Reverse if false behaviour.
8. Test the configured Client Script.
9. Verify the overall Incident form behaviour.
10. Record the test results.

## 6. Expected Testing Results

The expected results are:

| Test | Expected Result |
|---|---|
| Impact = 1 - High | Assignment group becomes mandatory |
| Impact condition false | Reverse behaviour is applied |
| Client Script trigger | Configured script behaviour executes |
| Incident form validation | Form behaves according to configuration |

## 7. Defect Identification

If any unexpected behaviour is identified during testing, the relevant ServiceNow configuration will be reviewed.

Possible areas for correction include:

- Client Script configuration
- UI Policy condition
- UI Policy Action
- Field selection
- Form configuration

## 8. Testing Evidence

Testing evidence will be collected from the ServiceNow Developer Instance.

Evidence may include:

- Incident form screenshots
- Client Script configuration
- UI Policy configuration
- UI Policy Action configuration
- Test results

## 9. Final Testing Criteria

The project will be considered successfully tested when:

- The Client Script behaves as configured.
- Impact = 1 - High makes Assignment group mandatory.
- Reverse if false behaviour works correctly.
- The Incident form operates without configuration errors.
- Test results are recorded.

## 10. Conclusion

The testing phase validates the implementation completed during the development phase.

The test cases verify the Client Script, UI Policy, Assignment group mandatory behaviour, and Reverse if false configuration.

Successful testing will prepare the project for the Project Documentation phase.
