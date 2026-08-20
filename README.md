# YMC — yestminds.com

Passcode-protected landing page for Yest Minds Co.

The page body is encrypted with AES-256-GCM (PBKDF2-SHA256, 250k iterations) and
is decrypted in the browser only after the correct passcode is entered. The
plaintext is therefore not present in the served source at all.

The source copy and the build script are intentionally **not** in this repository,
since it is public. They live alongside the brand assets in the project working
directory; rebuilding is `python build.py [NEW-PASSCODE]`.
