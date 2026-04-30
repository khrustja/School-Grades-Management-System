# Class diagram impact assessment

The four new features do **not** require changes to the domain class diagram.

## Why
- **Export Student Report to CSV** uses existing `Student`, `Grade`, `Teacher`, `Subject`.
- **Filter Students by Class** uses existing `Student` properties.
- **View Top Student in Class** calculates a report from existing grades.
- **Add Teacher Comment to Grade** uses the already existing `Grade.Comment` field.

## What changed instead
Only UI-level helper models were added:
- `TopStudentInClassViewModel`
- `GradeCommentViewModel`
