# TiltZone · בריף פרויקט (להעברה ל-Claude Code)

> מסמך הקשר מלא על עמוד האינסטגרם TiltZone, הקורס "פוקר מאפס", כל מה שהופק עד היום, ולאן הפרויקט הולך.
> עודכן: 28.10.2026 · בעלים: נריה

---

## 1. מה זה TiltZone

- **עמוד אינסטגרם** בשם TiltZone, שעליו רץ הקורס **"פוקר מאפס"**: קורס פוקר בעברית, מהבסיס ועד רמה מתקדמת.
- **מבנה הקורס:** 31 פרקים. כל פרק הוא ריל אחד (אינסטגרם/טיקטוק), באורך 1–3 דקות.
- **קהל יעד:** מתחילים ישראלים, צעירים, בלי ידע קודם. משחק Cash, שולחן 6 שחקנים, 100BB.
- **המטרה הבאה:** להפוך את העמוד מעמוד תוכן ל**קהילת פוקר** (ראו סעיף 7).

## 2. כללי תוכן (חובה)

1. **עברית, RTL.** מונחי פוקר נכתבים **באותיות אנגליות**: Raise, Fold, BTN, C-Bet ולא "רייז".
2. **בלי קריינות.** המנוי ל-ElevenLabs בוטל, אז הכל מוסבר ויזואלית בטקסט על המסך, בקצב שאפשר לקרוא.
3. **לוגו TiltZone בכל סרטון וסטורי.**
4. **ריל:** אנכי 1080×1920, ‏30fps, בין דקה ל-3 דקות.
5. **כל ריל נגמר ב-CTA:** "שמור לפני המשחק הבא" + "בפרק הבא: X" + "עקוב כדי לא לפספס".
6. **חידונים בתוך הרילים:** ספירה לאחור 3-2-1 ואז תשובה עם הסבר. זה הפורמט שעובד הכי טוב.
7. **תיאורים (captions):** פתיחה עם hook ואימוג'י, 1–2 שורות תוכן, "פרק X מתוך 31", שאלה לתגובות, ו**עד 5 האשטגים** (הבקשה האחרונה של נריה). דוגמה: `#פוקר #פוקרמאפס #TiltZone #poker #postflop`.
8. **ישראל:** הימורים על כסף אמיתי באונליין לא חוקיים. לא מפרסמים אתרי הימורים ולא עושים affiliate.

## 3. מיתוג: שתי שפות עיצוב

| | **חלק 1** (פרקים 1–6, PREFLOP) | **חלק 2** (פרק 7 ואילך, POSTFLOP) |
|---|---|---|
| רקע | לבד ירוק (`#0e3a2b` → `#072319`) | כחול לילה (`#06081a` / `#0f1438`) + רשת עדינה |
| הדגשה | זהב `#e8b64c` | טורקיז `#38e4d0` (+ סגול `#8b7bff`, קורל `#ff5f6d`, מנטה `#5ee39b`) |
| פונט כותרות | Karantina | Rubik 900 |
| פונט טקסט | Heebo | Heebo |
| מסגרת | מסגרת זהב מעוגלת | מסגרות בפינות בסגנון HUD (טורקיז) |
| לוגו | ז'יטון זהב, "TZ" על ירוק | ז'יטון כחול-טורקיז זוהר, T לבן + Z טורקיז |

- **לוגו v1:** `brand/logo.py`. קבצים: `brand/tiltzone-logo.png`, `tiltzone-avatar.png`, `tiltzone-profile.png`
- **לוגו v2:** `brand2/logo2.py`. קבצים: `brand2/tiltzone-logo-v2.png` (שקוף), `tiltzone-avatar-v2.png`, `tiltzone-profile-v2.png`
- **החלטה פתוחה:** האם v2 מחליף את v1 כלוגו הראשי (כולל תמונת הפרופיל), או רק מלווה את חלק 2. ההמלצה הייתה לבחור אחד.

## 4. מה הופק עד היום

