# Cafe Collective – QA Bug Reports

## Overview

This document contains the QA bug reports identified during testing of the **Cafe Collective** application. It includes authentication, onboarding, discovery, reviews, profile, notifications, rewards, referrals, and account-management issues.

---

## Bug Report Summary

| Sr. No. | Bug ID  | App             | Bug Title                                                                                 | Status    | Assigned To | Remarks                          |
| ------: | ------- | --------------- | ----------------------------------------------------------------------------------------- | --------- | ----------- | -------------------------------- |
|       1 | Bug-001 | Cafe Collective | Back Arrow on Referral Page Is Not Functioning                                            | Fixed     | M Salman    | Issue resolved                   |
|       2 | Bug-002 | Cafe Collective | Forgot Password Navigates to OTP Verification Screen Without Sending OTP                  | Fixed     | M Salman    | Verified and working as expected |
|       3 | Bug-003 | Cafe Collective | OTP Verification Accepts Invalid OTP During Password Recovery                             | Fixed     | M Salman    | Verified and working as expected |
|       4 | Bug-004 | Cafe Collective | Password Recovery Flow Redirects to Sign In Screen Without Sending Recovery Link          | Fixed     | M Salman    | Verified and working as expected |
|       5 | Bug-005 | Cafe Collective | Deleted Google Account Email Cannot Be Reused for Email Registration                      | Fixed     | M Salman    | Verified and working as expected |
|       6 | Bug-006 | Cafe Collective | Home Dashboard Does Not Provide Clear User Guidance or Next Actions                       | Fixed     | M Salman    | Not a bug                        |
|       7 | Bug-007 | Cafe Collective | Home Dashboard Does Not Display User Activity or Submitted Reviews                        | Fixed     | M Salman    | Not a bug                        |
|       8 | Bug-008 | Cafe Collective | Statistics Cards on Profile Screen Are Non-Responsive and Provide No Detailed Information | Fixed     | M Salman    | Verified in latest build         |
|       9 | Bug-009 | Cafe Collective | No Option Available to View or Edit Submitted Reviews                                     | Fixed     | M Salman    | Verified in latest build         |
|      10 | Bug-010 | Cafe Collective | No Option Available to View Reviews Submitted by Other Users                              | Fixed     | M Salman    | Verified in latest build         |
|      11 | Bug-011 | Cafe Collective | Deleted Account Data Persists After Re-registering With the Same Google Account           | Fixed     | M Salman    | Verified in latest build         |
|      12 | Bug-012 | Cafe Collective | No Nearby Cafes Displayed for First Discovery Quest                                       | Fixed     | M Salman    | Issue resolved                   |
|      13 | Bug-013 | Cafe Collective | "Start My First Discovery" Button Is Not Working                                          | Fixed     | M Salman    | Issue resolved                   |
|      14 | Bug-014 | Cafe Collective | Error Displayed When Submitting Second Cafe Review                                        | Fixed     | M Salman    | Verified and working as expected |
|      15 | Bug-015 | Cafe Collective | Password Reset Link Opens an Unreachable Page                                             | Fixed     | M Salman    | Verified and working as expected |
|      16 | Bug-016 | Cafe Collective | Invalid Operating Hours Are Accepted                                                      | Fixed     | M Salman    | Verified and working as expected |
|      17 | Bug-017 | Cafe Collective | Friends Invited Count Is Incorrect on Manage Invitations Screen                           | Fixed     | M Salman    | Verified and working as expected |
|      18 | Bug-018 | Cafe Collective | "Mark All as Read" Button Does Not Mark Notifications as Read                             | Not Fixed | M Salman    | Reported                         |
|      19 | Bug-019 | Cafe Collective | Notification Timestamp Does Not Update                                                    | Not Fixed | M Salman    | Reported                         |
|      20 | Bug-020 | Cafe Collective | Beans Are Not Awarded After Uploading a Cafe Image                                        | Fixed     | M Salman    | Verified in latest build         |
|      21 | Bug-021 | Cafe Collective | "Share Your Achievement" Button Is Not Working for Subsequent Cafe Discoveries            | Fixed     | M Salman    | Verified in latest build         |
|      22 | Bug-022 | Cafe Collective | Uploaded Review Image Is Not Displayed in My Reviews                                      | Fixed     | M Salman    | Verified in latest build         |
|      23 | Bug-023 | Cafe Collective | Shared Referral Code Is Reported as Invalid During Sign Up                                | Not Fixed | M Salman    | Reported                         |

---

# Detailed Bug Reports

## Bug-001 — Back Arrow on Referral Page Is Not Functioning

**Module:** Referral
**Status:** Fixed
**Assigned To:** M Salman

### Description

The back arrow on the Referral page was not functioning as expected, preventing the user from navigating back to the previous screen.

### Expected Result

Tapping the back arrow should navigate the user to the previous screen.

### Actual Result

The back arrow was not responding to user interaction.

### Resolution

Issue resolved and verified.

---

