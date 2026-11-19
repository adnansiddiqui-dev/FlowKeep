# Using FlowKeep

## First launch

1. HyperOS shows **"Review permissions"** for FlowKeep. Turn on **Modify system settings** and
   **Access list of installed apps**, then tap **OK**. (Everything else on that list is unused.)
2. Open FlowKeep again if HyperOS returned to the home screen.
3. Read the two short pages, then choose your apps. **Google Play services is pre-selected**:
   it delivers notifications for most apps.
4. On **Three switches, then you're done**, tap each row until it says *Allowed*:
   - **Modify system settings**: lets FlowKeep add your apps to Xiaomi's no-freeze list.
   - **Autostart for FlowKeep**: lets FlowKeep fix the list while it's closed.
   - **Battery: No restrictions**: so HyperOS never freezes FlowKeep itself.
5. Tap **Start FlowKeep**. Your apps are added at once.

## Every day: one screen, one switch per app

- The **top card** says, in one sentence, whether everything is fine ("Notifications are
  flowing") or the one thing to tap next. Your kept apps ride on a flowing line at the bottom of
  the card; an amber ring and dot mean that app needs a tap.
- **Keep flowing** lists your apps. Each row says *Flowing*, or what's wrong:
  - *Autostart is off · Tap to fix*: tap the row, then **Open settings**, switch **Autostart**
    on and come back. FlowKeep confirms with "All set".
  - *Removed by Xiaomi · Tap to fix*: tap the row to put it back now (FlowKeep also does this by
    itself within seconds).
- **Suggested** lists popular apps that often miss notifications on HyperOS (messaging, social,
  email, work chat, calls) — only the ones installed on your phone that you don't keep flowing
  yet. Flip one on, or tap **Turn on all**. FlowKeep never adds them by itself.
- **Other apps** lists your other apps. Flip the switch to start keeping one flowing.
  **Show system apps** reveals background apps too; searching always searches everything.
- **Turning an app on** adds it to Xiaomi's no-freeze list immediately. If its Autostart is off,
  FlowKeep shows how to turn it on. Xiaomi only lets *you* change Autostart, so FlowKeep opens the
  exact page instead of changing it.
- **Turning an app off** takes it off the list. If its Autostart is on, FlowKeep offers to open
  the page so you can turn that off too (optional).
- Tap an app's name for its page: the same switch, and a two-item checklist.
- The **ⓘ** button explains how FlowKeep works in four lines.

## Settings

- **Protect in the background**: the main on/off switch.
- **Instant fixing**: fixes in under a second using a small silent notification. Only needed if
  notifications are still late.
- **Start after restart** and **Alerts** (only when an app drops off and can't be put back).
- **What FlowKeep needs**: the status of each permission; tap a row to open its page.
- **Appearance**: System, Light or Dark.
- **Developer**: Adnan Siddiqui's website, LinkedIn and Facebook (open in your browser) and
  WhatsApp (opens the chat directly).
- **Advanced** (for troubleshooting): History, Xiaomi's list (the exact value, add by package
  name, restore backups including the original), Smart/Eco checking, Fix automatically, Reconnect
  Google push, Export/Import, Diagnostics.

## If something looks wrong

- *"One permission needed"* → tap **Allow** and turn on **Modify system settings**.
- *"Turn on Autostart for FlowKeep"* → tap **Open settings** and switch Autostart on.
- *"One battery setting"* → choose *No restrictions* for FlowKeep.
- Notifications still late for one app → check that its row says *Flowing* (Autostart on). If
  it does, try **Instant fixing** in Settings.

## Undo everything

Settings → turn off **Protect in the background**. Settings → Advanced → Xiaomi's list → Backups →
*Original value* → Restore. Then uninstall; HyperOS removes FlowKeep from its list by itself.
