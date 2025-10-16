# 📊 Activity Tracker

A simple, offline-first web application for tracking daily activities, visualizing time usage, and analyzing productivity patterns.

**Created with Claude** (Anthropic's AI assistant)

---

## 🌟 Features

### ⏱️ Activity Logging
- **Time-based entries** with start and end times
- **Automatic duration calculation** - just enter when you started and finished
- **Subject categorization** - create and reuse activity categories
- **Star ratings** (1-5 stars) to rate your activities
- **Notes field** for additional details
- **Persistent storage** - all data saved locally in your browser

### 📈 Visualizations

**Summary View (Bar Chart)**
- Visual breakdown of time spent by subject
- Percentage and minute totals for each activity
- Daily total time calculation

**Timeline View**
- 24-hour timeline showing when activities occurred
- Color-coded blocks for each subject
- Proportional sizing based on duration
- Visual representation of your entire day

### 🔍 Query & Filter

Filter your activities by:
- **Subject** - search by activity name
- **Date range** - start and end dates
- **Minimum rating** - show only highly-rated activities

### 💾 Data Management

**Export Options:**
- **CSV format** - compatible with Excel, Google Sheets, Numbers
- **JSON format** - complete data backup with all fields

**Import Options:**
- **CSV import** - bring data from spreadsheets
- **JSON import** - restore from backups

---

## 🚀 Getting Started

### Installation

1. **Access the app** at your GitHub Pages URL:
   ```
   https://YOUR-USERNAME.github.io/activity-tracker/
   ```

2. **Add to iPhone Home Screen** (recommended):
   - Open the app in Safari
   - Tap the Share button (square with arrow)
   - Scroll and tap "Add to Home Screen"
   - Name it "Activity Tracker"
   - Tap "Add"

3. **Works offline!** After the first load, the app works without internet

### First-Time Setup

1. **Add your first activity:**
   - Select today's date (pre-filled)
   - Enter when you started the activity
   - Enter when you finished (defaults to current time)
   - Create a new subject or select existing
   - Add notes (optional)
   - Rate the activity (optional)
   - Tap "Add Entry"

2. **View your data:**
   - Check the Summary view for totals
   - Switch to Timeline to see when activities occurred
   - Use filters in the Query section

---

## 📖 How to Use

### Adding an Entry

1. **Date** - Defaults to today, can be changed for past entries
2. **Start Time** - When you began the activity
3. **End Time** - When you finished (pre-filled with current time)
4. **Duration** - Calculated automatically, displayed below end time
5. **Subject** - Select from dropdown or create new
6. **Notes** - Optional details about the activity
7. **Rating** - Click stars to rate 1-5 (optional)
8. **Add Entry** - Saves to local storage

### Duration Calculation

The app automatically calculates duration from start and end times:
- Start: `09:00`, End: `11:30` → Duration: `2h 30m (150 minutes)`
- Handles overnight activities (end time before start time assumes next day)

### Creating Subjects

First time:
1. Select "**+ Add New Subject**" from dropdown
2. Enter subject name (e.g., "Work", "Exercise", "Reading")
3. Complete the entry

Future entries:
- Subject appears in dropdown for quick selection
- Consistent naming helps with visualization

### Viewing Data

**Summary View:**
- Select a date
- View bar chart showing time breakdown by subject
- See percentages and total minutes

**Timeline View:**
- Select a date  
- View 24-hour timeline with activity blocks
- Each subject has a unique color
- Activities span multiple hours automatically

### Filtering Entries

Use the Query Entries section to filter:

1. **Subject Filter** - Type to search (case-insensitive)
2. **Date Range** - Set start and/or end date
3. **Minimum Rating** - Show only activities rated X stars or higher

All filters work together (AND logic).

### Exporting Data

**CSV Export:**
- Click "📥 Export CSV"
- Opens in Excel, Sheets, Numbers
- Format: Date, Start Time, End Time, Duration, Subject, Rating, Notes

**JSON Export:**
- Click "📥 Export JSON"  
- Complete backup with all metadata
- Best for app-to-app data transfer

### Importing Data

**CSV Import:**
- Click "📤 Import CSV"
- Select your CSV file
- Adds entries to existing data (doesn't replace)

**JSON Import:**
- Click "📤 Import JSON"
- Select your JSON file
- **Replaces all existing data** with imported data

---

## 💡 Tips & Best Practices

### Data Entry
- ✅ **Log activities immediately** - end time defaults to now
- ✅ **Use consistent subject names** - "Exercise" vs "exercise" are different
- ✅ **Add notes for context** - helps remember details later
- ✅ **Rate meaningful activities** - use filters to find high-rated tasks

### Visualization
- 📊 **Check Summary view** for proportions (what took most time?)
- ⏰ **Check Timeline view** for patterns (when are you most productive?)
- 📅 **Review different dates** to identify trends

### Data Management
- 💾 **Export weekly** - create regular CSV backups
- 📁 **Save to Files app** - keep backups in iCloud Drive
- 🔄 **Test imports** - verify backups work before you need them

### Organization
- 🏷️ **Use clear subject names** - "Work: Project A" vs "Work: Emails"
- ⭐ **Rating system** - define what each star level means to you
- 📝 **Notes for exceptions** - explain unusual activities or circumstances

---

## 🔒 Privacy & Data Storage

### Where Is My Data?

Your activity data is stored in **browser localStorage**:
- ✅ **Stored locally** on your device only
- ✅ **Never sent to a server** - completely private
- ✅ **Persists between sessions** - data survives closing the browser
- ⚠️ **Device-specific** - doesn't sync across devices
- ⚠️ **Browser-specific** - Safari data doesn't transfer to Chrome

### Data Security

- **No account required** - no passwords to manage
- **No tracking** - no analytics or telemetry
- **Offline-capable** - works without internet after first load
- **Export control** - you decide when and where to save backups

### Clearing Data

Your data will be lost if you:
- Clear Safari's website data
- Delete the browser app
- Clear "All History and Website Data"

**Protection:** Export regular CSV/JSON backups!

---

## 🛠️ Technical Details

### Built With
- **Pure HTML/CSS/JavaScript** - no frameworks or dependencies
- **LocalStorage API** - for persistent data storage
- **File API** - for CSV/JSON import/export
- **Responsive Design** - works on desktop and mobile

### Browser Compatibility
- ✅ Safari (iOS/macOS)
- ✅ Chrome (Desktop/Mobile)
- ✅ Firefox (Desktop/Mobile)
- ✅ Edge (Desktop/Mobile)

Requires modern browser with ES6+ support.

### Hosting
- **GitHub Pages** - free static site hosting
- **No backend required** - purely client-side application
- **Instant updates** - changes to HTML file update site in ~2 minutes

---

## 📱 Mobile Optimization

The app is optimized for iPhone/mobile use:
- ✅ Touch-friendly buttons and inputs
- ✅ Large text and tap targets
- ✅ Responsive layout adapts to screen size
- ✅ iOS-specific meta tags for home screen app
- ✅ Works in Safari and as home screen icon

---

## 🐛 Troubleshooting

### Data Not Saving
**Problem:** Entries disappear after refresh  
**Solution:**
- Check Safari settings → Don't block cookies
- Don't use Private Browsing mode
- Export data as backup

### Can't Import CSV
**Problem:** Import fails or shows errors  
**Solution:**
- Ensure CSV has correct headers: `Date, Start Time, End Time, Duration (min), Subject, Rating, Notes`
- Check for special characters in notes field
- Try exporting first, then re-importing to verify format

### Timeline Not Showing Activities
**Problem:** Timeline view is empty but Summary shows data  
**Solution:**
- Verify activities have both start and end times
- Check that you've selected the correct date
- Old entries (before start/end time feature) may not display

### Duration Shows Wrong Time
**Problem:** Calculated duration is incorrect  
**Solution:**
- For overnight activities, duration wraps to next day
- Ensure start time is before end time (same day)
- Check 12-hour vs 24-hour time format

### App Won't Load
**Problem:** Blank page or loading error  
**Solution:**
- Check internet connection (first load only)
- Clear browser cache and reload
- Ensure you're using a modern browser
- Check GitHub Pages is enabled in repository settings

---

## 🔄 Updating the App

### To Update Your Deployment:

1. Go to your GitHub repository
2. Click on `index.html`
3. Click the pencil icon (Edit)
4. Make your changes
5. Scroll down and click "Commit changes"
6. Wait 1-2 minutes for GitHub Pages to update
7. Hard refresh your browser (Cmd+Shift+R or Ctrl+Shift+R)

### To Update the Home Screen App:

After updating the file on GitHub:
1. Remove the current app from home screen
2. Open Safari and navigate to your GitHub Pages URL
3. Tap Share → "Add to Home Screen" again

---

## 📊 Data Format

### CSV Format
```csv
Date,Start Time,End Time,Duration (min),Subject,Rating,Notes
2025-01-15,09:00,11:30,150,Work,4,"Completed project proposal"
2025-01-15,12:00,13:00,60,Lunch,5,"Great meal!"
```

### JSON Format
```json
[
  {
    "id": 1705315200000,
    "date": "2025-01-15",
    "time": "09:00",
    "endTime": "11:30",
    "duration": 150,
    "subject": "Work",
    "rating": 4,
    "notes": "Completed project proposal"
  }
]
```

---

## 🤝 Contributing

This is a personal project, but you're welcome to:
- Fork the repository
- Customize for your needs
- Share improvements (though no formal PR process)

---

## 📄 License

This project is open source and available for personal use. Feel free to modify and customize as needed.

---

## 🙏 Credits

**Created with Claude** - Anthropic's AI assistant  
Built through iterative conversation and requirements refinement.
