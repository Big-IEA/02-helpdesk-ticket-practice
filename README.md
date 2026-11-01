# Project: Helpdesk Ticket Practice (Zoho Desk + Microsoft Entra ID)

## Goal
Practise the full ticket cycle used in IT support: log, diagnose, fix,
document and close, with the real fixes done in an Entra ID lab tenant.

## Environment
- Zoho Desk (free trial) as the ticketing system
- Microsoft Entra ID lab tenant (Azure free account)

## Tickets completed
| # | Ticket | Type | Fix done in |
|---|--------|------|-------------|
| 101 | User cannot sign in | Password reset | Entra ID lab |
| 102 | Account locked after failed sign-ins | Lockout | Entra ID lab |
| 103 | Create account and add new hire to Finance-Team | Joiner | Entra ID lab |
| 104 | Printer shows offline | Hardware (simulated scenario) | Documented only |
| 105 | Disable account for departing employee | Leaver | Entra ID lab |

## Example: Leaver process (#105)
1. Received the request and verified it came from the employee's manager
2. Blocked sign-in on the account in Entra ID
3. Removed the user from the Finance-Team group
4. Confirmed: account shows Disabled and 0 group memberships;
   Finance-Team shows 3 remaining members
5. Kept the account (not deleted) so data can be handed over
6. Wrote a private note and closed the ticket

![Ticket list](ticket-list.png)
![Account disabled](entra-disabled.png)
![Finance-Team members](finance-team-members.png)

## What I learned
- Every ticket needs a clear note: what I verified, found, did, and the result
- Leavers are disabled first and deleted later, not deleted straight away
- Always confirm a change in the system before closing the ticket

## Skills shown
Ticketing, user lifecycle (joiner/leaver), Entra ID, group management,
troubleshooting, documentation
