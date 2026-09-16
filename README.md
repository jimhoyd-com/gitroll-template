# My Roll

A [GitRoll](https://github.com/jimhoyd-com/gitroll) log.

Events live in [`.gitroll/events/`](.gitroll/events), one Markdown file each, and the files kept
with them live in `.gitroll/files/`. [`.gitroll/README.md`](.gitroll/README.md) explains the
format and has a copyable example.

To log something: create `.gitroll/events/2026-09-15-ac-serviced.md`, write what happened, then
commit and push. Nothing has to be installed.

This log is as visible as this repository: keep it private if what you log is private.

---

## Using this template

This repository is the starting point for a **Roll**: a log kept as ordinary Markdown files in Git. Everything GitRoll knows about lives in [`.gitroll/`](.gitroll), and that folder is committed like the rest of the repository.

You do not need [GitRoll](https://github.com/jimhoyd-com/gitroll) to use it. Git and a text editor are enough; [`.gitroll/README.md`](.gitroll/README.md) is the whole format. GitRoll is an optional app that reads and writes the same files.

1. **Create your repository from this template.** Click **Use this template → Create a new repository**, pick the owner and a name, and choose **Private** if what you log is private.
2. **Clone it** to your computer:

   ```bash
   git clone git@github.com:YOU/YOUR-ROLL.git
   ```

3. **Log something.** Create `.gitroll/events/2026-09-15-ac-serviced.md`, write what happened, then:

   ```bash
   git add .gitroll
   git commit -m "AC serviced"
   git push
   ```

4. **Optionally, open it with GitRoll:**

   ```bash
   cd YOUR-ROLL
   gitroll
   ```

   GitRoll checks the files, adds the Roll to your list, and opens it. Use ↑↓ to browse, `n` to log, `/` to find, `s` to sync and `o` to open it in your browser. `gitroll rolls add .` adds it without opening.

### Good to know

- **The log is as visible as the repository.** `.gitroll/` is a namespace, not a privacy boundary: in a public repository, every event and every file in it is public. GitRoll refuses to sync a Roll to a public repository.
- **`.gitroll/config.yaml` records the template version** this repository follows. GitRoll reads it, and never changes it while logging or editing.
- **Already have a project?** You don't need this template. Run `gitroll` inside that repository and choose *Add a log to this repository*: only `.gitroll/` is created, and nothing else is touched.
- **Upgrades don't touch your log.** New GitRoll versions read the same files. Upgrade the app with `gitroll upgrade`.
- **No GitHub Actions are needed.** Logging and syncing use none of your Actions minutes.
- **Questions or problems?** Open an issue on [jimhoyd-com/gitroll](https://github.com/jimhoyd-com/gitroll/issues). This repository is generated from [`template/`](https://github.com/jimhoyd-com/gitroll/tree/main/template) there on each release, so please don't open pull requests here.
