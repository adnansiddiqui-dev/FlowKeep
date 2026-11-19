# Permissions

FlowKeep asks only for what it uses. Nothing is granted silently; every Xiaomi switch is opened
for the user to flip.

| Permission / switch | Required? | Why | Where the user grants it |
|---|---|---|---|
| **Modify system settings** (`WRITE_SETTINGS`) | Yes, to change the list | Android's gate for writing `Settings.System`; with FlowKeep's target level it also covers the non-public `MILLET_NO_RESTRICT_APP` key | HyperOS permission review on first launch, or Settings → *Modify system settings* |
| **Autostart** (MIUI app-op 10008) | Yes, for background repairs | Without it HyperOS refuses to start FlowKeep's job when its process isn't running (`AutoStartManagerService: Reject service`) | FlowKeep's App info page (one switch) |
| **Battery saver: No restrictions** for FlowKeep | Strongly recommended | Stops Greezer freezing FlowKeep; puts it in the EXEMPTED standby bucket so its trigger job isn't deferred | FlowKeep's battery page (deep link) |
| Access list of installed apps (`com.android.permission.GET_INSTALLED_APPS`) | Recommended | China HyperOS can hide other apps from the app list without it | Permission review / permission editor |
| Notifications (`POST_NOTIFICATIONS`) | Optional | Alerts when an app couldn't be put back; the Always-on notification | System notification settings |
| `RECEIVE_BOOT_COMPLETED` | Optional | "Start after reboot"; the receiver component is disabled when the option is off | Install-time |
| `FOREGROUND_SERVICE` | Optional | Only for Always-on mode (off by default) | Install-time |

Not requested: `INTERNET`, `QUERY_ALL_PACKAGES` (package visibility filtering doesn't apply to
FlowKeep's target level), location, storage, accessibility, overlay, device admin,
`WRITE_SECURE_SETTINGS`.

## What is impossible without more privilege

- Setting Xiaomi's per-app *No restrictions* policy for another app programmatically (its
  provider requires a signature permission; even the shell is refused).
- Seeing packages in Second space / Dual apps, or the ~34 packages HyperOS hides from all apps.
- Overriding HyperOS's night-time freeze or GMS network limits.
- Writing `MILLET_NO_RESTRICT_APP` from an app targeting API ≥ 23 (see RESEARCH).
