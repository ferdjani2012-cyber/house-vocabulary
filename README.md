# Houses & Furniture Game

An offline-ready English game for young learners (A1–A2) built around a house and its furniture.

## Main menu

The game opens on a menu with four skills:

1. **Vocabulary & Yes/No Questions** — a room is drawn on screen and the student answers
   *“Is there a sofa in the living room?”* / *“Are there two chairs in the kitchen?”* with Yes/No.
   A correct answer highlights the item and zooms the picture in on it.
2. **Prepositions of Place** — *“Where is the lamp?”* with four phrases to choose from
   (*next to the sofa*, *on the wall*, *in the corner of the room* …). An arrow points at the item.
3. **Adjectives & Listening** — one recorded sentence is played
   (*“In the kitchen, there is a big white modern fridge.”*) and the student picks the matching
   sentence out of four, all sharing the same nouns and differing only in adjectives.
4. **Word practice** — the original word quizzes: 74 words in 4 sets, with picture → word,
   listen → picture, spelling and memory rounds, in Standard or Challenge mode.

A single score is kept across the three skill sections and saved in the browser (`localStorage`),
so it survives a page reload. It can be reset from the menu.

## Notes for teachers

- Everything runs from one `index.html`: illustrations are inline SVG, all word and sentence
  audio is embedded as base64 MP3, so the game works with no internet connection.
- The three room scenes (living room, kitchen, bedroom, bathroom) are assembled from the same
  illustration library, so they match the rest of the game.
- Questions, options and scene layouts live in plain JavaScript arrays at the top of the file
  (`SCENES`, `SEC1`, `SEC2`, `SEC3` in the “main menu + skill sections” block at the end).
- Works on phones (from 320 px wide), tablets and computers. Keyboard: `Y`/`N` or `1`/`2` for
  Yes/No, `1`–`4` to pick an option, `Enter` for the next question, `Space` to replay the audio.

Open `index.html` locally, or publish the folder with GitHub Pages.

Made for classroom use.
