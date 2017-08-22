# SPMIssue

`swift build` fails with:

```
Compile Swift Module 'SPMIssueReport' (3 sources)
/Users/antondomashnev/Work/SPMIssueReport/Sources/Child+Functions.swift:11:16: error: 'Child' is not a member type of 'Base'
extension Base.Child {
          ~~~~ ^
/Users/antondomashnev/Work/SPMIssueReport/Sources/Child+Functions.swift:11:16: error: 'Child' is not a member type of 'Base'
extension Base.Child {
          ~~~~ ^
/Users/antondomashnev/Work/SPMIssueReport/Sources/Child+Functions.swift:11:16: error: 'Child' is not a member type of 'Base'
extension Base.Child {
          ~~~~ ^
<unknown>:0: error: build had 1 command failures
```

But if rename the `Child.swift` into something like `Child+Base.swift` it builds without errors.
