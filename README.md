# HOD Action Tracker (mydmeeting)

Follow-up tracker for action items from the District Collector's Monday HOD review meeting, Mayiladuthurai.

- Static site: `index.html`, no build step. Deploy on Vercel with the "Other" framework preset.
- Data: Firebase project `mydmeeting-43bc1`, collection `hodActions`. Anonymous sign-in must stay enabled.
- Anyone with the link can view. Editing needs the passcode (button "Unlock editing"). To change it, put the SHA-256 of the new passcode in `EDIT_HASH` in `index.html`.
- First load: unlock editing, then **Import Excel** with *HOD Open Action Items Tracker.xlsx*.

Note: the passcode only hides the edit controls. Real write protection needs Firestore security rules (for example Firebase Auth users with an editor list).
