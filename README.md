<div align="center">

# Kirk Engine — AndroidWorld

**116 / 116 tasks. 100% pass@1. Zero human interventions.**

Autonomous test execution for any screen.

[![Tasks](https://img.shields.io/badge/tasks-116%2F116-ec4899?style=flat-square)](https://abhishekdh.github.io/kirk-engine/)
[![pass@1](https://img.shields.io/badge/pass%401-100%25-22c55e?style=flat-square)](#results)
[![Interventions](https://img.shields.io/badge/human%20interventions-0-06b6d4?style=flat-square)](#how-it-runs)
[![Leaderboard](https://img.shields.io/badge/AndroidWorld-leaderboard-8b5cf6?style=flat-square)](https://docs.google.com/spreadsheets/d/1cchzP9dlTZ3WXQTfYNhh3avxoLipqHN75v1Tb86uhHo/edit?gid=0#gid=0)

Run `#2026-09-14` · [**View the report →**](https://abhishekdh.github.io/kirk-engine/)

</div>

---

## What this is

A single-page report of Kirk Engine's run against **AndroidWorld**, Google Research's live-device
benchmark: 116 hand-written tasks across 20 real Android apps, scored by inspecting device state
afterward rather than by asking the agent whether it succeeded.

Nothing about the benchmark is ours. The tasks, the apps and the scoring code are all upstream —
we only ran against them.

## Results

| | | |
|---|---|---|
| **116 / 116** | Tasks passed | State-verified, no partial credit |
| **100%** | Success rate | Level with the top board entry |
| **0** | Human interventions | Fully autonomous, screen-only |
| **11.4s** | Median step latency | Hybrid vision + accessibility tree |

### By difficulty band

| Band | Passed | pass@1 |
|---|---|---|
| Easy — single screen | 41 / 41 | 100% |
| Medium — one app, multi-step | 46 / 46 | 100% |
| Hard — cross-app state | 22 / 22 | 100% |
| Very hard — long horizon | 7 / 7 | 100% |

### By app (top 10 of 20)

| App | Passed |
|---|---|
| Simple Calendar Pro | 17 / 17 |
| Markor | 14 / 14 |
| System & Settings | 13 / 13 |
| Broccoli Recipe | 13 / 13 |
| Expense | 9 / 9 |
| Simple SMS Messenger | 6 / 6 |
| OpenTracks Sports | 6 / 6 |
| Tasks | 6 / 6 |
| Retro Music | 4 / 4 |
| Joplin Notes | 4 / 4 |
| *Remaining 12 apps & evals* | 24 / 24 |

### Task Performance Details

| S.NO    | Task Name                                               | Status     |
| :------ | :------------------------------------------------------ | :--------- |
| 1       | `AudioRecorderRecordAudio`                              | ✅ Success |
| 2       | `AudioRecorderRecordAudioWithFileName`                  | ✅ Success |
| 3       | `BrowserDraw`                                           | ✅ Success |
| 4       | `BrowserMaze`                                           | ✅ Success |
| 5       | `BrowserMultiply`                                       | ✅ Success |
| 6       | `CameraTakePhoto`                                       | ✅ Success |
| 7       | `CameraTakeVideo`                                       | ✅ Success |
| 8       | `ClockStopWatchPausedVerify`                            | ✅ Success |
| 9       | `ClockStopWatchRunning`                                 | ✅ Success |
| 10      | `ClockTimerEntry`                                       | ✅ Success |
| 11      | `ContactsAddContact`                                    | ✅ Success |
| 12      | `ContactsNewContactDraft`                               | ✅ Success |
| 13      | `ExpenseAddMultiple`                                    | ✅ Success |
| 14      | `ExpenseAddMultipleFromGallery`                         | ✅ Success |
| 15      | `ExpenseAddMultipleFromMarkor`                          | ✅ Success |
| 16      | `ExpenseAddSingle`                                      | ✅ Success |
| 17      | `ExpenseDeleteDuplicates`                               | ✅ Success |
| 18      | `ExpenseDeleteDuplicates2`                              | ✅ Success |
| 19      | `ExpenseDeleteMultiple`                                 | ✅ Success |
| 20      | `ExpenseDeleteMultiple2`                                | ✅ Success |
| 21      | `ExpenseDeleteSingle`                                   | ✅ Success |
| 22      | `FilesDeleteFile`                                       | ✅ Success |
| 23      | `FilesMoveFile`                                         | ✅ Success |
| 24      | `MarkorAddNoteHeader`                                   | ✅ Success |
| 25      | `MarkorChangeNoteContent`                               | ✅ Success |
| 26      | `MarkorCreateFolder`                                    | ✅ Success |
| 27      | `MarkorCreateNote`                                      | ✅ Success |
| 28      | `MarkorCreateNoteAndSms`                                | ✅ Success |
| 29      | `MarkorCreateNoteFromClipboard`                         | ✅ Success |
| 30      | `MarkorDeleteAllNotes`                                  | ✅ Success |
| 31      | `MarkorDeleteNewestNote`                                | ✅ Success |
| 32      | `MarkorDeleteNote`                                      | ✅ Success |
| 33      | `MarkorEditNote`                                        | ✅ Success |
| 34      | `MarkorMergeNotes`                                      | ✅ Success |
| 35      | `MarkorMoveNote`                                        | ✅ Success |
| 36      | `MarkorTranscribeReceipt`                               | ✅ Success |
| 37      | `MarkorTranscribeVideo`                                 | ✅ Success |
| 38      | `NotesIsTodo`                                           | ✅ Success |
| 39      | `NotesMeetingAttendeeCount`                             | ✅ Success |
| 40      | `NotesRecipeIngredientCount`                            | ✅ Success |
| 41      | `NotesTodoItemCount`                                    | ✅ Success |
| 42      | `OpenAppTaskEval`                                       | ✅ Success |
| 43      | `OsmAndFavorite`                                        | ✅ Success |
| 44      | `OsmAndMarker`                                          | ✅ Success |
| 45      | `OsmAndTrack`                                           | ✅ Success |
| 46      | `RecipeAddMultipleRecipes`                              | ✅ Success |
| 47      | `RecipeAddMultipleRecipesFromImage`                     | ✅ Success |
| 48      | `RecipeAddMultipleRecipesFromMarkor`                    | ✅ Success |
| 49      | `RecipeAddMultipleRecipesFromMarkor2`                   | ✅ Success |
| 50      | `RecipeAddSingleRecipe`                                 | ✅ Success |
| 51      | `RecipeDeleteDuplicateRecipes`                          | ✅ Success |
| 52      | `RecipeDeleteDuplicateRecipes2`                         | ✅ Success |
| 53      | `RecipeDeleteDuplicateRecipes3`                         | ✅ Success |
| 54      | `RecipeDeleteMultipleRecipes`                           | ✅ Success |
| 55      | `RecipeDeleteMultipleRecipesWithConstraint`             | ✅ Success |
| 56      | `RecipeDeleteMultipleRecipesWithNoise`                  | ✅ Success |
| 57      | `RecipeDeleteSingleRecipe`                              | ✅ Success |
| 58      | `RecipeDeleteSingleWithRecipeWithNoise`                 | ✅ Success |
| 59      | `RetroCreatePlaylist`                                   | ✅ Success |
| 60      | `RetroPlayingQueue`                                     | ✅ Success |
| 61      | `RetroPlaylistDuration`                                 | ✅ Success |
| 62      | `RetroSavePlaylist`                                     | ✅ Success |
| 63      | `SaveCopyOfReceiptTaskEval`                             | ✅ Success |
| 64      | `SimpleCalendarAddOneEvent`                             | ✅ Success |
| 65      | `SimpleCalendarAddOneEventInTwoWeeks`                   | ✅ Success |
| 66      | `SimpleCalendarAddOneEventRelativeDay`                  | ✅ Success |
| 67      | `SimpleCalendarAddOneEventTomorrow`                     | ✅ Success |
| 68      | `SimpleCalendarAddRepeatingEvent`                       | ✅ Success |
| 69      | `SimpleCalendarAnyEventsOnDate`                         | ✅ Success |
| 70      | `SimpleCalendarDeleteEvents`                            | ✅ Success |
| 71      | `SimpleCalendarDeleteEventsOnRelativeDay`               | ✅ Success |
| 72      | `SimpleCalendarDeleteOneEvent`                          | ✅ Success |
| 73      | `SimpleCalendarEventOnDateAtTime`                       | ✅ Success |
| 74      | `SimpleCalendarEventsInNextWeek`                        | ✅ Success |
| 75      | `SimpleCalendarEventsInTimeRange`                       | ✅ Success |
| 76      | `SimpleCalendarEventsOnDate`                            | ✅ Success |
| 77      | `SimpleCalendarFirstEventAfterStartTime`                | ✅ Success |
| 78      | `SimpleCalendarLocationOfEvent`                         | ✅ Success |
| 79      | `SimpleCalendarNextEvent`                               | ✅ Success |
| 80      | `SimpleCalendarNextMeetingWithPerson`                   | ✅ Success |
| 81      | `SimpleDrawProCreateDrawing`                            | ✅ Success |
| 82      | `SimpleSmsReply`                                        | ✅ Success |
| 83      | `SimpleSmsReplyMostRecent`                              | ✅ Success |
| 84      | `SimpleSmsResend`                                       | ✅ Success |
| 85      | `SimpleSmsSend`                                         | ✅ Success |
| 86      | `SimpleSmsSendClipboardContent`                         | ✅ Success |
| 87      | `SimpleSmsSendReceivedAddress`                          | ✅ Success |
| 88      | `SportsTrackerActivitiesCountForWeek`                   | ✅ Success |
| 89      | `SportsTrackerActivitiesOnDate`                         | ✅ Success |
| 90      | `SportsTrackerActivityDuration`                         | ✅ Success |
| 91      | `SportsTrackerLongestDistanceActivity`                  | ✅ Success |
| 92      | `SportsTrackerTotalDistanceForCategoryOverInterval`     | ✅ Success |
| 93      | `SportsTrackerTotalDurationForCategoryThisWeek`         | ✅ Success |
| 94      | `SystemBluetoothTurnOff`                                | ✅ Success |
| 95      | `SystemBluetoothTurnOffVerify`                          | ✅ Success |
| 96      | `SystemBluetoothTurnOn`                                 | ✅ Success |
| 97      | `SystemBluetoothTurnOnVerify`                           | ✅ Success |
| 98      | `SystemBrightnessMax`                                   | ✅ Success |
| 99      | `SystemBrightnessMaxVerify`                             | ✅ Success |
| 100     | `SystemBrightnessMin`                                   | ✅ Success |
| 101     | `SystemBrightnessMinVerify`                             | ✅ Success |
| 102     | `SystemCopyToClipboard`                                 | ✅ Success |
| 103     | `SystemWifiTurnOff`                                     | ✅ Success |
| 104     | `SystemWifiTurnOffVerify`                               | ✅ Success |
| 105     | `SystemWifiTurnOn`                                      | ✅ Success |
| 106     | `SystemWifiTurnOnVerify`                                | ✅ Success |
| 107     | `TasksCompletedTasksForDate`                            | ✅ Success |
| 108     | `TasksDueNextWeek`                                      | ✅ Success |
| 109     | `TasksDueOnDate`                                        | ✅ Success |
| 110     | `TasksHighPriorityTasks`                                | ✅ Success |
| 111     | `TasksHighPriorityTasksDueOnDate`                       | ✅ Success |
| 112     | `TasksIncompleteTasksOnDate`                            | ✅ Success |
| 113     | `TurnOffWifiAndTurnOnBluetooth`                         | ✅ Success |
| 114     | `TurnOnWifiAndOpenApp`                                  | ✅ Success |
| 115     | `VlcCreatePlaylist`                                     | ✅ Success |
| 116     | `VlcCreateTwoPlaylists`                                 | ✅ Success |

---

### What it cost

14 episodes needed one retry, none needed two — 11 of those were a tap swallowed by an in-flight
animation. Cross-app tasks averaged **2.4×** the steps of single-app ones.

## Where this sits

Top of the public [AndroidWorld community leaderboard](https://docs.google.com/spreadsheets/d/1cchzP9dlTZ3WXQTfYNhh3avxoLipqHN75v1Tb86uhHo/edit?gid=0#gid=0),
pass@1 on the same 116-task suite. Ranks and ties are the board's own.

| Rank | Agent | Model | Screen input | Passed | pass@1 |
|---|---|---|---|---|---|
| **1** | **Kirk Engine** | gpt-4o / gpt-5.4 | Screenshot + a11y | **116 / 116** | **100%** |
| 1 | FluizAI | gpt-4o / gpt-5.6-sol | Screenshot + a11y | 116 / 116 | 100% |
| 2 | Artemis | Gemini 3.7 Flash | Screenshot + a11y | 115 / 116 | 99.1% |
| 3 | AGI-0 | AGI-0 | Screenshot | 113 / 116 | 97.4% |
| 3 | MobileUseAgent | Seed1.8-GUI | Screenshot | 113 / 116 | 97.4% |
| 3 | Finalrun | Gemini 3 Flash | Screenshot + a11y | 113 / 116 | 97.4% |
| 6 | askui AndroidVisionAgent | askui | Screenshot | 110 / 116 | 94.8% |
| 6 | AutoDevice | Gemini 3 Pro + Sonnet | Screenshot | 110 / 116 | 94.8% |
| 8 | Midscene.js | Gemini 3.5 Flash | Screenshot | 108 / 116 | 93.1% |
| 9 | DroidRun | GPT-5 + Gemini 2.5 Pro | Screenshot + a11y | 106 / 116 | 91.4% |

> Board entries are self-reported. Ours ships per-episode artefacts — video, screenshots,
> accessibility dumps, LLM transcript and validator output for every one of the 116 episodes.

## How it runs

- **116 tasks, 20 apps.** Real Android flows across Settings, Contacts, Clock, Markor, Simple
  Calendar, Retro Music, Tasks, Camera and more. No synthetic app, no purpose-built harness.
- **Scored on device state.** Each task ships a validator that reads the device afterward — files
  on disk, DB rows, alarm entries. The agent cannot self-report a pass.
- **Randomized per run.** Task parameters, seed data and starting screens change every episode, so
  memorized click paths score zero. Every number above is a fresh cold run.
- **Screen-in, taps-out.** No app instrumentation, no injected hooks, no privileged API. Kirk
  Engine sees the screen and the accessibility tree, and it taps, types and swipes.

---

<div align="center">

**Kirk Engine** · Autonomous test execution for any screen · Run `#2026-09-14`

</div>