## Bug-002 — Forgot Password Navigates to OTP Verification Without Sending OTP

**Module:** Authentication / Password Recovery
**Status:** Fixed
**Assigned To:** M Salman

### Description

When the user selects the Forgot Password option, the application navigates to the OTP verification screen without first sending an OTP to the registered email/contact.

### Expected Result

The application should send an OTP before navigating the user to the OTP verification screen.

### Actual Result

The OTP verification screen was displayed without an OTP being sent.

### Resolution

Fixed and verified as working as expected.

---

## Bug-003 — OTP Verification Accepts Invalid OTP During Password Recovery

**Module:** Authentication / OTP
**Status:** Fixed
**Assigned To:** M Salman

### Description

The password recovery flow accepted an invalid OTP during OTP verification.

### Expected Result

Only a valid OTP should be accepted. Invalid or expired OTPs should be rejected with an appropriate validation message.

### Actual Result

An invalid OTP was accepted during password recovery.

### Resolution

Fixed and verified as working as expected.

---

## Bug-004 — Password Recovery Redirects to Sign In Without Sending Recovery Link

**Module:** Authentication / Password Recovery
**Status:** Fixed
**Assigned To:** M Salman

### Description

The password recovery flow redirected the user back to the Sign In screen without sending the expected recovery link.

### Expected Result

The recovery link should be sent successfully and the user should be able to proceed with password recovery.

### Actual Result

The user was redirected to Sign In without receiving the recovery link.

### Resolution

Fixed and verified as working as expected.

---

## Bug-005 — Deleted Google Account Email Cannot Be Reused for Email Registration

**Module:** Authentication / Account Management
**Status:** Fixed
**Assigned To:** M Salman

### Description

After deleting an account created using Google authentication, the same email address could not be reused to create a new account through email registration.

### Expected Result

Once the previous account has been successfully deleted, the email should become available for a new registration according to the application's account-management rules.

### Actual Result

The deleted Google account email remained unavailable for email registration.

### Resolution

Fixed and verified as working as expected.

---

## Bug-006 — Home Dashboard Does Not Provide Clear User Guidance or Next Actions

**Module:** Home Dashboard
**Status:** Not a Bug
**Assigned To:** M Salman

### Description

The Home Dashboard was initially reported as not providing clear guidance or next actions for the user.

### Expected Result

Dashboard behavior should follow the approved product requirements and design.

### Actual Result

The behavior was reviewed and determined to be expected product behavior.

### Resolution

Marked as **Not a Bug**.

---

## Bug-007 — Home Dashboard Does Not Display User Activity or Submitted Reviews

**Module:** Home Dashboard / Reviews
**Status:** Not a Bug
**Assigned To:** M Salman

### Description

The Home Dashboard was initially reported as not displaying the user's activity or submitted reviews.

### Expected Result

Dashboard content should follow the approved product requirements.

### Actual Result

After review, the absence of this information was determined to be expected behavior.

### Resolution

Marked as **Not a Bug**.

---

## Bug-008 — Statistics Cards Are Non-Responsive

**Module:** Profile / Statistics
**Status:** Fixed
**Assigned To:** M Salman

### Description

Statistics cards on the Profile screen were non-responsive and did not provide detailed information when interacted with.

### Expected Result

Statistics cards should respond according to the approved functionality and provide the expected information.

### Actual Result

The cards did not respond as expected.

### Resolution

Fixed and verified in the latest build.

---

## Bug-009 — No Option to View or Edit Submitted Reviews

**Module:** Reviews
**Status:** Fixed
**Assigned To:** M Salman

### Description

The application did not provide an accessible option for users to view or manage their submitted reviews.

### Expected Result

Users should be able to access their submitted reviews according to the defined product behavior.

### Actual Result

No appropriate option was available.

### Resolution

Fixed and verified in the latest build.

---

## Bug-010 — No Option to View Reviews Submitted by Other Users

**Module:** Reviews
**Status:** Fixed
**Assigned To:** M Salman

### Description

Users could not access reviews submitted by other users for a café.

### Expected Result

Users should be able to view available reviews submitted by other users where supported by the product.

### Actual Result

No option was available to view other users' reviews.

### Resolution

Fixed and verified in the latest build.

---

## Bug-011 — Deleted Account Data Persists After Re-registration

**Module:** Account Management / Authentication
**Status:** Fixed
**Assigned To:** M Salman

### Description

After deleting an account and re-registering with the same Google account, previously associated application data persisted.

### Expected Result

Deleted account data should not incorrectly persist after account deletion and re-registration.

### Actual Result

Previously associated data remained available after re-registration.

### Resolution

Fixed and verified in the latest build.

---

## Bug-012 — No Nearby Cafes Displayed for First Discovery Quest

**Module:** Discovery
**Status:** Fixed
**Assigned To:** M Salman

### Description

No nearby cafés were displayed when the user attempted to start the first Discovery Quest.

### Expected Result

Eligible nearby cafés should be displayed so that the user can begin the first discovery.

