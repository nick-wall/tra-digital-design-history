---
title: First designs for a minimum viable service
date: 2022-12-21
screenshots:
  items:
    - text: Referrals list
      src: list.png
    - text: View referral (employer)
      src: details.png
    - text: View referral (member of public)
      src: details--public.png
---

{% from "email/macro.njk" import appEmail with context %}

At the moment, people make [referrals of serious misconduct by a teacher by sending a form by email](/refer-serious-misconduct-by-a-teacher-in-england/mvp-eligibility/).

Caseworkers access a shared mailbox to open up new referrals. They open up the referral and move the details into the Teacher Misconduct System (TMS).

As we’re going to allow people to make referrals using an online form, we need to give caseworkers a way to access the referrals.

## How it works

### New referrals

When someone makes a referral, an email notification will be sent to the shared mailbox.

<!-- markdownlint-disable MD025 MD001 -->
{{ appEmail({
  subject: "Jo Swan has been referred",
  content: "

Jo Swan has been referred for serious misconduct by a teacher.

View referral:

((link))
  "
}) }}

To keep details secure, they’ll not be attached to the email.

Instead, caseworkers will click a link to view the referral which will be accessed through a DfE Sign-in account.

### Viewing a referral

Caseworkers will be able to click a link to view the referral.

### Copying the details into the TMS

Caseworkers can view all the details of the referral and copy across any details into the TMS.

They can download all the files and evidence provided in the referral by clicking ‘Download all files’ at the top of the page.

### Viewing the list of referrals

Caseworkers can also view a list of referrals ordered by most recent.

## Further considerations

We want to consider:

- how to make it easier for caseworkers to understand what an uploaded file contains
- how to prevent caseworkers from having to move data manually into the TMS
