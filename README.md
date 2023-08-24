# configuration-debian

Made to create the 'carmian' version of debian given a fresh debian install WITHOUT any desktop or window manager. Carmian boots into the console and runs .bash_login which checks the OS. A new user will imediately have to execute 'sudo .bash_login' once logged in to allow .bash_login to perform the OS setup. 

Carmian OS has no desktop and every program is meant to consume the entire screen. Carmian uses openbox and configures it to create keyboard shortcuts using the Windows|Super|Meta modifier to starup/select programs/windows. Carmian is uniqued by the a program called 'focus' (inclcuded in this repository) which locates an existing window to bring to top (focus) or launches a program which is expected to perform the task.

Example: Super-E is short for "email". Currently, thunderbird is used as the email client (still trying to understand mutt). If thunderbird is open, then Super-E will cycle around all open thunderbird windows. Otherwise, Super-E will launch thunderbird. This is accomplished via a single line declartion in openbox's rc file which launches 'focus'.

Carmian does not include a file manager as the user experience prefers the command line. Unlike Ubuntu and other releases, Carmian does not modify any existing packages. Carmian expects a basic debian install and provides an automated setup that can easily be modified via examination of .bash_login.
