# Follow Ledger

An Instagram follower tracker that runs entirely in the browser. It shows:

- **Don't follow you back**: accounts you follow that don't follow you
- **Unfollowed you**: people who followed you in an earlier export but not the latest one
- **You don't follow back** and **New followers**

It works from Instagram's official data export, so there's no login and no password. Files are read locally and never uploaded.

## Use

1. Instagram → Accounts Center → Your information and permissions → Export your information → Create export → Export to device.
2. Choose only **Followers and following**, date range **All time**, format **JSON**.
3. Open `index.html` and drop in the downloaded zip (or `followers_1.json` + `following.json`).
4. Repeat every week or two. Each export is saved as a snapshot in the browser's local storage and compared with the previous one to find unfollowers.
