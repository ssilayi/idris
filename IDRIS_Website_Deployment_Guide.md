# IDRIS Website Deployment Guide
## Deploy Your Website at $0 Cost in Under 15 Minutes

**Created:** January 2026  
**For:** IDRIS Website (idris-website.html)

---

## Quick Summary

You have **4 excellent free options** to deploy your IDRIS website:

| Platform | Best For | Setup Time | Custom Domain Cost |
|----------|----------|------------|-------------------|
| **Vercel** ⭐ | Easiest, fastest | 5 minutes | Free HTTPS |
| **Netlify** | Feature-rich | 5 minutes | Free HTTPS |
| **GitHub Pages** | Developer-friendly | 10 minutes | Free HTTPS |
| **Cloudflare Pages** | Performance-focused | 10 minutes | Free HTTPS |

**RECOMMENDED: Vercel** (easiest setup, excellent performance, perfect for your HTML site)

---

## Option 1: Vercel (RECOMMENDED) ⭐

### Why Vercel?
✅ Fastest deployment (literally 5 minutes)  
✅ Automatic HTTPS  
✅ Global CDN included  
✅ No credit card required  
✅ Perfect for static HTML sites  
✅ Free custom domain support  

### Step-by-Step Deployment

#### **Step 1: Prepare Your Website File**

1. Download `idris-website.html` from the outputs
2. Rename it to `index.html` (important!)
   ```bash
   # On your computer
   mv idris-website.html index.html
   ```
3. Create a new folder called `idris-website`
4. Put `index.html` inside this folder

**Your folder structure:**
```
idris-website/
└── index.html
```

#### **Step 2: Create Vercel Account**

1. Go to **https://vercel.com**
2. Click **"Sign Up"** (top right)
3. Choose one of these options:
   - **GitHub** (recommended if you use GitHub)
   - **GitLab**
   - **Bitbucket**
   - **Email** (works fine too)
4. Complete the sign-up process (no credit card needed!)

#### **Step 3: Deploy via Drag & Drop** (Easiest Method)

1. After signing in, you'll see the Vercel dashboard
2. Click **"Add New..."** button (top right)
3. Select **"Project"**
4. You'll see deployment options
5. **Scroll down** to find **"Deploy without Git"** section
6. You'll see a **drag-and-drop zone** that says:
   ```
   "Drop your project folder here to deploy"
   ```
7. **Drag your `idris-website` folder** into this zone
8. Vercel will automatically:
   - Upload your files
   - Detect it's a static site
   - Deploy it to a URL
9. **Wait 30-60 seconds** ⏱️
10. **Done!** You'll get a URL like: `https://idris-website-abc123.vercel.app`

#### **Step 4: Test Your Live Website**

1. Click the URL Vercel provides
2. Your IDRIS website should load immediately
3. Test all sections:
   - Navigation links work
   - Scrolling is smooth
   - Responsive on mobile (resize browser)
4. Share the link with others to test

#### **Step 5: Add Custom Domain (Optional but Recommended)**

**Option A: Use Free Vercel Subdomain**
- Your site is live at `your-project-name.vercel.app`
- Already has HTTPS
- No additional steps needed
- **Good for testing**, but not professional

**Option B: Add Your Own Domain ($10-15/year)**

1. **Buy a domain** (one-time annual cost):
   - **Namecheap**: $8-12/year for .com
   - **Google Domains**: $12/year
   - **Cloudflare**: $10/year
   - **Porkbun**: $8-10/year
   
   Recommended domains:
   - `idrisresearch.com`
   - `idris.io` (~$40/year but tech-friendly)
   - `idris-consulting.com`
   - `getidris.com`

2. **Connect domain to Vercel**:
   - In Vercel dashboard, go to your project
   - Click **"Settings"** tab
   - Click **"Domains"** in sidebar
   - Click **"Add Domain"**
   - Enter your domain (e.g., `idrisresearch.com`)
   - Vercel will show DNS records to add
   - Go to your domain registrar (Namecheap, etc.)
   - Add the DNS records Vercel shows you
   - Wait 5-30 minutes for DNS to propagate
   - **Done!** Your site is now at `idrisresearch.com` with free HTTPS

#### **Step 6: Update Your Website (Anytime)**

**Method 1: Drag & Drop (Easiest)**
1. Edit `index.html` on your computer
2. Go to Vercel dashboard
3. Click your project
4. Click **"Deployments"** tab
5. Drag updated `index.html` into the upload zone
6. New version goes live in ~30 seconds

