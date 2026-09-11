# House Music Remote

Status: Active public project — definition and feasibility stage. Started September 9, 2026. Working name; no final brand selected.

## First milestone

“AutoMix all day, volume on my wrist.”

Apple Music plays on a dedicated house device. Apple Watch controls global music volume. The personal iPhone and MacBook remain free to play videos, take calls, and move around without interrupting house audio. True Apple AutoMix is mandatory; ordinary crossfade is not a substitute.

## Proposed architecture (not yet validated)

Apple Watch / iPhone → authenticated local control bridge → Apple Music on a dedicated Apple-silicon Mac → supported audio output → speakers.

Apple Music remains the playback engine and owns AutoMix. The companion app sends controls; it does not reproduce Apple's mixing engine. An Apple-silicon Mac is the current candidate, not a purchase authorization. Windows may support orchestration later, but is not the selected AutoMix engine.

MVP: global volume, play/pause, next track, and accurate connection status. Verify control of the actual music output, not an unrelated system volume slider. The source remains independent of the personal phone and MacBook.

## Later milestones

1. Watch Digital Crown control and a more detailed iPhone controller.
2. Synchronized portable speaker, speaker groups, independent volume where hardware supports it.
3. Reconnect and recovery after app crashes, device disconnects, and reboots. Explicit user pause must survive recovery; retries must be bounded.
4. Potential public app: reusable pairing, device support matrix, accessibility, privacy review, distribution feasibility, beta testing, and App Store review. Public release and purchases are future decisions.

## Compatibility questions

Validate host OS, Watch model, speaker generations, and output capabilities before implementation. Do not assume PartyBoost from a computer, independent Bluetooth outputs in sync, individual speaker volume, or automatic power-on is supported.

## Evidence from initial research

Apple states AutoMix requires supported devices and is unavailable in Apple Music for Windows; on Mac it requires Apple silicon: https://support.apple.com/en-ie/105067

JBL documents a computer Bluetooth limitation for PartyBoost: https://support.jbl.com/howto/pc-laptop-apple-mac-nintendo-switch-partyboost-support-us/000016490.html

JBL pairing compatibility: https://support.jbl.com/howto/partyboost-support-us/000035192.html

These establish design constraints, not a tested end-to-end system. Recheck current documentation before implementation and hardware recommendations.

## Project storage

GitHub: https://github.com/omgbrasco/house-music-remote

The private Google Drive AIOS project folder is the source of truth. GitHub is the public development mirror and the local checkout is a working copy. See AGENTS.md for the required start-of-session and handoff synchronization process. Private access details are stored only in Drive.

The proposed phone control panel is a Home Screen PWA, with a native Watch app for Digital Crown volume and playback controls. Both communicate with the house-player service; closing the phone panel must not stop music. This design is not yet implemented or tested on devices.

See ROADMAP.md for acceptance criteria and STATUS.md for setup state.
