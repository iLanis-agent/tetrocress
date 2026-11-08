# Tetrocress 1.0 TEST
Native Android Tetrominous. These small boards are original generated layouts. Android 8+ (min 26), target 35. Package com.gg007.tetrocress.

## Rules
Tetrominous. Cover the whole 4x4 grid with nonoverlapping edge-connected four-cell shapes. Gold letters give the shape type: I line, L hook, O square, S zigzag, T tee. Rotations and reflections count as the same type. Equal types cannot share a side; corner contact is allowed. A shape can contain multiple matching letters or no letter. No fixed inventory, no four-corner restriction, no shaded sea and no falling-block mechanics. Tap internal borders to add/remove fences. Outer frame stays fixed. Eight original unique clue boards with eight different completed partitions. This small edition has exactly eight legal base partitions; their shapes are I,L,S. O and T are supported and tested by the classifier but do not occur in these eight solutions. Undo/reset/next/levels and saved shape palette/current shape-label settings.

## Download and status
https://mega.co.nz/#!FNkwlB4J!5gzrTW6QmH6HA32fU-6huEE71xPR2tE271ZT_o-FR9M
APK SHA256 f2e22bf280689832d729fd8b44fc2cfcb1ab28d68af09526d9dd0838b3b3b1df; 20974 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous download bytes match.

## Checks
Original generator builds all 113 tetromino placements by rotation/reflection, enumerates all 117 complete 4x4 tilings, then retains exactly eight with equal-shape side separation. All eight clue boards have one partition and eight different solutions. Independent Java canonical rotation/reflection classifier agrees with production degree/bounding-box/straight-three classifier on every 65,536 cell subset; independent exact-cover search also recovers all 117 tilings and eight legal partitions. Independent union-find fence oracle checks all enumerated tilings against production flood-fill, plus 120,000 random/invalid fence masks and clue arrays, 192 single-fence solution mutations, null/invalid clue sizes/values, bounds, solved lock and solve/undo/replay/reset. Archived portable generator reproduces levels.json, all-solutions.json and all-partitions.json; archived Java tests pass. Drawing adapter tests actual fence taps, undo/replay/next/levels/menu/settings/privacy and saved palette/current-shape labels/completion. Six drawing screens inspected, not phone screenshots. Phone runtime, performance and external-browser handoff QA remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Live 803-entry registry and semantic review of all 162 prior studio cards found no Tetrominous match. Triowillow uses orientation-sensitive trios; Timberfen shades LITS in existing rooms; Statuefern places a separated L/T bank in a connected white sea; Stonefence counts fenced cell sides. Tetrocress instead covers all cells with four-cell letter-typed regions and forbids equal types across a side regardless of turning/mirroring. Known Tetrominous genre, not a global invention. WPF2018 http://gp.worldpuzzle.org/sites/default/files/Puzzles/2018/2018_PuzzleRound6.pdf explicitly allows multiple letters per piece. https://wpcunofficial.miraheze.org/wiki/Polyominous agrees on shape separation. No source puzzle copied; original generated clue boards. Recovered repository corpus remains partial.

## Build
JDK 17 and Android SDK 35/build-tools35.0.0. python generate-levels.py reproduces levels.json. Board.java embeds generated shape-letter clues and fence solutions. javac -d /tmp/tetro-test src/com/gg007/tetrocress/Board.java BoardTest.java and java -cp /tmp/tetro-test com.gg007.tetrocress.BoardTest. bash build.sh creates an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to private original signing inputs. No credentials in source. Release build settings, signed TEST artifact, not final store release.

## Privacy and branding
Tetrocress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Shape palette, current shape labels and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 icon byte-equal to original. Menu studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and websites
Complete source and APK privately preserved at https://files.instinct.com/59kwj07zg9bc-tetrocress-source-archive, including exact cumulative 163-card studio and published catalog/studio sources/updater. Repository https://github.com/iLanis-agent/tetrocress holds README only; full Git source commit pending. Both website publications checked separately. No Pages settings change or Play rollout. November 8, 2026.
