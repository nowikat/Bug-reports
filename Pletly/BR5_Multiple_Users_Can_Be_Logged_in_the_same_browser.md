## Bug Report: Multiple Users Logged in Same Browser

### Description:
It is possible to be logged in as multiple users within the same browser, which causes various issues, such as:
- Posts added by User A are incorrectly displayed as being added by User B on the feed.
- Profile updates, such as changing the profile picture for User A, fail with a "Forbidden" error.

### Steps to Reproduce:
1. Open a browser and log in as User A.
2. In the same browser, open a new tab or window and log in as User B.
3. While logged in as User A:
    - a. Navigate to the feed and add a new post.
    - b. Attempt to update User A's profile picture.

### Expected Result:
- Posts and profile updates should be performed under the currently logged-in user.
- No errors should occur when updating the user's profile.

### Actual Result:
- Posts added while logged in as User B are incorrectly attributed to User A.
- Attempting to update User A's profile picture results in a "Forbidden" error.

### Additional Info:
- The new post is added by the user who was logged in last.
- Only after clicking "refresh" does the user session update to the most recently logged-in user.
- However, if we don't click 'refresh,' it's possible to navigate the page and switch tabs, and the session does not fully refresh for the last logged user.

### Environment:
- **Browser:** Chrome
- **Operating System:** Win 11

### Priority: 
- 🟢 **High**

### Severity: 
- 🟥 **Major**
