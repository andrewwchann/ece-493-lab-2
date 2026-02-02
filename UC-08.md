# Use Case UC-08: Validate Manuscript File Format and Size

## Goal in Context
Upload manuscript in supported formats and size limit.

## Scope
Conference Management System (CMS)

## Level
Subfunction

## Primary Actor
Author

## Secondary Actors
CMS Database

## Trigger
Author uploads a manuscript during submission.

## Success End Condition
File is accepted for upload and attached to submission.

## Failed End Condition
File is rejected with a clear error message.

## Preconditions
- Author is on the submission page.

## Main Success Scenario
1. Author selects a manuscript file to upload.
2. System checks the file type is supported.
3. System checks the file size is within the limit.
4. System uploads and attaches the file to the submission.

## Extensions
- **2a** Unsupported file type
  - **2a1** System rejects the file and displays an error.
- **3a** File exceeds size limit
  - **3a1** System rejects the file and displays an error.

## Related Information
- **Priority**: High
- **Frequency**: Medium
