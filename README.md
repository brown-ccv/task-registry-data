Repository with data for Behavioral Task Hub

---

To register your task data:

- Navigate to the issues tab of the repository
- Select new issue
- Select from Add New Task to register a new task, Bug Report to file a bug for any other issue/request/change and Update Task to request a change in the task data.

Add New Task:

- Please make sure to follow the specification in the comments. 
- When the issue is created the worflow will automatically create a PR for adding the file to the data folder of the repository with a comment on the issue  `We have created a PR for this issue - #[PR_Number]. The YML file for the task data will be entered into the data folder when the pull request is merged`.
- If the workflow fails with the comment `This issue has failed`  on the issue, this means either the default text for the fields 
is present or the required fields are missing. Please create a new issue with the required task details filled as per specification and the default ones removed.

YML template with specifications:

```yml
taskName: Example Task                            # [String, required]
links: 
  deployment: https://example.com                 # [String::URL, optional]
  sourceCode: https://github.com/example/task     # [String::URL, required]
  publication: https://example.com                # [String::URL, optional]
framework:
  library:                                        # [Array::String, optional]
    - LIBRARY_1 
    - LIBRARY_2
  language:                                       # [Array::String, optional]
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
