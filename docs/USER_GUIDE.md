# Using FlowKeep

## First launch

1. HyperOS first shows its own **"Review permissions"** list for FlowKeep (Xiaomi shows it for
   apps like this; FlowKeep can't change it). Only the first two switches matter: turn on
   **Access list of installed apps** and **Modify system settings**, leave everything else off,
   and tap **OK**.
2. If either of those two is off, FlowKeep opens on **"Two permissions to start"** and goes no
   further. Each permission has an **Allow** button that opens the right page:
   - *Modify system settings* opens Android's page with one switch, **Allow modifying system
     settings**.
   - *Access list of installed apps* opens Xiaomi's permission page: tap **Other permissions**,
     then turn on **Access list of installed apps**.

   Come back to FlowKeep and the screen clears by itself. (It comes back the same way if one is
   ever turned off later.)
3. Read the two short pages, then choose apps. **Google Play services is pre-selected**: it
   delivers notifications for most apps.
4. On **Two more switches, then you're done**, tap each row until it says *Allowed*/*Done*:
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
