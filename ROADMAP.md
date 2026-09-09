# Roadmap

## M0 — Establish the project

- [x] Record the owner's authorization, non-negotiable AutoMix requirement, and future app ambition.
- [x] Create local project documents and private Drive folder.
- [x] Commit local project and verify cloud snapshot presence and private permissions through Drive metadata.
- [x] Publish public GitHub repository and verify the initial files remotely.

## M1 — Prove playback and control

- [ ] Inventory the exact Mac, OS, Watch, JBL models, and current remote app.
- [ ] Confirm AutoMix on eligible Apple Music subscription tracks and the selected audio route.
- [ ] Test a supported Mac control interface for music volume, playback, track advance, and state reporting.
- [ ] Confirm music continues while the personal phone and MacBook independently play media.
- [ ] Prove Watch-to-host communication with authenticated pairing and no public network exposure.
- [ ] Verify that global volume audibly changes the intended speaker output and stays within a configured ceiling.
- [ ] Run an all-day playback trial, logging interruptions and remote responsiveness.

Exit criterion: AutoMix plays on a house device while Watch volume works reliably, with observed test evidence.

## M2 — Daily-use remote

- [ ] Build Watch volume, play/pause, skip, and connection status interface.
- [ ] Add iPhone setup, pairing, and detailed controls.
- [ ] Validate reachability throughout the house, reconnection, stale state, and explicit disconnect behavior.

## M3 — Recovery and multiple speakers

- [ ] Distinguish user pause from crash, network loss, and output loss.
- [ ] Test bounded recovery, safe resume volume, and stable output identity.
- [ ] Verify speaker synchronization while walking between rooms; document latency and dropout limits.
- [ ] Add individual speaker controls only for routes exposing independent gain and connection state.
- [ ] Document cold boot versus signed-in session behavior; do not promise unattended recovery through OS authentication.

## M4 — Product candidate

- [ ] Establish a supported hardware and OS matrix.
- [ ] Validate Apple APIs, entitlement needs, background behavior, and distribution constraints.
- [ ] Add onboarding, accessibility, privacy documentation, error recovery, and beta feedback.
- [ ] Decide name, licensing, business model, and whether to submit an official app.

No app implementation or physical-device acceptance testing is complete at project kickoff.
