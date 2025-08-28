# MEA-Game
a game for naturalists that helps them for the Critical Habitat Assessment.# README.md

Critical Habitat Quest is a mobile game that teaches and guides users through creating a **Critical Habitat Assessment (CHA) Plan**. Players progress through short, interactive missions (Site, Species, Habitat Features, Threats, Mitigation, Monitoring), then auto-generate a well-structured **PDF plan** for export/share.

The app is built with **Flutter**, uses provider for state, and the `pdf` + `printing` packages for PDF generation & sharing.

---

## Features
- Guided, mission-style flow with progress tracking
- Offline-first (no backend)
- Autosave (in-memory during session; add Hive/SharedPreferences if needed)
- Export **PDF** of the CHA Plan (English; easy to localize)
- Mobile-friendly UI, large touch targets, validation, error handling
- Clean architecture, strongly typed models, null safety

---

## Project Structure
```
/critical_habitat_quest
  ├── pubspec.yaml
  └── lib/
      └── main.dart
```

> This minimal scaffold is production-ready. You can scale to multiple files later.

---

## Quick Start
1) Install Flutter (3.19+ recommended).
2) Create a new project, then replace `pubspec.yaml` and `lib/main.dart` with the files below.
3) Run: `flutter pub get`
4) Test on device: `flutter run`
5) Build Android App Bundle: `flutter build appbundle`
6) Upload to Google Play Console (Internal Testing → Closed/Open → Production).

---

## Play Console Notes
- Package name is set by your project. Use a unique applicationId in `android/app/build.gradle`, e.g. `com.barcelonareact.chaquest`.
- App icon: replace launcher icons via `flutter_launcher_icons` (optional).
- Privacy policy: include a simple static page or link (no data collection by default).
- Content rating: Education, no UGC, no location.

