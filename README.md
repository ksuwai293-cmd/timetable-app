# Level 3 Junior - Class Timetable

A modern, responsive web application for displaying class schedules automatically generated from Excel data.

## Features

- 📅 **Interactive Timetable**: View class schedules organized by day
- 🔍 **Search Functionality**: Search for specific subjects, times, or days
- 🌓 **Dark Mode**: Toggle between light and dark themes
- 📊 **Statistics**: View class statistics and analytics
- 📱 **Responsive Design**: Works perfectly on desktop and mobile devices
- 🌐 **Myanmar Language Support**: Proper display of Myanmar Unicode text
- ⚡ **Real-time Updates**: Live clock and current day highlighting

## Technology Stack

- **Frontend**: React 18 with Vite
- **Styling**: Tailwind CSS with shadcn/ui components
- **Icons**: Lucide React
- **Deployment**: GitHub Pages with GitHub Actions

## Getting Started

### Prerequisites

- Node.js 18 or higher
- npm or yarn package manager

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/timetable-app.git
   cd timetable-app
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```

4. Open your browser and navigate to `http://localhost:5173`

### Building for Production

```bash
npm run build
```

The built files will be in the `dist` directory.

## Deployment to GitHub Pages

This project is configured for automatic deployment to GitHub Pages using GitHub Actions.

### Setup Instructions

1. **Create a GitHub Repository**:
   - Go to GitHub and create a new repository named `timetable-app`
   - Make sure it's public (required for free GitHub Pages)

2. **Push Your Code**:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/yourusername/timetable-app.git
   git push -u origin main
   ```

3. **Enable GitHub Pages**:
   - Go to your repository settings
   - Navigate to "Pages" in the left sidebar
   - Under "Source", select "GitHub Actions"
   - The workflow will automatically deploy your site

4. **Access Your Site**:
   - Your site will be available at: `https://yourusername.github.io/timetable-app/`
   - It may take a few minutes for the first deployment

### Manual Deployment (Alternative)

If you prefer manual deployment:

1. Build the project:
   ```bash
   npm run build
   ```

2. Deploy the `dist` folder to GitHub Pages using any deployment tool or service.

## Data Structure

The timetable data is stored in `src/assets/processed_timetable.json` with the following structure:

```json
[
  {
    "level": "Level 3 Junior",
    "day": "TUE",
    "time": "6:30 - 7:30 AM",
    "subject": "ဦးသောဘန"
  }
]
```

### Updating Timetable Data

To update the timetable:

1. Replace the data in `src/assets/processed_timetable.json`
2. Follow the same JSON structure
3. Rebuild and redeploy the application

## Customization

### Colors and Themes

Subject colors are automatically assigned based on subject type in `src/App.jsx`:

- **Grammar**: Blue theme
- **Vocab**: Green theme  
- **Headway**: Purple theme
- **Myanmar names**: Amber theme
- **Default**: Gray theme

### Adding New Features

The application is built with modern React patterns and is easily extensible:

- Add new components in `src/components/`
- Modify styling in `src/App.jsx` using Tailwind classes
- Update data processing logic as needed

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## License

This project is open source and available under the [MIT License](LICENSE).

## Support

For support or questions, please open an issue in the GitHub repository.

---

**Built with ❤️ for Level 3 Junior students**

