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
# YML template does not require Strings and Boolean to be in quotes, also URL.
taskName: Example Task                            # [String, required] 
links: 
  deployment: https://example.com                 # [String::URL, optional]
  sourceCode: https://github.com/example/task     # [String::URL, required]
  publication: https://example.com                # [String::URL, optional]
framework:
  - name: FRAMEWORK_1                             # [Array::String, optional]
    link: LINK_TO_FRAMEWORK_1                     # [String::URL, optional] 
  - name: FRAMEWORK_2                             # [Array::String, optional]
    link: LINK_TO_FRAMEWORK_2                     # [String::URL, optional]
language:                                         # [Array::String, optional]
  - LANGUAGE_1
  - LANGUAGE_2
lab:
  name:                                           # [String, required]
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
