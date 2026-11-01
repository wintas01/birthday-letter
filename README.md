# 🎂 Birthday Letter

A little interactive birthday surprise you can send to someone you love: a wax-sealed envelope, a birthday card with a song, a swipeable photo album, a bouquet of flower wishes, and a heartfelt letter at the end.

**Live demo:** https://wintas01.github.io/birthday-letter/

It's a single `index.html` file with no build step, no framework and nothing to install. It works on phones and desktops.

## What's inside

1. **Envelope:** tap the seal to open it (with confetti 🎉)
2. **Birthday card:** a personal message and a built-in song player
3. **Photo album:** swipe or tap through up to 5 memories with captions
4. **Bouquet:** three flowers that flip over to reveal birthday wishes
5. **Letter:** a final heartfelt letter, signed by you

The default song is a romantic slow-waltz version of *Happy Birthday*, generated in the browser. It needs no audio file and has no copyright issues. You can swap in your own `.mp3` instead.

## Make your own (5 minutes, no coding needed)

### 1. Copy the project

Click **Fork** at the top of this page to get your own copy. Or download `index.html` and host it anywhere.

### 2. Add your photos

1. In your copy, open the `photos` folder.
2. Click **Add file → Upload files** and drag your pictures in.
3. Use simple names with no spaces, like `1.jpg`, `2.jpg`. Names are case-sensitive, so `1.JPG` is not the same as `1.jpg`.
4. Keep each photo under about 2 MB so the page loads fast on phones.

### 3. Edit the words

Open `index.html`, click the ✏️ pencil icon and find the section marked **`EDIT EVERYTHING HERE ✏️`** (near the bottom). Everything you need is in that one block:

| Setting    | What it changes |
|------------|-----------------|
| `hello`    | The greeting on the envelope screen |
| `name`     | What you call them, shown on the card and letter |
| `from`     | Your signature at the end of the letter |
| `message`  | The message on the birthday card |
| `songUrl`  | A direct link to an `.mp3`. Leave it `""` to use the built-in song |
| `songNote` | The little handwritten note under the song |
| `memories` | Album photos and captions, e.g. `photo:"photos/1.jpg"` |
| `wishes`   | The 3 notes hidden inside the flowers |
| `popMsg`   | The pop-up after all flowers are opened |
| `letter`   | The final letter, one paragraph per line |

For example, to use a photo:

```js
{ photo:"photos/1.jpg", doodle:"bouquet", caption:"our first trip together 💕" },
```

If `photo` is left empty (`""`), a cute bunny doodle is shown instead. The doodle can be `bouquet`, `balloon`, `cake`, `gift`, `hat` or `heart`.

**Tips:**
- Only change the text **inside the quotes**, and keep the commas between items.
- If your text needs a double quote, write it as `\"`.

Click **Commit changes** when you're done.

### 4. Put it online (free)

1. In your repo go to **Settings → Pages**.
2. Under **Source** pick **Deploy from a branch**, then choose `main` and `/ (root)`, and click **Save**.
3. After a minute or two your page is live at `https://<your-username>.github.io/<repo-name>/`.
4. Send the link to the birthday person 🎁

After any edit, wait a minute and hard-refresh the page (Ctrl+Shift+R, or Cmd+Shift+R on Mac) to see the changes.

## Notes

- Music only starts after a tap. Browsers block sound until the visitor interacts with the page.
- Anyone with the link can see the page, so only use photos you're happy to share.

## License

[MIT](LICENSE). Feel free to use, change and share it. Make someone smile ♡
