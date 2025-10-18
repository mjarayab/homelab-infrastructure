# Git and GitHub for DevOps - Study Notebook
## Mauricio Araya - DevOps Transition Notes

---

## Day 1-2: Fundamentals and First Complete Workflow

### 🎯 Main Objective
Convert my real homelab into a professional portfolio that demonstrates 
operational DevOps experience, not just theoretical knowledge.

### 📚 Key Concepts Learned

#### Git vs GitHub
- **Git**: Version control system (local)
- **GitHub**: Web platform that hosts Git repositories (remote)
- **Repository**: Project folder with change history

#### Branching Strategy (VERY IMPORTANT)
```
main branch = PRODUCTION (NEVER touch directly)
feature branches = Safe development
```

**Golden rule**: ALWAYS create branch for any change
- ✅ `git checkout -b descriptive-name`
- ❌ Work directly on `main`

#### Conventional Commits
Professional format for commit messages:
```
type: short description

- Detail 1
- Detail 2
- Detail 3
```

**Common types:**
- `feat:` New functionality
- `docs:` Documentation
- `fix:` Bug fixes
- `ci:` CI/CD changes

---

## 🛠️ Essential Commands Learned

### Initial Setup (one time only)
```bash
git config --global user.name "Mauricio Araya Badilla"
git config --global user.email "mjaraya@gmail.com"
git config --global init.defaultBranch main
```

### Basic Workflow
```bash
# 1. Check status
git status

# 2. Create new branch
git checkout -b docs/descriptive-name

# 3. Make changes (create/edit files)

# 4. Add files to staging
git add filename.md
# or git add . (all files)

# 5. Make commit
git commit -m "type: clear description"

# 6. Push to GitHub
git push origin branch-name

# 7. Create Pull Request on GitHub web
# 8. Merge PR
# 9. Clean local branch (optional)
git checkout main
git branch -d branch-name
```

### Verification Commands
```bash
pwd                    # Where am I?
ls -la                 # What files are here?
git status            # What branch? What changes?
git branch -a         # What branches exist?
git log --oneline -3  # See recent commits
```

---

## 🌿 Branch Workflow (Professional Process)

### Before any change:
1. **Check location**: `git status` 
2. **Create branch**: `git checkout -b type/description`
3. **Confirm change**: `git status` (should show new branch)

### During development:
4. **Make changes** (create folders, files, edit)
5. **Check changes**: `git status`
6. **Stage files**: `git add file` or `git add .`
7. **Professional commit**: `git commit -m "conventional message"`

### Publish work:
8. **Push to GitHub**: `git push origin branch-name`
9. **Create Pull Request** on GitHub web
10. **Merge after review**

---

## 🏗️ DevOps Portfolio Structure

### Professional Folder Architecture
```
homelab-infrastructure/
├── README.md                 # Project presentation
├── services/                # Production services
│   ├── pihole-production.md  # DNS filtering ✅ COMPLETED
│   ├── plex-media.md        # Media server (next)
│   └── gns3-labs.md         # Network labs
├── hardware/                # Physical infrastructure
│   ├── nuc-5i3-proxmox.md   # Main host
│   ├── nuc-6i5-vmware.md    # Dev environment
│   └── photos/              # Visual setup
├── network/                 # Topology and design
│   └── topology/
├── monitoring/              # Observability
└── docs/                   # Additional documentation
```