### רילים (הקורס)
| # | נושא | תוכן עיקרי | עיצוב |
|---|---|---|---|
| 1 | חוקי המשחק | 2 קלפים + 5 משותפים, 4 סבבים, Check/Bet/Call/Raise/Fold, 5 מתוך 7, דירוג ידיים | ירוק |
| 2 | הכפתור והבליינדים | Button, SB/BB, סדר פעולה, Pot/Stack/Effective stack | ירוק |
| 3 | מיקום | UTG מול BTN, יתרון מידע, שליטה בקופה, UTG ‏15% מול BTN ‏40% | ירוק |
| 4 | טבלאות פתיחה | גריד 169 ידיים, בלי Limp (3 סיבות), טבלה לכל מקום: UTG 15 / MP 20 / CO 27 / BTN 42 / SB 37 | ירוק |
| 5 | מישהו העלה לפניך | 3-Bet לערך (QQ+, AK) ובלוף (A5s, A4s), פי 3 עם מיקום ופי 4 בלי, Call, SB = 3-Bet או Fold, Squeeze ~12BB, מול 3-Bet. גרסה 5b בנויה מחידון של 7 ידיים | ירוק |
| 6 | הגנה על הבליינדים | חשבון 27% (‏1.5 מתוך 5.5), מול BTN לעומת UTG, ‏SB, suited. חידון של 7 ידיים | ירוק |
| 7 | קריאת הבורד | בורד יבש/רטוב, 3 שאלות (צבע/רצף/זוג), Rainbow/Two-tone/Monotone, סקאלה, חידון של 3 בורדים | **כחול (חלק 2)** |
| 8 | Outs וסיכויים | ספירת Outs, טבלת draws, כלל 2 ו-4, pot odds, טבלת גודל הימור → אחוז נדרש (17/25/30/33), Implied odds, חידון | **כחול** |
| 9 | C-Bet | מה זה, למה עובד (‏~1/3 פגיעה), מתי כן ומתי לא, גודל 1/3 מול 2/3, אחוז Fold נדרש (25/33/40/50), חידון של 3 ידיים | **כחול** |

> פרק 10 כבר הובטח בסוף ריל 9: **"מה עושים כשעושים לך C-Bet"**.
> שימו לב: סדר הנושאים של פרקים 7–9 נבחר בלי רשימת פרקים כתובה. **רשימת 31 הפרקים המלאה לא מתועדת**, וזה החור הכי גדול בתכנון. (טיוטה: `chapters.md`)

### פוסטים (קרוסלות)
- **סדרה מוקדמת** (`carousel1–3`): "5 הטעויות של מתחילים" (7 שקפים), "איך תשחק A-8? תלוי איפה אתה יושב" (8), "הטבלה הזאת נראית מסובכת?" (8).
- **פוסטים מלווים לפרקים** (`posts/out/p1–p3`):
  1. כל טבלאות הפתיחה (11 שקפים, ההסבר המלא לפרק 4)
  2. המדריך המלא לפרי-פלופ (11 שקפים, פרק 5)
  3. הגנה על הבליינדים (8 שקפים, פרק 6)

### סטוריז
- סקר קצב: "איך הקצב? עברנו כבר 3 פרקים"
- תיבת שאלות: "מה חסר לכם?"
- סקר קריינות: "כמה הקול חשוב?" (+ דמו בלי קול)
- **סטורי הכרזה על העיצוב החדש** (‏26 שניות, `story3/story-new-design.mp4`): העיצוב הירוק "קורס" בגליץ' ← SYSTEM ERROR ← מסך מתנפץ ← "02" ← POSTFLOP ← קלפים שמתהפכים ל"עיצוב חדש!" ← הלוגו החדש ← "פרק 7 בחוץ"

### נוספים
- **סרטון וואטסאפ לחברים** (‏30 שניות, `story4/tiltzone-whatsapp.mp4`): הכרזה חובבנית-מצחיקה עם WordArt, צופרים, זום דרמטי, קבלה עם "שפיות: אבדה", משקפי "תתמודדו 😎", ואיום חביב על הז'יטונים של פוקר שישי.
- **סרטון סיכום ארוך לחלק 1** (‏31 דקות, לרוחב 1920×1080, `master/poker-zero-part1-summary.mp4`): לשימוש אישי ולא לאינסטגרם. 8 פרקים, הסבר פשוט מאוד, עשרות דוגמאות, 24 חידונים, יד שלמה מההתחלה עד הסוף, ודף לשמירה. בעיצוב החדש.

## 5. תוכנית הקורס

- **חלק 1 · PREFLOP** (פרקים 1–6): הושלם.
- **חלק 2 · POSTFLOP** (פרק 7 ואילך): בתהליך. 7–9 מוכנים, 10 הובטח (הגנה מול C-Bet).
- **פרקים 11–31:** לא הוגדרו. הצעה לחלק 2 ואילך: Double barrel / משחק על ה-Turn, River ו-value bet, גודל הימורים, Check-raise, מיקום אחרי ה-flop, קריאת יריבים וסוגי שחקנים, ניהול בנקרול, טילט ומיינדסט, טורנירים מול Cash, ניתוח ידיים.
- **צעד ראשון מומלץ:** לכתוב ולאשר את רשימת 31 הפרקים לפני שממשיכים להפיק.

## 6. החלטות שכבר התקבלו

- בלי קריינות, הכל ויזואלי.
- עיצוב חדש לכל פתיחה של חלק בקורס (חלק 2 = כחול-טורקיז).
- טווחים פשוטים למתחילים ולא GTO מלא. תמיד מציינים "נקודת התחלה, לא חוק".
- חידונים הם חלק קבוע מהפורמט.

## 7. לאן הולכים: עמוד ← קהילה

