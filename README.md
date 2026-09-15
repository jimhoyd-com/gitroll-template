# My Roll

A [GitRoll](https://github.com/jimhoyd-com/gitroll) Roll: a private, chronological record of what happened.

- `entries/YYYY/MM/<id>.md`: one Markdown file per event, with YAML front matter
- `projects/<slug>.yaml`: projects that events reference
- `attachments/<sha256>.<ext>`: photos, receipts and documents, named by content hash
- `.gitroll/types/<id>.yaml`: optional custom event types

Every file uses an ordinary format. Edit files directly, commit, and push; GitRoll picks up the changes.
Run `gitroll check` to validate the Roll locally. No GitHub Actions are needed.

**Keep this repository private.**

---

## Using this template

This repository is the starting point for a **Roll**, a private logbook for [GitRoll](https://github.com/jimhoyd-com/gitroll). It holds only starter data: no app code, scripts or GitHub Actions. You use it through the GitRoll app on your own computer.

Most people don't need this template: install GitRoll and run `gitroll setup`, which creates a private repository for you. Use the template if you'd rather create the repository yourself on GitHub (for example, in an organization, or with your own settings).

1. **Install GitRoll** on your computer. See [Install](https://github.com/jimhoyd-com/gitroll#install).
2. **Create your repository from this template.** Click **Use this template → Create a new repository**, pick the owner and a name, and choose **Private**. Leave "Include all branches" unchecked.
3. **Clone it** to your computer:

   ```bash
   git clone git@github.com:YOU/YOUR-ROLL.git
   ```

4. **Open it with GitRoll:**

   ```bash
   cd YOUR-ROLL
   gitroll
   ```

   GitRoll checks the files, adds the Roll to your list, and opens it. Use ↑↓ to browse, `n` to log, `/` to find, `s` to sync and `o` to open it in your browser. `gitroll rolls add .` adds it without opening.

5. **Name it:** `gitroll rename "Home"`. After that, log from anywhere with `gitroll log "what happened" --roll home`, and back up with `gitroll sync`.

### Good to know

- **Keep it private.** GitRoll refuses to sync to a public repository.
- **Upgrades don't touch your Roll.** New GitRoll versions read the same files, so there's nothing to update here. Upgrade the app with `gitroll upgrade`.
- **Changes to this template don't reach existing Rolls.** A repository created from a template is a copy, not a fork.
- **No GitHub Actions are needed.** Logging and syncing use none of your Actions minutes.
- **Questions or problems?** Open an issue on [jimhoyd-com/gitroll](https://github.com/jimhoyd-com/gitroll/issues). This repository is generated from [`template/`](https://github.com/jimhoyd-com/gitroll/tree/main/template) there on each release, so please don't open pull requests here.
