# Fencelark 1.0 TEST
Native Android Yagit animal-separation fence puzzle. Android 8+ (min 26), target 35. Package com.gg007.fencelark.

## Rules
Yagit: tap internal grid edges to add or remove fences. Every field must contain at least one circle (goat) or at least one square (wolf), never both. Fences must start and end on the outside frame. Turn only at black posts, but a post may be passed straight or left unused. Fences cross straight through only away from black posts. No branches, dangling ends or closed fence loops. The twelve 3x3 puzzles have distinct post patterns, animal layouts and unique fence solutions. Undo/reset/next/levels and saved field palette/animal labels.

## Download and status
https://mega.co.nz/#!xIkXGCSD!01wu6s0CLWPC69QcChH5_5i82-n0_UFNcHSs0uvIvSc
APK SHA256 c6e215d5b2273cc919439ab03db4d62158766587a98ebf1bb4e1ad6507ecfadf; 20974 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous download bytes match.

## Checks
Independent selected-edge component oracle checks two boundary endpoints per fence; its cell BFS checks each field. It agrees with production ray tracing and union-find fields on all 49,152 fence boards across 12 levels and 120,000 invalid/random states. Exactly one solution per puzzle; all 12 post, animal and fence layouts distinct. Archived generator reproduces levels.json; archived Java exhaustive tests pass. Fixed clues, bounds, solved lock and solve/undo/replay/reset pass. Drawing adapter tests actual edge taps, ignored cell centers, reset/undo/next/levels/menu/settings/privacy and saved palette/animal labels/completion. Six actual drawing screens inspected, not phone screenshots. Phone runtime, performance and external-browser handoff QA remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Live 803-entry registry, 127 recovered partial READMEs and semantic review of all 154 prior studio cards found no Yagit match. GoatMath is livestock-planning arithmetic, not a fence puzzle. Cocoafold partitions fixed colors into matching shapes; Lassofem draws rectangular loops with room quotas. Fencelark instead checks boundary-to-boundary fence trajectories, post-only turns, nonpost crossings and animal separation. Known Yagit genre from Nikoli, not a global invention; recovered corpus is partial. Rules https://www.nikoli.co.jp/ja/puzzles/yagi_to_ookami/ https://www.janko.at/Raetsel/Yagit/index.htm https://www.cross-plus-a.com/html/cros7yagt.htm .

## Build
JDK 17 and Android SDK 35/build-tools35.0.0. python generate-levels.py reproduces levels.json. Board.java embeds generated post patterns/animals/fences. javac -d /tmp/fence-test src/com/gg007/fencelark/Board.java BoardTest.java and java -cp /tmp/fence-test com.gg007.fencelark.BoardTest. bash build.sh creates an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to private original signing inputs. No credentials in source. Release build settings, signed TEST artifact, not final store release.

## Privacy and branding
Fencelark runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Field palette, animal labels and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 icon byte-equal to original. Menu studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and websites
Complete source and APK privately preserved at https://files.instinct.com/48pns3qaubeo-fencelark-source-archive, including exact cumulative 155-card studio and published catalog/studio sources/updater. Repository https://github.com/iLanis-agent/fencelark holds README only; full Git source commit pending. Both website publications checked separately. No Pages settings change or Play rollout. November 7, 2026.
