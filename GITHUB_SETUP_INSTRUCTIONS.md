# GitHub Repository Setup Instructions
## How to Organize Your IDRIS Business Package

**Goal:** Create a professional GitHub repository with all IDRIS business materials properly organized.

---

## 📦 Step 1: Download All Files

Download these files from your outputs:

**Core Documents:**
- [ ] README.md
- [ ] REPOSITORY_STRUCTURE.md
- [ ] IDRIS_Executive_Summary.md
- [ ] idris_business_plan.md
- [ ] idris_founding_team_analysis.md
- [ ] IDRIS_Startup_Costs_Breakdown.md

**Website Files:**
- [ ] index.html
- [ ] idris-website.html (backup)
- [ ] IDRIS_Website_Deployment_Guide.md
- [ ] README_DEPLOYMENT.md

**Presentation:**
- [ ] IDRIS_Business_Plan_Presentation.pptx

---

## 🗂️ Step 2: Create Folder Structure

On your computer, create this folder structure:

```bash
# Create main folder
mkdir idris-business-package
cd idris-business-package

# Create subfolders
mkdir Executive_Summary
mkdir Business_Plan
mkdir Team_Analysis
mkdir Financial
mkdir Website
mkdir Presentation
mkdir Guides  # Optional for future additions
```

---

## 📁 Step 3: Organize Files

Move downloaded files into appropriate folders:

### Root Directory
```bash
# Move to root
mv ~/Downloads/README.md ./
mv ~/Downloads/REPOSITORY_STRUCTURE.md ./
```

### Executive_Summary/
```bash
mv ~/Downloads/IDRIS_Executive_Summary.md ./Executive_Summary/
```

### Business_Plan/
```bash
mv ~/Downloads/idris_business_plan.md ./Business_Plan/
```

### Team_Analysis/
```bash
mv ~/Downloads/idris_founding_team_analysis.md ./Team_Analysis/
```

### Financial/
```bash
mv ~/Downloads/IDRIS_Startup_Costs_Breakdown.md ./Financial/
```

### Website/
```bash
mv ~/Downloads/index.html ./Website/
mv ~/Downloads/idris-website.html ./Website/
mv ~/Downloads/IDRIS_Website_Deployment_Guide.md ./Website/
mv ~/Downloads/README_DEPLOYMENT.md ./Website/
```

### Presentation/
```bash
mv ~/Downloads/IDRIS_Business_Plan_Presentation.pptx ./Presentation/
```

---

## 🔧 Step 4: Create GitHub Repository

### Option A: Via GitHub Website (Easiest)

1. **Go to GitHub.com**
   - Sign in to your account
   - Click "+" icon (top right)
   - Select "New repository"

2. **Repository Settings**
   - Repository name: `idris-business-package`
   - Description: "Complete business launch package for IDRIS - Institute for Data-Driven Research & Innovation"
   - Visibility: 
     - **Private** (recommended initially - only you and collaborators can see)
     - **Public** (if you want to share openly)
   - Initialize with:
     - ✅ Add a README file (UNCHECK - we have our own)
     - ⬜ Add .gitignore (leave unchecked)
     - ⬜ Choose a license (leave unchecked for now)
   
3. **Click "Create repository"**

### Option B: Via Command Line

```bash
# Initialize git in your local folder
cd idris-business-package
git init

# Create README if not already there
# (You should already have README.md from downloads)

# Add all files
git add .

# Initial commit
git commit -m "Initial commit: Complete IDRIS business package"

# Create repository on GitHub (use GitHub CLI if installed)
gh repo create idris-business-package --private --source=. --remote=origin

# Or manually: Go to github.com, create repo, then:
git remote add origin https://github.com/YOUR-USERNAME/idris-business-package.git
git branch -M main
git push -u origin main
```

---

## 📤 Step 5: Upload Files to GitHub

### Method 1: Drag & Drop (Easiest for non-developers)

1. Go to your repository on GitHub.com
2. Click "Add file" → "Upload files"
3. Drag your entire `idris-business-package` folder structure
4. Add commit message: "Add complete IDRIS business package"
5. Click "Commit changes"

**Note:** This uploads everything at once, maintaining folder structure.

### Method 2: Git Command Line

```bash
# From your idris-business-package directory
cd idris-business-package

# Add all files
git add .

# Check what will be committed
git status

# Commit with message
git commit -m "Add complete IDRIS business package

- Executive summary and business plan
- Founding team analysis
- Financial projections and startup costs
- Production-ready website
- PowerPoint presentation with charts
- Deployment guides and documentation"

# Push to GitHub
git push -u origin main
```

---

