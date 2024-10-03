# Bug Report: Unable to Complete Registration Process due to Error in 'Complete Your Account Setup' Step

## Summary
Users are unable to complete the registration process due to an error that occurs in the 'Complete Your Account Setup' step.

## Severity
🔴 High

## Priority
🔴 High

## Steps to Reproduce
1. On the welcome screen, tap on the 'Sign Up' button.
2. Fill in the 'Create Account' section with valid registration details and proceed.
3. Tap on the 'Get Started' button.
4. Enter a valid first name and last name in the 'Complete Your Account Setup' step, then tap 'Next'.

## Expected Result
The registration process should proceed to the next step, allowing the user to complete account setup without any errors.

## Actual Result
An error message appears after entering a valid first name and last name:
"ERROR: Cannot read properties of undefined reading 'to...'"
This error prevents the user from completing the registration process.


**Environment**:
  
  - **Pletly Pal**, Build 667
  - **Operating System**: Android 11
  - **Device**: Xiaomi Redmi Note 8 Pro

