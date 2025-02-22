---
title: Handling incomplete tasks
date: 2023-02-13
---

We allow referrers to partially complete a task.

For example, a referrer may enter their name and leave without filling out their job title and phone number.

At the moment, if a user clicks a partially completed task they’ll be taken through the flow from the start with any answers prefilled. This is long-winded and does not give users an overview of the task.

We also allow users to review their referral before it’s complete. This allows them to check their answers without clicking into each task. But we do not highlight which tasks are incomplete making it harder to understand what needs doing.

Finally, if the user tries to send an incomplete referral, they’ll see an error message that says ‘Complete all sections of the referral’. But this is long-winded because users have to perform an action to see what’s missing.

So we made changes to address these problems.

## How it works

If the user clicks a task that’s not been started, they’ll be taken to the first question in the task.

If the user clicks a task that’s partially complete, they’ll be taken to the check answers page. It will show:

- a blue highlighted summary list with any questions that have been answered
- a message that says ‘You must complete your details before sending a referral’ (or similar)
- a ‘Complete your details’ (or similar) button which when clicked will take users to the next unanswered question

![Check answers - incomplete](check-answers-incomplete.png)

If the user clicks a task that’s complete, they’ll be taken to the check answers page. It will show:

- a summary list with the questions and answers
- radio buttons to mark the task as complete or incomplete
- a ‘Save and continue’ button which when clicked takes the user back to the task list

![Check answers page - complete](check-answers-complete.png)

The same experience applies on the review page.

![Review page - incomplete](review-page-incomplete.png)

If the user tries to send an incomplete referral, a list of errors will show at the top of the page for each incomplete task. Clicking each will anchor the user down to the relevant summary list.

![Review page - error](review-page-error.png)
