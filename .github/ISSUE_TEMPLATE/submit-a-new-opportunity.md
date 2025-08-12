---
name: Submit a New Opportunity
about: Use this form to suggest a new event, fellowship, or opportunity.
title: "\U0001F195 New Opportunity Submission: [Insert Program or Event Name]"
labels: new opportunity
assignees: ''

---

name: 📝 Submit a New Opportunity
description: Use this form to suggest a new conference, fellowship, job, or opportunity for the IGF Commons repository.
title: "🆕 New Opportunity Submission: "
labels: ["new opportunity"]
assignees: []

body:
  - type: input
    id: title
    attributes:
      label: Program or Event Name
      placeholder: e.g., ICANN Fellowship
    validations:
      required: true

  - type: input
    id: link
    attributes:
      label: Link to Opportunity
      placeholder: https://example.com
    validations:
      required: true

  - type: dropdown
    id: type
    attributes:
      label: Type of Opportunity
      options:
        - Conference
        - Fellowship
        - Mentorship
        - Job/Internship
        - Funding
        - Success Story
    validations:
      required: true

  - type: input
    id: region
    attributes:
      label: Region (Optional)
      placeholder: e.g., Global, Africa, Europe

  - type: input
    id: deadline
    attributes:
      label: Application Deadline (Optional)
      placeholder: e.g., September 15, 2025

  - type: textarea
    id: notes
    attributes:
      label: Additional Info or Comments
      placeholder: Add any context, notes, or clarifications you'd like us to know.
