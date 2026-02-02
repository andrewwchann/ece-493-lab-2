# UC-02 Fully Dressed Scenario Narratives

## Main Success Scenario (Happy Path)

A public user has completed the registration form on the Conference Management System (CMS) and submits the form with an email address and password. The CMS receives the submitted credentials and begins validation.

The CMS first checks the format of the email address and determines that it is syntactically valid. The CMS then checks the system database to confirm that the email address is not already registered. After confirming uniqueness, the CMS evaluates the submitted password and determines that it meets the password security standards.

Because both the email address and password are valid, the CMS confirms that the credentials are acceptable and allows the registration process to proceed. Control is returned to the registration workflow so the user account can be created and the user can continue toward successful registration.

---

## Alternative Path 2a: Email Address Format Is Invalid

The user submits the registration form with an email address and password. The CMS attempts to validate the email address and determines that the email address format is invalid.

Since the email format does not meet validation requirements, the CMS halts the credential validation process. The CMS does not proceed to check email uniqueness or password validity. Instead, the CMS displays an error message informing the user that one or more fields are invalid. The registration process pauses, allowing the user to correct the email address and resubmit the form.

---

## Alternative Path 3a: Email Address Already Registered

The user submits the registration form with an email address that is syntactically valid. The CMS checks the database and determines that the email address is already associated with an existing account.

Because the email address is not unique, the CMS rejects the credential validation. The CMS displays an error message indicating that one or more fields are invalid. The registration process does not continue, and the user is prompted to provide a different email address before attempting to submit the form again.

---

## Alternative Path 4a: Password Does Not Meet Security Standards

The user submits the registration form with a valid and unique email address and a password. The CMS evaluates the password and determines that it does not meet the required password security standards.

As a result, the CMS rejects the credentials and displays an error message indicating that one or more fields are invalid. The CMS allows the user to remain on the registration page so the user can enter a new password that satisfies the security requirements and resubmit the form.
