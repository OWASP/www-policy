---

title: Update Board Attendance
layout: col-sidebar

---

v2021.3.4 

### Updating Board Attendance

1. Go to the most recent board minutes found under /www-board/minutes/
3. Navigate to Call to Order - Attendance
    - Under Board Members add the name and title (in parentheses) of the board member in Markdown list format (either with `*` or with `-` in front, e.g. `* Jimmy Jim Jim (Vice Chair)`) only of the members attending >= 90% of the offical length of the meeting
    - Under Guests add the name of the guest in Markdown list format (see above)
4. Commit Changes
5. Navigate back to the /www-board/_data folder and edit attendance.yml
    - Insert a new section (copy & paste an old section)
    - Under attendees, add/replace names only of those attending >= 90% of the official length of the meeting.  These names **MUST** match previous names and may **NOT** contain titles.
    - Under guests, add/replace names of the guests
6. Commit Changes