## ✅ Step 6: Verify Upload

1. Go to your repository on GitHub.com
2. Check that you see:
   - README.md displays as the main page
   - All folders visible (Executive_Summary, Business_Plan, etc.)
   - Files in each folder
   - Presentation file uploadable

**Your repository should look like:**
```
idris-business-package/
├── README.md (displays on main page)
├── REPOSITORY_STRUCTURE.md
├── Executive_Summary/
│   └── IDRIS_Executive_Summary.md
├── Business_Plan/
│   └── idris_business_plan.md
├── Team_Analysis/
│   └── idris_founding_team_analysis.md
├── Financial/
│   └── IDRIS_Startup_Costs_Breakdown.md
├── Website/
│   ├── index.html
│   ├── idris-website.html
│   ├── IDRIS_Website_Deployment_Guide.md
│   └── README_DEPLOYMENT.md
└── Presentation/
    └── IDRIS_Business_Plan_Presentation.pptx
```

---

## 🔒 Step 7: Add Collaborators (Optional)

If working with co-founders:

1. In your repository, click "Settings" tab
2. Click "Collaborators" in left sidebar
3. Click "Add people"
4. Enter Sanae's GitHub username or email
5. Select permission level:
   - **Write** (recommended) - Can push changes
   - **Admin** - Full control

---

## 📝 Step 8: Add Important Files

### Create .gitignore (Optional)

To exclude sensitive files from being committed:

```bash
# Create .gitignore file
cat > .gitignore << 'EOF'
# Operating System Files
.DS_Store
Thumbs.db

# Editor Files
.vscode/
.idea/
*.swp
*.swo

# Temporary Files
*.tmp
*.bak
~$*

# Private/Sensitive Files (DO NOT COMMIT)
*_PRIVATE.md
secrets/
.env
*.key

# Build/Output Folders
dist/
build/
*.log
EOF

# Add and commit
git add .gitignore
git commit -m "Add .gitignore to protect sensitive files"
git push
```

### Create LICENSE (Optional)

If making repository public:

```bash
# Create LICENSE file (MIT License for code, all rights reserved for docs)
cat > LICENSE << 'EOF'
MIT License

Copyright (c) 2026 IDRIS - Institute for Data-Driven Research & Innovation

Permission is hereby granted, free of charge, to any person obtaining a copy
of the website and code files (the "Software"), to deal in the Software 
without restriction, including without limitation the rights to use, copy, 
modify, merge, publish, distribute, sublicense, and/or sell copies of the 
Software, and to permit persons to whom the Software is furnished to do so, 
subject to the following conditions:

The above copyright notice and this permission notice shall be included in 
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

---

Business Plan & Strategy Documents © 2026 IDRIS. All rights reserved.
EOF

git add LICENSE
git commit -m "Add license"
git push
```

---

## 🎨 Step 9: Customize Repository Settings

### Repository Description

1. Go to repository main page
2. Click ⚙️ gear icon next to "About"
3. Add description:
   ```
   Complete business launch package for IDRIS - Research computing consultancy 
   serving academic institutions through reproducible software engineering, 
   scalable data pipelines, and advanced computing infrastructure.
   ```
4. Add topics (tags):
   - `research-computing`
   - `scientific-software`
   - `business-plan`
   - `hpc`
   - `bioinformatics`
   - `consulting`
   - `startup`
5. Save changes

### Social Preview Image (Optional)

Create a 1280×640px image with:
- IDRIS logo/name
- Tagline: "From Data to Discovery — At Scale"
- Upload in Settings → General → Social preview

---

## 📊 Step 10: Enable GitHub Features

### GitHub Pages (for website hosting)

1. Go to Settings → Pages
2. Under "Source", select:
   - Branch: `main`
   - Folder: `/Website`
3. Click "Save"
4. Your website will be at: `https://YOUR-USERNAME.github.io/idris-business-package/`

**Alternative:** Use Vercel (recommended) instead - see Website/README_DEPLOYMENT.md

### Projects (for task management)

1. Click "Projects" tab
2. Click "New project"
3. Select "Board" template
4. Name: "IDRIS Launch"
5. Add columns:
   - To Do
   - In Progress
   - Done
6. Add tasks from Next Steps in README.md

### Wiki (Optional - for additional documentation)

1. Click "Wiki" tab
2. Enable wiki
3. Can add:
   - Meeting notes
   - Decision logs
   - Technical documentation

---

## 🔐 Step 11: Security Best Practices

### Important: Never Commit Sensitive Data