### Actual Result

No nearby cafés were displayed, preventing the expected discovery flow.

### Resolution

Issue resolved.

---

## Bug-013 — "Start My First Discovery" Button Is Not Working

**Module:** Discovery
**Status:** Fixed
**Assigned To:** M Salman

### Description

The "Start My First Discovery" button was not initiating the expected discovery flow.

### Expected Result

Tapping the button should start the user's first Discovery Quest.

### Actual Result

The button did not initiate the expected flow.

### Resolution

Issue resolved.

---

## Bug-014 — Error Displayed When Submitting Second Cafe Review

**Module:** Reviews
**Status:** Fixed
**Assigned To:** M Salman

### Description

An error was displayed when the user attempted to submit a second café review.

### Expected Result

Users should be able to complete and submit subsequent café reviews successfully.

### Actual Result

The application displayed an error during submission of the second café review.

### Resolution

Fixed and verified as working as expected.

---

## Bug-015 — Password Reset Link Opens an Unreachable Page

**Module:** Authentication / Password Recovery
**Status:** Fixed
**Assigned To:** M Salman

### Description

The password reset link redirected the user to an unreachable page.

### Expected Result

The password reset link should open the valid password recovery page.

### Actual Result

The link opened an unreachable page.

### Resolution

Fixed and verified as working as expected.

---

## Bug-016 — Invalid Operating Hours Are Accepted

**Module:** Cafe Information / Validation
**Status:** Fixed
**Assigned To:** M Salman

### Description

The application accepted invalid operating-hour values where validation should have prevented the submission.

### Expected Result

Invalid operating hours should be rejected with appropriate validation.

### Actual Result

Invalid operating hours were accepted.

### Resolution

Fixed and verified as working as expected.

---

## Bug-017 — Friends Invited Count Is Incorrect

**Module:** Invitations
**Status:** Fixed
**Assigned To:** M Salman

### Description

The Friends Invited count displayed on the Manage Invitations screen did not accurately reflect the number of invited friends.

### Expected Result

The count should accurately represent the applicable invitations.

### Actual Result

The displayed count was incorrect.

### Resolution

Fixed and verified as working as expected.

---

## Bug-018 — "Mark All as Read" Does Not Mark Notifications as Read

**Module:** Notifications
**Status:** Not Fixed
**Assigned To:** M Salman

### Description

The "Mark All as Read" button does not mark all notifications as read.

### Expected Result

Tapping "Mark All as Read" should update all unread notifications to the read state.

### Actual Result

Notifications remain unread after using the "Mark All as Read" option.

### Resolution / Remarks

Reported. Pending fix and retest.

---

## Bug-019 — Notification Timestamp Does Not Update

**Module:** Notifications
**Status:** Not Fixed
**Assigned To:** M Salman

### Description

The timestamp displayed for notifications does not update according to the latest notification activity.

### Expected Result

Notification timestamps should accurately reflect when each notification was generated/received.

### Actual Result

The displayed timestamp does not update correctly.

### Resolution / Remarks

Reported. Pending fix and retest.

---

## Bug-020 — Beans Are Not Awarded After Uploading a Cafe Image

**Module:** Rewards / Beans / Reviews
**Status:** Fixed
**Assigned To:** M Salman

### Description

Beans were not awarded after the user uploaded a café image as part of the supported review/discovery flow.

### Expected Result

The configured bean reward should be credited after successfully completing the image-upload requirement.

### Actual Result

The expected beans were not awarded.

### Resolution

Fixed and verified in the latest build.

---

## Bug-021 — "Share Your Achievement" Does Not Work for Subsequent Discoveries

**Module:** Discovery / Achievement Sharing
**Status:** Fixed
**Assigned To:** M Salman

### Description

The "Share Your Achievement" button was not functioning for subsequent café discoveries.

### Expected Result

Users should be able to share the achievement after each eligible discovery according to product rules.

### Actual Result

The button did not work for subsequent café discoveries.

### Resolution

Fixed and verified in the latest build.

---

## Bug-022 — Uploaded Review Image Is Not Displayed in My Reviews

**Module:** Reviews / Images
**Status:** Fixed
**Assigned To:** M Salman

### Description

An image uploaded as part of a café review was successfully submitted but was not displayed when viewing the review under My Reviews.

### Expected Result

The uploaded review image should be displayed with the corresponding submitted review.

### Actual Result

The uploaded image was not visible in My Reviews.

### Resolution

Fixed and verified in the latest build.

---

## Bug-023 — Shared Referral Code Is Reported as Invalid During Sign Up

**Module:** Referral / Registration
**Status:** Not Fixed
**Assigned To:** M Salman

### Description

A referral code shared with a new user is reported as invalid when the user attempts to apply it during sign-up.

### Expected Result

A valid and active referral code should be accepted during registration and the applicable referral benefit should be processed.

### Actual Result

The shared referral code is reported as invalid during sign-up.

### Resolution / Remarks

Reported. Pending fix and retest.