רעיונות שעלו (מהחזק לחלש):
1. **"יד השבוע":** יד קשה עם "מה עושים?", ותשובה עם הסבר למחרת.
2. **סטוריז אינטראקטיביים:** סקר Call/Fold/Raise, ואז הסבר.
3. **שליחת ידיים מהקהל** (בהודעה פרטית) וניתוח שלהן, בלי שמות.
4. **קבוצת וואטסאפ** (קטנה) או **דיסקורד** (כשגדלים).
5. **משחק חודשי פיזי** על שולחן הפוקר ה-DIY שנריה בונה (אובלי, LED, מסך דילר), עם דירוג ופרסים סמליים או בלי כסף.
6. ניתוח סרטונים של עוקבים.
7. שיתופי פעולה עם עמודי פוקר ישראליים קטנים.

**הערות כנות:**
- ההימורים בישראל מוגבלים מאוד. טורנירים עם כסף, במיוחד פתוחים לציבור, דורשים בדיקה משפטית לפני שמתחילים.
- קהילה צריכה קודם בסיס עוקבים פעיל. כדאי לדעת כמה עוקבים יש ומי הם לפני שמשקיעים.

## 8. Technical pipeline (for Claude Code)

> All source currently lives in a **cloud workspace at `/home/claude/`**, not on Neriya's machine. To continue there, copy the project folder (minus `node_modules` and renders) to the local machine first.
> Note (28.10.2026): the Claude Code session that received this brief has an empty `/home/claude/`. The source was not carried over and still needs to be uploaded.

**How a video is made**
1. **Python build script** (`reelN/build.py`) generates a single HTML page: a 1080×1920 `#stage`, scenes as `<section class="scene" data-s data-e>`, elements animated with CSS keyframes + `--d` delay (`class="a up|pop|deal|flip..."`).
2. **Timeline engine** (copied from `reel1/reel1.html`, after `<div class="ctrl">`): in `#record` mode it exposes `window.__seek(t)` (pauses all animations and sets `currentTime`) and `window.__total`.
3. **Render:** `frames.js` (Playwright Chromium) → seeks every 1/30 s → JPEG screenshots piped to `ffmpeg` (libx264, crf 18, yuv420p).
4. **Audio:** `music.py` (numpy/scipy synth: Part 2 = Cm–Ab–Eb–Bb, 94 BPM, plucked arps, half-time drums) + `sfx.py` (whoosh/tick/ding/deal/pop from `sfx.json` timestamps the build script emits) → mixed with ffmpeg or numpy (music ~0.5, sfx ~0.9).
5. **Fonts:** `@fontsource/{heebo,karantina,rubik}` from `reel1/node_modules`, embedded via `@font-face` (no network).

**Key files**
- `part2/common.py`: Part 2 reel framework. `Reel(num,title).scene(dur, html, fx=[...])`, `card()/cards()`, `caps()` (timed captions), `countdown()` (quiz), `hand_board()`, `A(anim, delay, html, tag, cls)`, `build(dir)` → `rec.html` + `sfx.json` + `meta.json`.
- `part2/frames.js`, `part2/music.py`, `part2/sfx.py`, `part2/mix.sh N`
- `reel6/builder.js`: renders the 13×13 range grid (`.grid[data-cfg]`, tokens like `22+ A2s+ KTs+ AJo+`) and the 6-max table with seats/bets/dealer (`.tbl[data-cfg]`).
- `master/common.py`: landscape (1920×1080) variant, `Chapter` class, `table()`, `grid()`, `quiz()`, `say()`.
- `brand/logo.py` (v1), `brand2/logo2.py` (v2): `logo(h)` returns inline SVG+HTML.

**Gotchas already solved**
- Don't reuse the class name `.st` on card inners (it collided with a step-row style and broke card width). The static card inner is `.stc`.
- `.cap` is a flex container: wrap caption text in `<span>` or the spaces around `<b>` collapse.
- Animations with `fill-mode: both` show their 0% keyframe **before** the delay, so overlays (noise/bands/blackout) must start at `opacity:0`.
- An animated `transform` overrides a static positioning transform: put the positioning on a wrapper element.
- Bidi: wrap English/numbers in `<span class="en">` (`direction:ltr; unicode-bidi:isolate; white-space:nowrap`). In Hebrew sentences use `←` (the build swaps `→` to `←`).
- Render cost: ~1000 frames/min across 3 parallel workers on 2 cores. A 2.5-minute reel takes about 5–8 minutes.

## 9. Open items

- [ ] Write and approve the full 31-chapter list (biggest gap). Draft: `chapters.md`.
- [ ] Chapter 10: "What to do when someone C-Bets you" (already teased).
- [ ] Decide: is logo v2 the main logo or Part 2 only?
- [ ] Community: pick the first 1–2 initiatives (e.g. "Hand of the week" + WhatsApp group).
- [ ] Find out the current follower count and audience (beginners vs. players).
- [ ] Upload the production source (`part2/`, `reel*/`, `brand*/`, `master/`) into this repo.
