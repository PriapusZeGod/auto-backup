# 🛡️ auto-backup

A Bash-based automation tool that backs up your `~/Documents` directory with compression and timestamped archive names. Built as part of my journey into DevOps and Cloud Infrastructure engineering.

## 🔧 What It Does

- Backs up your `~/Documents` directory
- Compresses the backup into a `.tar.gz` file
- Adds a timestamp to every backup archive (e.g. `2025-06-03-Backup-Documents.tar.gz`)
- Logs each action (start, success, errors, location)
- Prepares the ground for future features like cron scheduling and flag-based config

## 📂 Example Output

After running:

./auto-backup


You’ll see something like this:

~/Backups/2025-06-03-Backup-Documents.tar.gz


And logs will be written to:

./logs/backup.log


## 🛠️ Why I Made This

I wanted to practice:
- Shell scripting for real-world automation
- Building projects from scratch instead of following a tutorial
- Thinking like a DevOps/Platform engineer: logs, structure, backups, clean code

## 📌 Planned Features
- [ ] Add CLI flags: `--source`, `--dest`, `--no-log`, `--dry-run`
- [ ] Setup `cron` support for scheduled backups
- [ ] Email or system notification after success/failure
- [ ] Archive cleanup (delete older than X days)

## 📚 What I Learned
This project helped me understand:
- Real Bash scripting workflows
- File operations, logging, conditionals
- Good Git hygiene and clean project structure
- The DevOps mindset of building flexible, safe tooling

## 🚀 How to Run

```bash
chmod +x backup.sh
./backup.sh

Make sure the ~/Documents folder exists, and that you have write permissions to ~/Backups.
```

---

📁 Part of my DevOps learning series — more tools coming soon.