# passync

This is an attempt to write solution to sync passwords from Chrome to Safari's
iCloud storage (so it'll be synced to iPhone).

The biggest problem is that iCloud keychain is not available through command
line `security` utility. So it works through Applescript's UI scripting (for
Safari), which is really slow and requires Safari to be active application. This
in turn means I can't put this in cron to just sync all the time.
