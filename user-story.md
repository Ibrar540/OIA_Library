name: User story
about: A feature described from the user's point of view
title: "US-04: Reserve an Unavailable Book"
labels: user-story
assignees: ''
---
## Story
As a registered library member, I want to place a hold on a book that is currently checked out so that I am next in line to borrow it when it is returned.

## Acceptance criteria
- [ ] A "Place Hold" button is displayed on a book's detail page when all physical copies have a status of "Checked Out".
- [ ] Clicking "Place Hold" adds the member to the reservation queue and displays their current position (e.g., "You are #2 in line").
- [ ] A member cannot place multiple holds on the same book title simultaneously.
- [ ] A member with overdue books or unpaid late fees exceeding $5.00 is blocked from placing a new hold and shown a clear warning message.
- [ ] When a copy is returned and checked in by a librarian, the system automatically sends an email notification to the first member in the queue and holds the book for 48 hours.

## Notes
- **Assumptions:** User authentication and the book catalog inventory database are already implemented.
- **Questions for Stakeholder:** What is the maximum number of active holds a single library member can have at one time (e.g., 3 or 5)?
- **Related Issues:** Depends on #02 (Book Catalog Search) and #03 (Book Check-In/Check-Out Workflow).