**DO NOT commit:**
- ❌ Passwords or API keys
- ❌ Personal financial information
- ❌ Tax documents
- ❌ Social security numbers
- ❌ Private client data
- ❌ Signed contracts with confidential terms

**Safe to commit (already in package):**
- ✅ Business plan (generic, no sensitive data)
- ✅ Financial projections (models, not actual accounts)
- ✅ Website code (public anyway)
- ✅ Presentation (for pitching)
- ✅ Cost breakdowns (vendor pricing, not your actual expenses)

### If You Accidentally Commit Sensitive Data

```bash
# DO NOT just delete the file and commit
# The data is still in git history!

# Instead, use git filter-branch or BFG Repo-Cleaner
# Or delete the entire repository and start fresh

# Prevention is better - use .gitignore!
```

---

## 🎯 Step 12: Final Checklist

Before making repository public or sharing:

- [ ] All files uploaded correctly
- [ ] Folder structure matches REPOSITORY_STRUCTURE.md
- [ ] README.md displays properly on main page
- [ ] No sensitive data committed (double-check!)
- [ ] .gitignore created (if using)
- [ ] LICENSE added (if making public)
- [ ] Repository description and topics added
- [ ] Collaborators added (co-founder)
- [ ] Test: Clone repository to new location to verify everything works

---

## 🚀 Step 13: Using the Repository

### For Daily Work

```bash
# Pull latest changes (if working with co-founder)
git pull

# Make changes to files
# (edit documents, update website, etc.)

# See what changed
git status
git diff

# Stage changes
git add .

# Commit with descriptive message
git commit -m "Update financial projections with Q1 actuals"

# Push to GitHub
git push
```

### For Website Deployment

```bash
# Website files are in Website/ folder
cd Website/

# Option 1: Deploy to Vercel (recommended)
# See README_DEPLOYMENT.md for instructions

# Option 2: GitHub Pages
# Already configured if you enabled in Step 10
# Just push changes and site updates automatically
```

### For Presentations

```bash
# Presentation is in Presentation/ folder
# Download, edit in PowerPoint, upload updated version

# Command line:
git add Presentation/IDRIS_Business_Plan_Presentation.pptx
git commit -m "Update presentation with Q1 results"
git push
```

---

## 🔄 Keeping Repository Updated

### Regular Maintenance

**Weekly:**
- [ ] Review open issues/tasks
- [ ] Update financial projections if needed
- [ ] Sync any offline document changes

**Monthly:**
- [ ] Update business plan with actuals
- [ ] Refresh market data
- [ ] Archive old versions (git tags)

**Quarterly:**
- [ ] Major review of all documents
- [ ] Update presentation for new data
- [ ] Refresh website content

### Version Tagging

Mark important milestones:

```bash
# After incorporating Q1 results
git tag -a v1.1 -m "Post-Q1 2026 Update"
git push origin v1.1

# After first year
git tag -a v2.0 -m "Year 1 Complete - Actual Results"
git push origin v2.0
```

---

## 📞 Getting Help

### Git/GitHub Issues

**Resources:**
- GitHub Docs: https://docs.github.com
- Git Tutorial: https://git-scm.com/book/en/v2
- GitHub Learning Lab: https://lab.github.com

**Common Commands:**
```bash
# Help with any git command
git help <command>
git help commit

# Check repository status
git status

# View commit history
git log --oneline

# Undo last commit (keep changes)
git reset --soft HEAD~1

# Discard local changes
git checkout -- <file>
```

### Repository Organization Questions

- Check REPOSITORY_STRUCTURE.md for folder explanations
- See README.md for usage guidelines
- Review .gitignore to understand excluded files

---

## ✅ Success Criteria

Your repository is properly set up when:

1. ✅ All 9+ files organized in correct folders
2. ✅ README.md displays as main page with badges
3. ✅ No sensitive data committed
4. ✅ Co-founder has access (if applicable)
5. ✅ Can clone and all files are present
6. ✅ Website deployable from Website/ folder
7. ✅ Presentation downloads properly
8. ✅ All markdown files render correctly

---

## 🎊 You're Done!

**Your IDRIS business package is now professionally organized on GitHub.**

**Next steps:**
1. Share repository link with co-founder
2. Deploy website using Website/README_DEPLOYMENT.md
3. Start executing on business plan
4. Update repository as you progress

**Repository URL format:**
```
https://github.com/YOUR-USERNAME/idris-business-package
```

Share this URL with:
- Co-founder (required)
- Advisors/mentors (optional)
- Potential investors (if public)

---

**Questions?** All documentation is in the repository. Start with README.md!

**Ready to launch?** Follow the roadmap in Executive_Summary/IDRIS_Executive_Summary.md!
