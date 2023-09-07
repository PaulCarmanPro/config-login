# configuration-debian

I am very good at bombing an OS.
These bash_login files execute during login and convert a fresh install to paulian.
Fresh debian install needs NO desktop or window manager.

Paulian features:
- No Desktop.
- No file manager.
- Currently uses openbox.
- Super keybindngs for common commands.
- Every window is meant to consume the entire screen.
- If window does not consume entire display, then press Super-3.
- Uses of 'focus' which locates an existing window to bring to top or launches a program which is expected to.

Example: Super-E is short for "email". Currently, thunderbird is used as the email client (still configuing neomutt). If thunderbird is open, then Super-E will cycle around all open thunderbird windows. Otherwise, Super-E will launch thunderbird. This is accomplished via a single line declartion in openbox's rc file which launches 'focus'.

- Press Super-K to view and edit the keyboard declaration file and make it yours.