### Why this structure?
- **services/**: Demonstrates real operational experience
- **hardware/**: Shows infrastructure knowledge
- **network/**: Evidence of design thinking
- **monitoring/**: Signals DevOps mindset (observability)

---

## 🔐 GitHub Authentication

### Problem: Passwords don't work
GitHub NO longer accepts normal passwords for `git push`

### Solution: GitHub CLI (easier)
```bash
# Install (Mac)
brew install gh

# Authenticate
gh auth login
# Follow wizard: GitHub.com → HTTPS → Yes → Web browser
```

### Alternative: Personal Access Token
1. GitHub.com → Settings → Developer settings
2. Personal access tokens → Tokens (classic)
3. Generate new token → Check "repo" scope
4. **SAVE IN BITWARDEN** immediately
5. Use as password in terminal

---

## 🎯 My First Completed Project

### Pi-hole Production Service Documentation
**What I achieved:**
- ✅ Professional branch: `docs/add-service-uptime`
- ✅ File: `services/pihole-production.md`
- ✅ Conventional commit with detailed description
- ✅ Successful push to GitHub
- ✅ Pull Request #1 created and merged
- ✅ Complete technical documentation

**Why it's valuable for recruiters:**
- Demonstrates REAL production services
- Shows Proxmox + LXC knowledge
- Evidence of lifecycle management
- Includes learning roadmap (growth mindset)

---

## ❌ Common Mistakes and How to Avoid Them

### Mistake #1: Working on main branch
**Symptom**: `git status` says "On branch main"
**Solution**: ALWAYS create branch before changes
```bash
git checkout -b my-feature  # BEFORE making changes
```

### Mistake #2: Incorrect user configuration
**Symptom**: Commits appear with system hostname
**Solution**: Configure Git globally from the start
```bash
git config --global user.name "Real Name"
git config --global user.email "email@github.com"
```

### Mistake #3: Vim problems
**Symptom**: Confusing editor opens on commit
**Solution**: Use one-line commits or configure nano
```bash
git config --global core.editor nano  # Use nano instead of vim
```

### Mistake #4: Multiline commits in terminal
**Symptom**: `dquote>` appears and can't exit
**Solution**: `Ctrl + C` to cancel, use shorter message

---

## 📈 Next Steps Roadmap

### This Week
- [ ] Document Plex Media Server
- [ ] Create hardware documentation (NUCs)
- [ ] Take professional setup photos

### Next Week  
- [ ] Basic GitHub Actions for validation
- [ ] Impressive Profile README
- [ ] Issues templates for incident management

### Next Month
- [ ] GitHub Pages for portfolio website
- [ ] Additional projects (scripts, automation)
- [ ] Open source contributions

---

## 💡 Important Insights

### DevOps Mindset
- **Document EVERYTHING**: If it's not documented, it doesn't exist
- **Automation mindset**: Always think how to automate
- **Infrastructure as Code**: Treat infrastructure like code
- **Fail fast, learn faster**: Mistakes are learning opportunities

### Differentiators for Recruiters
1. **Real services vs demos**: My Pi-hole has operational history
2. **Lifecycle management**: Hibernation/reactivation shows pragmatism
3. **Learning roadmap**: Demonstrates growth mindset
4. **Conventional commits**: Following industry standards

### My Competitive Advantage
- Intel background (industrial processes)
- Current digital transformation leadership
- Real physical infrastructure (not just cloud)
- Engineering mindset applied to DevOps

---

## 🔄 Quick Reference Commands

```bash
# Initial setup
git clone https://github.com/user/repo.git
cd repo

# Basic workflow
git checkout -b feature/new-functionality
# make changes
git add .
git commit -m "feat: clear description"
git push origin feature/new-functionality

# Constant verification
git status           # Where am I? What changes?
pwd                  # What folder am I in?
ls -la              # What files are here?

# Emergencies
Ctrl + C            # Cancel current command
git checkout main   # Return to main branch
git stash          # Save changes temporarily
```

---

## 📝 Personal Notes

### What was most difficult?
- Understanding branch concept (but now I get it)
- Vim confuses me, better use nano
- Remembering to do `git status` before each action

### What I liked most?
- Seeing my professional documentation on GitHub
- Completed Pull Request #1
- Having a workflow I can repeat

### What I need to practice more?
- Conventional commits (message + description)
- Check branch before making changes
- Python and Bash scripting for next projects

---

## 🏆 Current Status
- **Git configured**: Mac and Windows ✅
- **First workflow completed**: Branch → Commit → Push → PR → Merge ✅
- **Professional documentation**: Pi-hole service documented ✅
- **Repository structure**: Following DevOps best practices ✅

---

## 🎯 Success Metrics
- ✅ Consistent commits (5+ per week goal)
- ✅ 3+ well-documented repositories
- ✅ Professional Issues and PRs with templates
- ✅ Working GitHub Actions
- ✅ Deployed portfolio website
- ✅ Standout Profile README

---

*Last updated: September 15, 2024*  
*Next session: Document Plex Media Server*
