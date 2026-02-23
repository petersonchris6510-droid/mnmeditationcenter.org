# MMC WEBSITE UPDATE - READY TO DEPLOY

## Changes Made (Per Monk Choo's Feedback)

### ✅ Team Page Updates
- **Years of practice:** Updated from 15 to 17 years
- **Ecuador added:** Now shows both Mexico and Ecuador flags
- **Ecuador emphasis:** Text updated to mention he runs a club in Ecuador

### ✅ Schedule Page Updates  
**Saturday class made more inviting:**
- **Before:** "90-minute meditation session. A longer session for those who want more time in practice."
- **After:** "90-minute session with guided meditation, gentle introduction, and wisdom talk. Perfect for those wanting a deeper practice. Beginners welcome."

### ✅ Phone Number Updates (Site-Wide)
- **Primary phone:** (561) 229-9694 (Monk Choo's direct line)
- **WhatsApp added:** 💬 icon next to every phone number links to WhatsApp
- **Updated in:** Schema markup, footer, contact sections, all 17 pages

### ✅ Code Refactor (Professional Structure)
- **Shared CSS:** All styles in /css/shared.css
- **Shared JS:** All navigation in /js/shared.js  
- **Mobile optimized:** Better touch targets, responsive menu, readable text
- **File size:** 54% smaller HTML files

---

## How to Deploy

### Option 1: Replace Entire Site (Recommended)
```bash
# 1. Navigate to your local GitHub repo
cd ~/path/to/mnmeditationcenter.org

# 2. Backup current version (just in case)
cp -r . ../mmc-backup-$(date +%Y%m%d)

# 3. Copy all updated files from outputs
cp -r /path/to/outputs/mmc-site-refactored/* .

# 4. Push to GitHub
git add .
git commit -m "Update: Monk Choo edits + professional refactor + WhatsApp integration"
git push
```

### Option 2: Download and Deploy
1. Download the entire `mmc-site-refactored` folder
2. Replace your GitHub repo contents with these files
3. Commit and push

---

## What Changed Where

### Files Modified
**Content changes:**
- team.html (17 years, Ecuador added)
- schedule.html (Saturday description more inviting)
- All 17 HTML pages (phone numbers + WhatsApp)

**Structure changes:**
- Created: css/shared.css (11KB - all styles)
- Created: js/shared.js (2.5KB - navigation)
- Updated: All HTML files now link to shared files

### What to Test After Deploy

1. **Visit mnmeditationcenter.org**
2. **Check phone number:** Should show (561) 229-9694 with WhatsApp icon
3. **Click WhatsApp icon:** Should open WhatsApp to that number
4. **Check team page:** Should say 17 years, show Ecuador flag
5. **Check schedule:** Saturday should mention "gentle introduction and wisdom talk"
6. **Test mobile:** Hamburger menu should work

---

## Files Ready in Outputs

The complete updated site is in:
`/mnt/user-data/outputs/mmc-site-refactored/`

This includes:
- All HTML pages with Monk Choo's edits
- New css/ and js/ folders
- Updated phone numbers everywhere
- WhatsApp integration
- Mobile improvements

---

## Quick Verification Checklist

Before deploying, you can:
- [ ] Open index.html locally, verify phone shows (561) 229-9694
- [ ] Check WhatsApp link works
- [ ] Open team.html, verify says 17 years and shows Ecuador
- [ ] Open schedule.html, verify Saturday sounds more inviting
- [ ] Test mobile view (browser F12 → device toggle)

After deploying:
- [ ] Visit live site
- [ ] Click WhatsApp icon
- [ ] Check on mobile phone
- [ ] Tell Monk Choo changes are live!

---

**Ready to push when you are!**
