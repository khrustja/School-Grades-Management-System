# SRS update v1.1

## Version change
- Previous version: **1.0**
- Current version: **1.1**

## Change log
- Added use case **Export Student Report to CSV**
- Added use case **Filter Students by Class**
- Added use case **View Top Student in Class**
- Added use case **Add Teacher Comment to Grade**
- Added CI/CD workflows for personal feature branches

## New functional requirements
- **FR-31** The system shall allow an authenticated user to export a selected student's report card to CSV format.
- **FR-32** The system shall allow authenticated users to filter students by class and search by first or last name.
- **FR-33** The system shall calculate and display the top student in a selected class for authenticated staff users based on average grade.
- **FR-34** The system shall allow a teacher or administrator to add or edit a textual comment for a grade on a dedicated page.

## New use cases
### UC-31 Export Student Report to CSV
**Actors:** User, Administrator

**Main flow:**
1. User opens a student report.
2. User presses **Export CSV**.
3. System generates a CSV file.
4. Browser downloads the file.

### UC-32 Filter Students by Class
**Actors:** User, Administrator

**Main flow:**
1. Actor opens the students page.
2. Actor enters a name fragment and/or selects a class.
3. System refreshes the list according to filters.

### UC-33 View Top Student in Class
**Actors:** User, Administrator

**Main flow:**
1. Actor opens the reports page.
2. Actor selects a class.
3. System shows the top student for this class and the student's average grade.

### UC-34 Add Teacher Comment to Grade
**Actors:** User, Administrator

**Main flow:**
1. Actor opens a grade.
2. Actor selects **Edit comment**.
3. Actor enters a comment and saves changes.
4. System stores the comment and displays it in grade details and reports.
