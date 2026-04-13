## Balagot

#### Framework: Svelte + Vite

#### Module: Alumni Portal - Document Request & Digital Credentials

#### Installation

To replicate and run this project follow the following steps using Windows PowerShell:

```bash
# Install Node.js
winget install OpenJS.NodeJS.LTS

# Use nvm to manage Node versions (optional)
nvm install lts
nvm use lts

# Clone the repository
git clone <repo-link-here>
cd firstattempt2026_Balagot

# Install dependencies
npm install

# Run development server
npm run dev
```

The application will be available at **http://localhost:5173/**

### AI Tools:

1. ChatGPT
2. Claude (Premium)
3. GitHub Copilot (VS Code)

### Prompt:

Create a comprehensive alumni portal for Ateneo de Davao University featuring:
- Role-based authentication (Alumni & Office Staff)
- Digital academic credentials with QR code sharing
- Multi-step document request workflow
- Biometric login (FaceID/Fingerprint)
- Staff dashboard for document processing, inventory management, and payment verification
- Professional Blue Knight branding with royal blue color scheme
- Responsive mobile design
- Real-time status tracking for document requests

### Features Implemented:

✅ **Alumni Module**
- Role-based login with biometric support
- Digital Academic Passport
- Multi-step document request (TOR, Diploma, GMC, Certification, Letter)
- Rush processing option (48-hour delivery)
- QR code secure sharing
- PDF download with 30-day expiration

✅ **Staff Module**
- Verification Dashboard (alumni verification requests)
- Document Log with barcode/QR scanning
- Inventory Alerts (stock monitoring)
- Payment Verification (unique reference codes)

✅ **Design System**
- Professional sidebar navigation
- Responsive topbar with notifications
- 27 CSS variables for complete theming
- DM Serif Display & DM Sans fonts
- "Blue Knight" royal blue branding

### Screenshots

Create an `images/` folder in your root directory and place all screenshots there.

Use the following format to embed images:

```markdown
![Alt text](images/screenshot-name.png)
```

Example:
```markdown
#### Login Screen
![Login Dashboard](images/login-screen.png)

#### Alumni Dashboard
![Alumni Dashboard](images/dashboard-alumni.png)

#### Document Request Form
![Document Request](images/document-request.png)

#### Staff Dashboard
![Staff Dashboard](images/staff-dashboard.png)
```

### Project Structure

```
src/
├── App.svelte              # Main entry point
├── app.css                 # Global styles & design system
├── main.js                 # App initialization
└── lib/
    ├── LoginNew.svelte           # Authentication with role selection
    ├── DashboardNew.svelte       # Main dashboard with sidebar navigation
    ├── MyProfile.svelte          # Alumni profile & credentials
    ├── DocumentRequest.svelte    # Multi-step document request
    ├── StaffDashboard.svelte     # Staff admin panel
    └── Counter.svelte            # (Component template)
```

### Technology Stack

- **Frontend Framework:** Svelte 5.55.1
- **Build Tool:** Vite 8.0.8
- **Styling:** CSS3 with CSS Variables
- **Fonts:** Google Fonts (DM Serif Display, DM Sans)

### Color Palette

- **Royal Dark:** #0f2347
- **Royal:** #1a3a6b
- **Royal Mid:** #2e5fa3
- **Royal Light:** #e8eef8
- **Gold:** #c9a227
- **Success:** #1a7a4a
- **Warning:** #b45309
- **Danger:** #b91c1c

### Scripts

```bash
# Development
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

### Browser Support

Works on all modern browsers supporting ES6+:
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)

### Future Enhancements

- [ ] Backend integration (Node.js/Express)
- [ ] Database setup (MongoDB/PostgreSQL)
- [ ] Payment gateway integration (Stripe/GCash)
- [ ] Email notifications
- [ ] QR code generation library
- [ ] Barcode scanning library
- [ ] Two-factor authentication
- [ ] Document storage & archiving
