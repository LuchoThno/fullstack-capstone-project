---
name: User Story
about: Create a new user story for the product backlog
title: "[USER STORY] "
labels: user-story, backlog
assignees: ""
---

# User Story

## Story Summary
Short description of the user story.

---

## User Story

**As a** [type of user]  
**I need** [some goal / functionality]  
**So that** [some reason / benefit]

---

## Business Value

Describe the value this feature provides to the user or the business.

Examples:
- Improve user engagement
- Enable core functionality of the platform
- Reduce operational friction

---

## Scope

### In Scope
- List the elements included in this story
- Backend functionality
- Frontend components
- Database updates

### Out of Scope
- Features not included in this story
- Future enhancements

---

## Details and Assumptions

Document important information about the feature.

- User must be authenticated
- Data must be stored in the database
- API must follow REST conventions
- UI must follow the design system

Dependencies:

- Authentication service
- Database connection
- Existing API endpoints

---

## Acceptance Criteria

```gherkin
Feature: [Feature name]

Scenario: Successful operation
Given [initial context]
And [additional context]
When [action performed]
Then [expected result]

Scenario: Error condition
Given [initial context]
When [invalid action]
Then [error message or failure state]
