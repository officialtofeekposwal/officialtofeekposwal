<h1 align="center">
<picture>
<source media="(prefers-color-scheme: dark)" srcset="assets/hero-dark.svg">
<img src="assets/hero-light.svg" alt="Tofeek Poswal. Offline-first Android apps. Your data belongs on your device." width="100%">
</picture>
</h1>

<p align="center">
I build offline-first Android apps that keep your data on your device.
</p>

<p align="center">
<a href="https://github.com/officialtofeekposwal?tab=followers"><img src="https://img.shields.io/github/followers/officialtofeekposwal?style=flat&color=14B8A6&labelColor=0F1626" alt="GitHub followers"></a>
<a href="https://github.com/officialtofeekposwal/poswal-orbit/stargazers"><img src="https://img.shields.io/github/stars/officialtofeekposwal/poswal-orbit?style=flat&label=Orbit%20stars&color=8B7CFF&labelColor=0F1626" alt="Poswal Orbit stars"></a>
<a href="https://github.com/officialtofeekposwal/PoswalNoor/stargazers"><img src="https://img.shields.io/github/stars/officialtofeekposwal/PoswalNoor?style=flat&label=Noor%20stars&color=FFC857&labelColor=0F1626" alt="Poswal Noor stars"></a>
</p>

<p align="center">
<a href="#about">About</a> ·
<a href="#projects">Projects</a> ·
<a href="#stack">Stack</a> ·
<a href="#how-i-work">How I work</a> ·
<a href="#contact">Contact</a>
</p>

## About

I make Android apps that work without an account and without a network. My two main projects are Poswal Orbit, a habit, task and note app, and Poswal Noor, an offline Islamic reference app. Both store everything on the phone.

I am currently building both of them, and learning Android system internals and Kotlin 2.x.

Ask me about Flutter, Dart, Kotlin, Android, SQLite, local-first design and state management.

<p align="center"><img src="assets/divider.svg" alt="" width="100%"></p>

## Projects

### Poswal Orbit

<a href="https://github.com/officialtofeekposwal/poswal-orbit"><img src="assets/card-orbit.svg" alt="Poswal Orbit: habits, tasks, notes. Illustration of the app logo with a small planet circling it." width="100%"></a>

Habits, tasks and notes in one offline Android app. Habits are the inner orbit, tasks the outer one, and notes hold the day together.

- Built with Flutter and Dart. State is handled with Riverpod and data is stored with Drift (SQLite).
- The day starts at 4:00 AM by default, so a check-in after midnight counts for the day before.
- Habits have a consistency score and an optional streak freeze. Tasks accept plain sentences such as "Pay rent tomorrow 4pm".
- English, Hindi and Urdu, with a right-to-left layout and bundled fonts.
- No accounts and no analytics. Release builds do not request the `INTERNET` permission. Debug and CI test builds may.
- Automated tests run in CI. Text colors are tested for WCAG AA contrast.

**Status.** Android builds are made by CI. Verification on real phones is in progress. iOS code is written but not verified, because I have no Mac. It is not on the Play Store. To try it, follow the [CI debug build steps](https://github.com/officialtofeekposwal/poswal-orbit/blob/main/docs/INSTALL_DEBUG_APK.md).

[Repository](https://github.com/officialtofeekposwal/poswal-orbit) · MIT license

### Super Apple Design

<a href="https://github.com/officialtofeekposwal/super-apple-design"><img src="assets/card-super-apple-design.svg" alt="Super Apple Design: a skill pack for AI tools. Illustration of four stacked panes lifting one after another." width="100%"></a>

A set of instructions for AI coding tools. A skill is a Markdown file that a tool such as Claude Code or Cursor reads before it starts work.

- Two skills: `apple-design-universal`, design rules rewritten in my own words from Apple's Human Interface Guidelines, and `design-workflow`, a four-phase routine of direction, build, test and review.
- A Cursor rule file, and an `AGENTS.md` file for Codex and Windsurf.
- An install script that copies the skills into the right folder for each tool. With `--with-upstream` it also clones seven skills from their original authors. Their code is not copied into this repository.
- Not affiliated with Apple. No tagged release yet.

[Repository](https://github.com/officialtofeekposwal/super-apple-design) · MIT license

### Poswal Noor

<a href="https://github.com/officialtofeekposwal/PoswalNoor"><img src="assets/card-noor.svg" alt="Poswal Noor: an offline Islamic app. Illustration of a compass with a swinging needle and a crescent moon." width="100%"></a>

An offline Islamic reference app for Android, written in Kotlin with Jetpack Compose and Material 3.

- The Quran: 6,236 ayahs in 114 surahs, in Arabic with English, Hindi and Urdu translations.
- Hadith: 14,060 records from Sahih al-Bukhari and Sahih Muslim.
- Prayer times are calculated on the device for a built-in list of 38 cities, with a standard or Hanafi Asr setting. The Qibla compass uses the phone's rotation sensor.
- Dhikr and tasbih tools, a Hijri calendar and home screen widgets.
- The app's own manifest declares no permissions, so it does not request `INTERNET`.
- `DATA_SOURCES.md` lists where each text comes from and its license. A few items are marked unverified there.

[Repository](https://github.com/officialtofeekposwal/PoswalNoor) · MIT license

<p align="center"><img src="assets/divider.svg" alt="" width="100%"></p>

## Stack

<img src="assets/stack.svg" alt="Eight chips: Flutter, Dart, Kotlin, Compose, Riverpod, Drift, Room and Actions (GitHub Actions). The same list is written out below." width="100%">

These are the technologies that appear in the three repositories above.

- **Flutter and Dart:** Poswal Orbit.
- **Kotlin and Jetpack Compose:** Poswal Noor. Orbit's Android widget code is also Kotlin.
- **Riverpod:** state management in Orbit.
- **Drift and Room:** SQLite access in Orbit and Noor.
- **GitHub Actions:** build, test and release workflows in Orbit.

<details>
<summary>Also in these repositories</summary>

- Hilt, Paging 3 and Glance in Noor.
- go_router and home_widget in Orbit.
- Python scripts that build Noor's content database.
- Swift in Orbit's iOS widget code. It has not been verified on a device.

</details>

## How I work

- **Keep data on the device.** Both apps store everything locally and work without a network.
- **Test the logic that matters.** In Orbit, streaks, scores, schedules and quick add are plain Dart with automated tests, run in CI.
- **Say what is verified.** Orbit's repository states plainly that iOS has not been verified.
- **Keep the interface calm.** Sentence-case text, no emoji in the app, and support for reduced motion.

<p align="center"><img src="assets/divider.svg" alt="" width="100%"></p>

## Contact

- GitHub: [officialtofeekposwal](https://github.com/officialtofeekposwal)
- Questions or bugs: open an issue on [Poswal Orbit](https://github.com/officialtofeekposwal/poswal-orbit/issues) or [Poswal Noor](https://github.com/officialtofeekposwal/PoswalNoor/issues)
- Email: [workwithtofeek@gmail.com](mailto:workwithtofeek@gmail.com)
- Instagram: [officialtofeekposwal](https://instagram.com/officialtofeekposwal)