**Method 2: Connect to GitHub (Better for Long-term)**
1. Create GitHub account (if you don't have one)
2. Create new repository called `idris-website`
3. Upload `index.html` to this repo
4. In Vercel, click **"Import Project"**
5. Connect your GitHub account
6. Select the `idris-website` repository
7. Click **"Deploy"**
8. Now every time you push to GitHub, Vercel auto-deploys!

---

## Option 2: Netlify

### Why Netlify?
✅ Similar to Vercel (equally good)  
✅ More form handling features  
✅ Great analytics on free tier  
✅ No credit card required  

### Step-by-Step Deployment

#### **Step 1: Prepare Files**
Same as Vercel - rename to `index.html` and put in a folder.

#### **Step 2: Create Netlify Account**

1. Go to **https://www.netlify.com**
2. Click **"Sign up"**
3. Choose:
   - **GitHub** (recommended)
   - **GitLab**
   - **Bitbucket**
   - **Email**
4. Complete sign-up (no credit card needed)

#### **Step 3: Deploy via Drag & Drop**

1. After logging in, you'll see the Netlify dashboard
2. Look for the **drag-and-drop zone** that says:
   ```
   "Want to deploy a new site without connecting to Git? 
   Drag and drop your site folder here"
   ```
3. **Drag your `idris-website` folder** into this area
4. Netlify uploads and deploys (30-60 seconds)
5. **Done!** You get a URL like: `https://random-name-123.netlify.app`

#### **Step 4: Customize Your Site Name**

1. Click **"Site settings"**
2. Under **"Site information"**, click **"Change site name"**
3. Enter: `idris-research` or `idris-website`
4. Your URL becomes: `https://idris-research.netlify.app`

#### **Step 5: Add Custom Domain**

1. Buy domain (same as Vercel instructions above)
2. In Netlify, go to **"Domain settings"**
3. Click **"Add custom domain"**
4. Enter your domain
5. Follow DNS instructions
6. Free HTTPS automatically enabled

#### **Step 6: Update Website**

1. Edit `index.html`
2. Go to **"Deploys"** tab in Netlify
3. Drag updated folder to upload zone
4. New version live in ~30 seconds

---

## Option 3: GitHub Pages

### Why GitHub Pages?
✅ Completely free forever  
✅ Developer-friendly  
✅ Integrated with Git version control  
✅ Custom domain support  

### Step-by-Step Deployment

#### **Step 1: Create GitHub Account**

1. Go to **https://github.com**
2. Click **"Sign up"**
3. Create account (free)
4. Verify your email

#### **Step 2: Create Repository**

1. Click **"+"** icon (top right)
2. Select **"New repository"**
3. Repository name: `idris-website`
4. Description: "IDRIS - Institute for Data-Driven Research & Innovation"
5. Select **"Public"** (required for free GitHub Pages)
6. Check **"Add a README file"**
7. Click **"Create repository"**

#### **Step 3: Upload Your Website**

1. In your new repository, click **"Add file"** → **"Upload files"**
2. Drag `index.html` (renamed from idris-website.html)
3. Add commit message: "Initial website upload"
4. Click **"Commit changes"**

#### **Step 4: Enable GitHub Pages**

1. In your repository, click **"Settings"** tab
2. Scroll down to **"Pages"** in left sidebar
3. Under **"Source"**, select:
   - Branch: **main**
   - Folder: **/ (root)**
4. Click **"Save"**
5. Wait 1-2 minutes
6. GitHub will show your site URL:
   ```
   Your site is published at https://your-username.github.io/idris-website/
   ```

#### **Step 5: Add Custom Domain (Optional)**

1. Buy domain (see Vercel instructions)
2. In GitHub Pages settings, enter your domain in **"Custom domain"** field
3. Click **"Save"**
4. In your domain registrar, add these DNS records:
   ```
   Type: A
   Name: @
   Value: 185.199.108.153
   
   Type: A
   Name: @
   Value: 185.199.109.153
   
   Type: A
   Name: @
   Value: 185.199.110.153
   
   Type: A
   Name: @
   Value: 185.199.111.153
   ```
5. Wait for DNS propagation (5-30 minutes)
6. Check **"Enforce HTTPS"** in GitHub Pages settings

#### **Step 6: Update Website**

1. Edit `index.html` on your computer
2. In GitHub repo, click **"Add file"** → **"Upload files"**
3. Drag updated `index.html`
4. Commit message: "Update website content"
5. Click **"Commit changes"**
6. Changes go live in 1-2 minutes

---

## Option 4: Cloudflare Pages

### Why Cloudflare Pages?
✅ Best global performance  
✅ Unlimited bandwidth  
✅ Excellent security  
✅ Free forever  

### Step-by-Step Deployment

#### **Step 1: Create Cloudflare Account**

1. Go to **https://pages.cloudflare.com**
2. Click **"Sign up"**
3. Enter email and create password
4. Verify email
5. No credit card required

#### **Step 2: Create New Project**

1. Click **"Create a project"**
2. Choose **"Connect to Git"** OR **"Direct Upload"**

**Option A: Direct Upload (Simpler)**
3. Select **"Direct Upload"**
4. Name your project: `idris-website`
5. Drag your folder with `index.html`
6. Click **"Deploy site"**
7. Wait 30-60 seconds
8. Done! URL: `https://idris-website.pages.dev`

**Option B: Git Integration**
3. Connect GitHub account
4. Select repository
5. Click **"Begin setup"**
6. Leave build settings empty (static site)
7. Click **"Save and Deploy"**

#### **Step 3: Add Custom Domain**

1. In project settings, click **"Custom domains"**
2. Click **"Set up a custom domain"**
3. Enter your domain
4. Follow DNS instructions
5. Cloudflare automatically manages HTTPS

---

## Cost Comparison

### Free Forever (100% Free)

| Item | Vercel | Netlify | GitHub Pages | Cloudflare |
|------|--------|---------|--------------|------------|
| Hosting | ✅ Free | ✅ Free | ✅ Free | ✅ Free |
| HTTPS | ✅ Free | ✅ Free | ✅ Free | ✅ Free |
| CDN | ✅ Free | ✅ Free | ✅ Free | ✅ Free |
| Bandwidth | 100GB/mo | 100GB/mo | 100GB/mo | Unlimited |
| Builds | Unlimited | 300/mo | Unlimited | 500/mo |

### Optional Costs (If You Want a Custom Domain)

**Domain Registration (Annual):**
- `.com` domain: $8-12/year (Namecheap, Porkbun)
- `.io` domain: $30-40/year (Namecheap)
- `.consulting`: $25-30/year
- `.co` domain: $20-25/year

**Everything else stays FREE** - all platforms include free HTTPS with custom domains!

---

## Recommended Approach for IDRIS

### Phase 1: Launch (Week 1) - $0

**Use Vercel with free subdomain:**
1. Deploy to `idris-research.vercel.app` (FREE)
2. Test with colleagues and potential clients
3. Gather feedback
4. Make adjustments
5. **Total cost: $0**

**Advantage:** Live website immediately, professional appearance, no financial commitment

### Phase 2: Professional Domain (Month 1-2) - $10-15

**Buy custom domain:**
1. After validating interest, buy `idrisresearch.com` ($10-12/year)
2. Connect to Vercel (takes 10 minutes)
3. Now your site is at `idrisresearch.com`
4. Professional email: `contact@idrisresearch.com` via Google Workspace ($6/user/month)

**Total Year 1 cost: $12 + $72 = $84/year**

### Phase 3: Long-term (Month 3+) - $0 hosting

**Maintain free hosting:**
- Vercel hosting: FREE forever
- HTTPS: FREE forever
- CDN: FREE forever
- Updates: FREE unlimited

**Only recurring cost: Domain ($12/year) + Email ($72/year) = $84/year**

---

## Troubleshooting Common Issues

### Issue 1: "Site not loading"
**Solution:**
- Clear browser cache (Ctrl+Shift+Delete)
- Try incognito/private browsing
- Wait 2-5 minutes after deployment
- Check if URL is exactly correct

### Issue 2: "CSS/styling not working"
**Solution:**
- Ensure file is named `index.html` (not idris-website.html)
- Check that HTML file is in root folder
- Verify file uploaded completely

### Issue 3: "Custom domain not working"
**Solution:**
- DNS propagation takes 5-30 minutes (sometimes up to 24 hours)
- Verify DNS records exactly match platform instructions
- Use https://dnschecker.org to check propagation
- Try clearing DNS cache: `ipconfig /flushdns` (Windows) or `sudo dscacheutil -flushcache` (Mac)

### Issue 4: "HTTPS not working"
**Solution:**
- All platforms auto-enable HTTPS, but it can take 5-10 minutes
- With custom domain, wait 30 minutes after DNS propagates
- Check "Enforce HTTPS" setting in platform

### Issue 5: "Can't update website"
**Solution:**
- **Vercel/Netlify:** Drag new file to deployment area (overwrites old version)
- **GitHub:** Upload new file, commit changes
- **Cloudflare:** Use "Create new deployment" in dashboard
- Clear browser cache after updating

---

## Step-by-Step Quick Start (Absolute Fastest)

### Total Time: 5 Minutes

1. **Download** `idris-website.html` from outputs
2. **Rename** to `index.html`
3. **Go to** https://vercel.com
4. **Sign up** with GitHub or email (1 min)
5. **Drag** your `index.html` file to Vercel (1 min)
6. **Wait** 30 seconds for deployment
7. **Click** the URL Vercel gives you
8. **Done!** Your website is live at `https://your-project.vercel.app`

**Live website in under 5 minutes, $0 cost, HTTPS included!**

---

## Advanced: Email Setup (Optional)

Once you have a custom domain, you can add professional email:

### Option 1: Google Workspace ($6/user/month)
- Professional: `contact@idrisresearch.com`
- Gmail interface
- 30GB storage
- Google Meet, Calendar, Drive included

### Option 2: Zoho Mail ($1/user/month or FREE for 1 user)
- Budget-friendly
- 5GB storage (free tier)
- Basic features
- Good for startups

### Option 3: Cloudflare Email Routing (FREE)
- Email forwarding only
- Forward `contact@idrisresearch.com` to personal Gmail
- No inbox, just forwarding
- Perfect for bootstrap stage

---

## What to Do Right Now

### Immediate Action Plan:

**Next 30 Minutes:**
1. ☐ Go to Vercel.com
2. ☐ Create free account
3. ☐ Download idris-website.html and rename to index.html
4. ☐ Drag file to Vercel
5. ☐ Get your live URL
6. ☐ Test website on phone and desktop
7. ☐ Share URL with Swabir and Sanae

**This Week:**
8. ☐ Get feedback from co-founder
9. ☐ Make any needed adjustments
10. ☐ Decide on domain name
11. ☐ Test site with 3-5 colleagues

**Next Week (If Happy with Site):**
12. ☐ Buy custom domain ($10-12)
13. ☐ Connect domain to Vercel
14. ☐ Set up professional email
15. ☐ Announce to network

**Month 2:**
16. ☐ Site is live and professional
17. ☐ Business is operational
18. ☐ Total spent: ~$84/year

---

## Summary: Why This Works

✅ **$0 to start** - no financial risk  
✅ **5 minutes to deploy** - can be live today  
✅ **Professional appearance** - looks like $5,000 website  
✅ **Global CDN** - fast loading worldwide  
✅ **Automatic HTTPS** - secure and trusted  
✅ **Easy updates** - drag & drop new versions  
✅ **Scalable** - handles 100,000+ visitors/month free  
✅ **No maintenance** - platform handles everything  

**You literally cannot find a better deal than FREE with this level of quality.**

---

## Quick Reference Card

**Fastest Deployment:**
```
1. Vercel.com
2. Sign up (GitHub or email)
3. Drag index.html file
4. Live in 60 seconds at https://your-project.vercel.app
```

**Add Domain Later:**
```
1. Buy domain: Namecheap.com ($10-12/year)
2. In Vercel: Settings → Domains → Add
3. Add DNS records from Vercel to Namecheap
4. Wait 10-30 minutes
5. Done! https://idrisresearch.com with free HTTPS
```

**Update Website:**
```
1. Edit index.html
2. Drag to Vercel deployment area
3. Live in 30 seconds
```

---

**BOTTOM LINE:** 

Deploy to Vercel right now (5 minutes, $0), test for a week, then add a custom domain ($12) when ready. You'll have a professional research consultancy website for $12/year in hosting costs.

**This is the same infrastructure that billion-dollar companies use, and you get it free.**

---

**Document Version:** 1.0  
**Last Updated:** January 2026  
**Next Update:** After first deployment feedback

**Questions?** All platforms have excellent documentation and support forums. Vercel has live chat support even on free tier!
