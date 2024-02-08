# git-pr-release

Create a release pull-request that describes feature pull-requests between specified two branches and simplifies release processes.

Default template is:
```mustache
{{#pulls}}
 - [{{#checked}}x{{/checked}}{{^checked}} {{/checked}}] #{{number}} {{title}} {{#assignees}}@{{login}}{{/assignees}}{{^assignees}}{{#user}}@{{login}}{{/user}}{{/assignees}}
{{/pulls}}
```
