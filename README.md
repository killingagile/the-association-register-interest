# Beta Signup Page

A simple, beautiful beta signup page that saves user details to Google Sheets.

## Features
- ✨ Clean, responsive design
- 📊 Saves data to Google Sheets
- 🚀 Hosted on GitHub Pages
- ✅ Email validation and duplicate checking
- 🎯 Error handling and user feedback

## Setup Instructions

### 1. Google Sheets Setup
1. Create a new [Google Sheet](https://sheets.google.com)
2. Add these headers in row 1: `Name`, `Email`, `Company`, `Notes`, `Timestamp`
3. Copy the Sheet ID from the URL (the long string between `/d/` and `/edit`)

### 2. Google Apps Script Setup
1. Go to [Google Apps Script](https://script.google.com)
2. Create a new project
3. Paste the code from `google-apps-script.js`
4. Replace `YOUR_SHEET_ID` with your actual Sheet ID
5. Deploy as web app:
   - Execute as: "Me"
   - Who has access: "Anyone"
   - Copy the web app URL

### 3. Update HTML
1. In `index.html`, replace `YOUR_GOOGLE_APPS_SCRIPT_WEB_APP_URL_HERE` with your actual web app URL
2. Customize the title, heading, and description as needed

### 4. Deploy to GitHub Pages
1. Push this repository to GitHub
2. Go to Settings → Pages
3. Select source: "Deploy from a branch"
4. Choose: "main branch"
5. Your site will be available at: `https://yourusername.github.io/repository-name`

## Testing
1. Test locally by opening `index.html` in a browser
2. Fill out the form and submit
3. Check your Google Sheet for the new row
4. Verify error handling by submitting duplicate emails

## Customization
- Edit the CSS in `<style>` section for different colors/styling
- Add more form fields by updating both HTML and Apps Script
- Modify validation rules in the Apps Script

## Troubleshooting
- Check browser console for JavaScript errors
- Verify Google Apps Script deployment has "Anyone" access
- Ensure Sheet ID is correct in Apps Script
- Test the Apps Script URL directly in browser (should return JSON)
