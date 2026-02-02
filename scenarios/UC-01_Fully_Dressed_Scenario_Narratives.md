# UC-01 Fully Dressed Scenario Narratives

## Main Success Scenario (Happy Path)

A public user visits the Conference Management System (CMS) and decides they want access to CMS features such as submitting papers or registering for the conference. The user selects the option to register. The CMS responds by displaying the registration form. The user enters the required registration information and submits the form.

After the form is submitted, the CMS validates the information provided, including the email address and password. Since all information meets the system’s requirements, the CMS creates the user account and stores the account details in the CMS database. The CMS then redirects the user to the login page, indicating that registration was successful and allowing the user to log in using the newly created account.

---

## Alternative Path 5a: Email Invalid or Already Registered

The user completes the registration form and submits it. The CMS validates the email address and determines that it is either invalid in format or already associated with an existing account.

The CMS does not create a new account and instead displays an error message indicating that one or more fields are invalid. The user remains on the registration page and is prompted to correct the email address or provide a different one before attempting to submit the form again.

---

## Alternative Path 5b: Password Does Not Meet Security Requirements

The user enters all required registration information, including a password, and submits the form. The CMS evaluates the password and determines that it does not meet the defined security requirements.

The CMS rejects the registration attempt and displays an error message indicating that the password is invalid. The user stays on the registration page and is given the opportunity to enter a new password that satisfies the security requirements and resubmit the form.
