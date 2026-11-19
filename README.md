<p align="center">
  <img src="assets/flowkeep-icon.png" width="112" alt="FlowKeep icon">
</p>

<h1 align="center">FlowKeep</h1>

<p align="center"><b>Let notifications flow.</b><br>
Keeps the notifications from your important apps arriving on time on Xiaomi HyperOS.</p>

<p align="center">
  <a href="https://github.com/adnansiddiqui-dev/FlowKeep/releases/latest"><b>⬇ Download the latest APK</b></a>
</p>

---

## The problem

To save battery, HyperOS freezes apps you aren't using. A frozen app can't receive messages, so
its notifications arrive late or not at all. Xiaomi keeps a list of apps it never freezes, but it
rewrites that list now and then and drops apps it didn't choose. Google Play services, which
delivers the notifications for most apps, has no setting to stay on it.

## What FlowKeep does

- **One switch per app.** Turn an app on and FlowKeep puts it on Xiaomi's no-freeze list,
  including Google Play services.
- **Puts them back within seconds** whenever Xiaomi removes them, then asks Google Play services
  to reconnect so pushes resume immediately.
- **Guides the rest.** If an app's Xiaomi *Autostart* switch is off, FlowKeep shows you exactly
  where to turn it on, and warns until it is.
- **Suggests popular apps** that often miss notifications (messaging, social, email, work chat),
  only the ones installed on your phone.
- **Uses almost no battery.** Nothing runs until Xiaomi changes its list; an open, idle FlowKeep
  draws nothing. Measured numbers: [Battery & performance](docs/BATTERY.md).
- **Private by design.** No internet permission, no analytics, no ads, no account. It doesn't
  need root, a second app or Developer options. See [Permissions & privacy](docs/PERMISSIONS.md).

## Requirements

- A **Xiaomi, Redmi or POCO** phone with **HyperOS**, **Android 12 or newer**.
- Tested on a Redmi K90 with HyperOS 4 (China ROM, Android 17). Other models and HyperOS versions
  should behave the same but are not confirmed yet; reports are welcome.
- FlowKeep deliberately targets an older Android API level, because that is what lets an app edit
  Xiaomi's list. HyperOS 4 (China) installs it normally; stock Android 14+ and possibly some global
  ROMs refuse apps like this. If installation is blocked, please open an issue.

## Install

1. On your phone, open **[Releases](https://github.com/adnansiddiqui-dev/FlowKeep/releases/latest)**,
   download `FlowKeep-….apk` and open it (allow installing from your browser if asked).
2. HyperOS shows **Review permissions**: turn on **Modify system settings** and **Access list of
   installed apps**, then tap OK.
3. In FlowKeep's setup, tap the three switches it lists: **Modify system settings**, **Autostart
   for FlowKeep** and **Battery: No restrictions**.
4. Done. Google Play services is pre-selected; turn on your chat and mail apps on the home screen.

To update, install the newer APK over the old one; your settings stay.

Full walkthrough: [User guide](docs/USER_GUIDE.md).

## Honest limits

Being on Xiaomi's list stops HyperOS's routine freezing. HyperOS has a few other limits, such as
deep sleep at night, that no app can change, so FlowKeep makes late notifications much rarer but
can't promise every single one is instant.

## Feedback

Found a bug or have a phone it doesn't work on? Open an
[issue](https://github.com/adnansiddiqui-dev/FlowKeep/issues) with your phone model and HyperOS
version (Settings → About phone).

## Developer

Made by **Adnan Siddiqui** · [adnansiddiqui.dev](https://adnansiddiqui.dev) ·
[LinkedIn](https://www.linkedin.com/in/adnansiddiqui-dev/) ·
[Facebook](https://www.facebook.com/adnansiddiqui.dev)

FlowKeep is free to use. Its source code is not public. Xiaomi, Redmi, POCO, HyperOS and Google
Play are trademarks of their owners; FlowKeep is not affiliated with them.
