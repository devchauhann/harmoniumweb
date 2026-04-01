name: Feature Request
description: Suggest an idea for Web Harmonium
title: "[FEATURE] "
labels: ["enhancement"]
assignees: []

body:
  - type: markdown
    attributes:
      value: |
        Thanks for suggesting a feature! Help us understand your idea.

  - type: textarea
    id: description
    attributes:
      label: Feature Description
      description: Clearly describe the feature you'd like
      placeholder: What would you like to add?
    validations:
      required: true

  - type: textarea
    id: motivation
    attributes:
      label: Motivation & Benefit
      description: Why is this feature valuable? How does it help users?
      placeholder: |
        This feature would...
        Users would benefit because...
    validations:
      required: true

  - type: textarea
    id: examples
    attributes:
      label: Use Case Examples
      description: Show how users would interact with this feature
      placeholder: |
        Example 1: A user could...
        Example 2: This would allow...
    validations:
      required: true

  - type: textarea
    id: alternatives
    attributes:
      label: Alternative Solutions
      description: Any other ways to solve this problem?
      placeholder: |
        Alternative approach 1: ...
        Alternative approach 2: ...

  - type: dropdown
    id: impact
    attributes:
      label: Impact
      description: How important is this feature?
      options:
        - Critical
        - High
        - Medium
        - Low
    validations:
      required: true

  - type: textarea
    id: additional
    attributes:
      label: Additional Context
      description: Any sketches, mockups, or references?
      placeholder: Add links, images, or other context

  - type: checkboxes
    id: checklist
    attributes:
      label: Checklist
      options:
        - label: I've checked existing feature requests
          required: true
        - label: This feature aligns with Web Harmonium's goals
          required: true
        - label: I've provided clear use cases
          required: true
