name: Bug Report
description: Report a bug to help us improve Web Harmonium
title: "[BUG] "
labels: ["bug"]
assignees: []

body:
  - type: markdown
    attributes:
      value: |
        Thanks for reporting a bug! Please fill out the details below to help us investigate.

  - type: textarea
    id: description
    attributes:
      label: Description
      description: Clearly describe the bug
      placeholder: What happened?
    validations:
      required: true

  - type: textarea
    id: reproduction
    attributes:
      label: Steps to Reproduce
      description: Detailed steps to reproduce the bug
      placeholder: |
        1. ...
        2. ...
        3. ...
      value: |
        1. 
        2. 
        3. 
    validations:
      required: true

  - type: textarea
    id: expected
    attributes:
      label: Expected Behavior
      description: What should happen?
      placeholder: Describe expected behavior
    validations:
      required: true

  - type: textarea
    id: actual
    attributes:
      label: Actual Behavior
      description: What actually happens?
      placeholder: Describe actual behavior
    validations:
      required: true

  - type: dropdown
    id: browser
    attributes:
      label: Browser
      description: Which browser are you using?
      options:
        - Chrome
        - Firefox
        - Safari
        - Edge
        - Other
    validations:
      required: true

  - type: textarea
    id: environment
    attributes:
      label: Environment
      description: |
        Provide environment details
      placeholder: |
        OS: macOS 14
        Browser Version: Chrome 120
        Screen Size: 1920x1080
        Device: Desktop / Mobile / Tablet
    validations:
      required: true

  - type: textarea
    id: screenshots
    attributes:
      label: Screenshots or Recording
      description: Add screenshots or video if applicable
      placeholder: Drag and drop images or paste links

  - type: textarea
    id: console
    attributes:
      label: Console Errors
      description: Any errors in browser console? (F12 → Console tab)
      placeholder: Paste console errors here

  - type: textarea
    id: additional
    attributes:
      label: Additional Context
      description: Any other relevant information?
      placeholder: Add any other context here

  - type: checkboxes
    id: checklist
    attributes:
      label: Checklist
      options:
        - label: I've checked existing issues
          required: true
        - label: I can reproduce the bug
          required: true
        - label: I've provided all relevant details
          required: true
