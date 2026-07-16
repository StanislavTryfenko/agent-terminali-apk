Agent Terminali

Latest release — fixes enrollment revert loop and incomplete state rollback:

- Enrollment retry cooldown (60 s) after a failed attempt so a missing enrollment.json no longer triggers an infinite retry loop on every AP change
- SharedPreferences (agent_config) fully re-synced from the restored config.json after any rollback — prefs no longer hold stale values from a failed enrollment
- HOME alias released after rollback when kiosk was not active before the failed enrollment
- Kiosk exit password: null / missing / empty hash in server policy exits immediately with no password prompt

[Download APK](https://stanislavtryfenko.github.io/agent-terminali-apk/app-release.apk)
