---
name: Add New Task
about: Register new tasks to hub
title: Register [Task Name]
labels: data request
assignees: ''

---

**Instructions**
Fill in the below yml template as per the specification in the comments.
You can view the preview side-by-side for the yml below you are editing and see changes reflected in real-time as you edit.
```yml
# YML template does not require Strings(also URL) and Boolean to be in quotes.
# Please add a valid URL starting with https.
taskName: Example Task                            # [String, required] 
about: 
  description: A short description of the task    # [String, required]
  deployment: https://example.com                 # [String::URL, optional]
  sourceCode: 
    access: private/public                        # [String, required] Stating if the GitHub repository is private or public.
    link: https://github.com/example/task         # [String::URL, optional] If the repository is public, provide URL.
  publication: https://example.com                # [String::URL, optional]
framework:
  - name: FRAMEWORK_1                             # [Array::String, optional]
    link: LINK_TO_FRAMEWORK_1                     # [String::URL, optional] 
  - name: FRAMEWORK_2                             # [Array::String, optional]
    link: LINK_TO_FRAMEWORK_2                     # [String::URL, optional]
language:                                         # [Array::String, optional]
  - LANGUAGE_1
  - LANGUAGE_2
lab:                                              # List of the labs who collaborated.
  - name:                                           # [String, required]
    institution:                                    # [String, required]
    principalInvestigator:                          # [String, optional]
    developers:                                     # [Array::String, optional]
      - DEVELOPER_1
      - DEVELOPER_2
    website: https://example.com                    # [String::URL, optional]
platform:                                         # [Boolean, optional]
  desktop:
    windows: false
    linux: false
    mac: false
  mobile:
    ios: false
    android: false
features:                                         # [Boolean, optional]
  electron: false
  browser: false
  docker: false
  eegTrigger: false
  mturk: false
tags:                                             # [Array::String, optional]
  - TAG_1
  - TAG_2
  - TAG_3
  - TAG_4
```
