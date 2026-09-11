# House Music Remote: agent handoff

## Authority and storage

The owner-designated private project workspace is the source of truth for project decisions and accepted current files. Authorized agents should obtain its location from the owner's private handoff, then read START-HERE.md and SYNC-MANIFEST.json there. GitHub is the public development mirror; a local checkout is a working copy. Private storage locations are intentionally not published here.

If Drive is inaccessible, state that the canonical state cannot be verified. Read-only work or clearly labeled proposals may continue, but do not claim synchronization or overwrite either side from stale context. Instructions cannot grant an agent access to Drive.

## Start and finish each work session

1. Read the canonical Drive handoff and manifest, then check GitHub main and local working-tree status. Compare against the recorded baseline, not timestamps alone.
2. Preserve independent changes. If Drive, GitHub, or local files diverge, reconcile explicitly; never force-push, delete versions, or use last-writer-wins.
3. Perform only the user's authorized project work. AutoMix is required. The proposed phone controller is a PWA; Watch controls require a native watchOS app. Both address the same house-player service. This architecture is not yet implemented or hardware-tested.
4. Before calling work complete, update the accepted files in Drive, publish only public-safe files to GitHub, and verify readback. Refresh the private manifest and handoff with the actual commit, file IDs, hashes, timestamp, and unresolved work.
5. If any write or verification fails, retain the working copy, mark synchronization incomplete, and report the single next remedy. A periodic check is a safety net, not a substitute for handoff synchronization.

## Public boundary

Do not publish private Drive URLs/IDs, local machine paths, account credentials, household inventory, or private operational notes. Keep these in the private Drive handoff. Public Git history must not incorporate the earlier private kickoff history. Use the public repository checkout.

## Product status

The repository currently contains planning documents, not a functioning app. First milestone: Apple Music AutoMix on a house player with global volume controlled from Apple Watch. Keep verified capabilities distinct from design intentions.
