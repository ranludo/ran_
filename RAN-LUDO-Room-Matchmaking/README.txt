# RAN LUDO - Online Room Demo

## What this version does
- Firebase Email/Password signup + login
- Dashboard with points
- Create a unique 6-digit room
- Join a room by entering the 6-digit code
- Quick Play public matchmaking: automatically joins an available public room or creates one
- Multiple independent rooms can run at the same time
- Maximum 4 players per room
- Live online player lobby using Cloud Firestore
- Host can start the room status
- RAN LUDO logo included

## Firebase setup

1. Open Firebase Console.
2. Open project: ran-ludo-eb86d
3. Authentication -> Sign-in method -> enable **Email/Password**.
4. Firestore Database -> Create database.
5. In Firestore -> Rules, replace the rules with the contents of `firestore.rules`.
6. Save/publish the rules.
7. Keep all files in the same folder.
8. Open the project through a local web server (recommended), not by double-clicking the HTML file.

## Run locally

If Python is installed:
python -m http.server 5500

Then open:
http://localhost:5500

Or use VS Code + Live Server.

## Important
The Firebase web config is intended for client-side Firebase apps. Do not add service-account JSON or private keys to this project.

This is an online room/lobby system. It does not integrate with or control Ludo King, and it does not contain real-money betting/withdrawal functionality.

The actual Ludo board, dice, token movement, turn synchronization and win logic can be added as the next module.
