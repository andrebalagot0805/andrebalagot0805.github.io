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

#### 🎓 Alumni Module

##### Login Screen
![](https://github.com/andrebalagot0805/andrebalagot0805.github.io/blob/main/e7348d98-44f0-403a-8a6a-06556226b7c8.jpg)

![](https://github.com/andrebalagot0805/andrebalagot0805.github.io/blob/main/d4ed5ce0-7e62-4dcf-aabc-f5239a1d5787.jpg)

![](https://github.com/andrebalagot0805/andrebalagot0805.github.io/blob/main/c6cc646a-2953-4f91-9464-c656605e451c.jpg)

![](https://github.com/andrebalagot0805/andrebalagot0805.github.io/blob/main/be2f175a-0f23-4840-8c03-7a1db5365d7c.jpg)

![](https://github.com/andrebalagot0805/andrebalagot0805.github.io/blob/main/a55513e4-b902-4ada-af6e-5e55a76cb260.jpg)

![](https://github.com/andrebalagot0805/andrebalagot0805.github.io/blob/main/91dd7620-dd6d-43b1-a6ee-cba8cffdb581.jpg)

![](https://github.com/andrebalagot0805/andrebalagot0805.github.io/blob/main/6fdfb96d-2e69-43bb-9ac9-ee8ae8178708.jpg)

![](https://github.com/andrebalagot0805/andrebalagot0805.github.io/blob/main/271c0b4a-3b3a-4446-95d9-ce96124482e5.jpg)

![](https://github.com/andrebalagot0805/andrebalagot0805.github.io/blob/main/24265f61-541d-4428-a085-904874879775.jpg)

![](https://github.com/andrebalagot0805/andrebalagot0805.github.io/blob/main/106205c9-85b3-4584-ad1b-ca9b5971b7f4.jpg)

![](https://github.com/andrebalagot0805/andrebalagot0805.github.io/blob/main/03146867-1d56-4188-9ee7-e97fa0ebed8b.jpg)


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
