# GitHub Pages Deployment Guide

## Quick Start (5 Minutes)

Your timetable application is ready for deployment! Follow these simple steps:

### Step 1: Create GitHub Repository

1. Go to [GitHub.com](https://github.com) and sign in
2. Click the "+" icon in the top right corner
3. Select "New repository"
4. Name it: `timetable-app`
5. Make sure it's **Public** (required for free GitHub Pages)
6. Click "Create repository"

### Step 2: Upload Your Code

You have two options:

#### Option A: Using Git (Recommended)
```bash
# Navigate to your project folder
cd timetable-app

# Initialize git repository
git init

# Add all files
git add .

# Commit your changes
git commit -m "Initial commit - Level 3 Junior Timetable"

# Add your GitHub repository as remote
git remote add origin https://github.com/YOURUSERNAME/timetable-app.git

# Push to GitHub
git push -u origin main
```

#### Option B: Upload Files Directly
1. Download the `timetable-app` folder from this environment
2. Go to your GitHub repository page
3. Click "uploading an existing file"
4. Drag and drop all files from the `timetable-app` folder
5. Commit the changes

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click "Settings" tab
3. Scroll down to "Pages" in the left sidebar
4. Under "Source", select **"GitHub Actions"**
5. The deployment will start automatically

### Step 4: Access Your Website

- Your website will be live at: `https://YOURUSERNAME.github.io/timetable-app/`
- First deployment takes 2-5 minutes
- Future updates deploy automatically when you push changes

## Features of Your Deployed Website

✅ **Automatic Timetable Display**: Shows Level 3 Junior class schedule
✅ **Search & Filter**: Find classes by subject, time, or day
✅ **Dark/Light Mode**: Toggle between themes
✅ **Mobile Responsive**: Works on phones, tablets, and computers
✅ **Myanmar Language Support**: Proper display of Myanmar text
✅ **Real-time Features**: Live clock and current day highlighting
✅ **Statistics Dashboard**: Class analytics and insights

## Updating Your Timetable

### Method 1: Edit JSON File Directly
1. Go to your GitHub repository
2. Navigate to `src/assets/processed_timetable.json`
3. Click the pencil icon to edit
4. Update the schedule data
5. Commit changes - website updates automatically!

### Method 2: Upload New Excel File
1. Process your new Excel file using the same method we used
2. Replace the JSON data
3. Push changes to GitHub

## Customization Options

### Change Colors
Edit `src/App.jsx` and modify the `getSubjectColor` function:
```javascript
const getSubjectColor = (subject) => {
  if (subject.includes('Grammar')) return 'bg-blue-100 text-blue-800'
  // Add your custom colors here
}
```

### Add New Features
- The code is well-organized and documented
- Add new components in `src/components/`
- Modify styling using Tailwind CSS classes

### Change Title
Edit `index.html` to change the page title:
```html
<title>Your Custom Title</title>
```

## Troubleshooting

### Website Not Loading?
- Check if repository is public
- Verify GitHub Pages is enabled with "GitHub Actions" source
- Wait 5-10 minutes for first deployment

### Changes Not Showing?
- Check the "Actions" tab in your repository for deployment status
- Clear browser cache (Ctrl+F5 or Cmd+Shift+R)
- Verify your changes were committed to the main branch

### Need Help?
- Check the repository's "Actions" tab for error messages
- Ensure all files are properly uploaded
- Verify the `dist` folder was created during build

## Advanced Features

### Custom Domain (Optional)
1. Buy a domain name
2. Add a `CNAME` file to your repository with your domain
3. Configure DNS settings with your domain provider

### Analytics (Optional)
Add Google Analytics by editing `index.html`:
```html
<!-- Add Google Analytics code here -->
```

## File Structure
```
timetable-app/
├── src/
│   ├── assets/
│   │   └── processed_timetable.json  # Your schedule data
│   ├── components/
│   └── App.jsx                       # Main application
├── dist/                             # Built files (auto-generated)
├── .github/workflows/deploy.yml      # Auto-deployment config
└── README.md                         # Documentation
```

## Success! 🎉

Your automatic timetable website is now live and accessible to anyone with the URL. Students and teachers can:

- View the complete class schedule
- Search for specific subjects or times
- Use dark mode for better viewing
- Access it from any device with internet

The website will automatically update whenever you push changes to GitHub!

