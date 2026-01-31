- Here’s a compact cheat-sheet of the core building-blocks and how they fit together, plus a quick “real-world” example.
  
  ---
  
  ## Key Terms
  
  * **Mailbox**
    A full user account with its own login, storage and folders.
  
    > e.g. `alice@company.com`
  
  * **Alias**
    An extra address that points into a mailbox. No separate login—mail just lands in the target inbox.
  
    > e.g. `info@company.com` → delivered to `alice@company.com`
  
  * **Distribution List (Group)**
    A list-address that fans incoming mail out to multiple mailboxes.
  
    > e.g. `support@company.com` → `alice@…`, `bob@…`, `carol@…`
  
  * **Shared Mailbox**
    A special mailbox (no password) that delegates open/read/send rights to users on their own accounts—gives a central inbox without sharing credentials.
  
    > e.g. a true “team inbox” at `info@…` that Alice/Bob/Carol open alongside their own mailboxes
  
  * **Catch-All**
    A wildcard mailbox that receives mail sent to any undefined address at your domain.
  
    > e.g. `anything@company.com` → dropped into your catch-all inbox
  
  ---
  
  ## Common Setup Patterns
  
  | Goal                                             | Pattern                         | Rough Pros & Cons                                     |
  | ------------------------------------------------ | ------------------------------- | ----------------------------------------------------- |
  | **One centralized inbox + many front-end names** | Mailbox + Aliases               | 👍 Simple, 1 licence<br>👎 Harder to assign threads   |
  | **Fan out mail to individuals**                  | Distribution List / Group       | 👍 Each keeps separate archive<br>👎 Duplicate copies |
  | **Team shares & replies from same address**      | Shared Mailbox + Send-As Rights | 👍 Central audit trail<br>👍 No shared passwords      |
  | **Catch all misspellings/unregistered names**    | Catch-All Mailbox               | 👍 Never lose mail<br>👎 Can get lots of spam         |
  
  ---
  
  ## Quick Example
  
  Your company has three people (Alice, Bob, Carol) and you want:
  
  * **Front-end addresses**
    `info@company.com`, `sales@company.com`, `support@company.com`
  
  * **Workflow**
  
    1. **Create one Shared Mailbox** `info@company.com`.
    2. **Add Aliases** on it: `sales@…`, `support@…`.
    3. **Grant Alice/Bob/Carol** Full Access + Send As on that mailbox.
    4. **Optional filters** in the shared mailbox:
  
       * Move messages with **To: sales@…** into a “Sales” folder
       * Move **To: support@…** into a “Support” folder
  
  Now:
  
  * Alice logs in as `alice@…` but opens the `info@…` inbox in her client.
  * Every “role” address lands in the same place, yet each person uses their own credentials and can see who actually sent/replied.
  
  ---
  
  With these patterns you can mix & match to match your team size, security needs, and budget. Let me know if you want step-by-step instructions for any specific platform!