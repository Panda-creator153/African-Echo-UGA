# African Echo - Official Website

A full-stack web application for African Echo, a Ugandan singer, songwriter, and sonic architect based in Kampala, Uganda.

## 🎵 Project Overview

African Echo is a modern, responsive website showcasing:
- **Music Platform** - Tracks, albums, and lyrics management
- **Gallery** - Image showcase of performances and events
- **Booking System** - Event booking requests and management
- **Contact System** - Direct messaging and inquiries
- **Admin Dashboard** - Content management interface

## 🛠️ Tech Stack

### Frontend
- **React 19** - UI framework
- **Vite** - Build tool and dev server
- **Tailwind CSS** - Utility-first CSS framework
- **Lucide React** - Icon library
- **Motion** - Animation library
- **React Router** - Navigation

### Backend & Database
- **Firebase** - Authentication & Firestore database
- **Supabase** - Alternative database and file storage
- **Express.js** - Server framework (optional)
- **Google Gemini API** - AI integration

### Development Tools
- **TypeScript** - Type safety
- **ESBuild** - Fast bundler
- **Multer** - File upload handling
- **CORS** - Cross-origin resource sharing

## 📁 Project Structure

```
.
├── metadata.json                 # Project metadata
├── .env.example                  # Environment variables template
├── .gitignore                    # Git ignore rules
├── index.html                    # Main HTML entry point
├── package.json                  # Dependencies
├── package-lock.json             # Locked dependency versions
├── firebase-applet-config.json   # Firebase configuration
├── firebase-blueprint.json       # Database schema blueprint
├── firestore.rules               # Firestore security rules
├── src/                          # Source code (extracted separately)
└── README.md                     # This file
```

## 🔐 Firestore Database Schema

### Collections
- **settings/main** - Global site configuration and branding
- **home/main** - Homepage content
- **about/main** - About page biography
- **booking/main** - Booking page information
- **contact/main** - Contact page details
- **tracks/{trackId}** - Music tracks collection
- **albums/{albumId}** - Albums collection
- **videos/{videoId}** - Music videos collection
- **gallery/{imageId}** - Gallery images collection
- **bookings/{bookingId}** - Booking requests
- **contacts/{messageId}** - Contact messages
- **admins/{adminId}** - Admin users

## 🔑 Environment Variables

Create a `.env` file based on `.env.example`:

```bash
# Gemini AI API
GEMINI_API_KEY=your_gemini_api_key

# App URL
APP_URL=https://your-domain.com

# Admin Access
ADMIN_PASSWORD=your_secure_password

# Supabase Configuration
SUPABASE_URL=your_supabase_url
SUPABASE_ANON_KEY=your_anon_key
SUPABASE_SERVICE_ROLE_KEY=your_service_role_key
SUPABASE_BUCKET_NAME=uploads

# Google Picker API (optional)
VITE_GOOGLE_PICKER_API_KEY=your_google_picker_api_key
```

## 🚀 Getting Started

### Prerequisites
- Node.js 18+
- npm or yarn
- Firebase project
- Supabase project (optional)

### Installation

```bash
# Clone the repository
git clone https://github.com/Panda-creator153/African-Echo-UGA.git
cd African-Echo-UGA

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env
# Edit .env with your configuration

# Start development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## 🔒 Security

### Firestore Rules
The project includes comprehensive Firestore security rules (`firestore.rules`) that:
- Deny access by default
- Allow public read access to content (tracks, albums, videos, gallery)
- Restrict write access to authenticated admins
- Validate all incoming data
- Protect admin collection

### Admin Authentication
- Bootstrap admin: `silinkjay43@gmail.com`
- Admins verified via Firestore `admins` collection
- Email verification required

## 📝 Available Scripts

```bash
npm run dev          # Start development server
npm run build        # Build for production
npm run preview      # Preview production build
npm run lint         # Run linter
npm run type-check   # Run TypeScript type checking
```

## 🤝 Contributing

This is a personal artist website. For contributions or issues, please contact the repository owner.

## 📄 License

This project is proprietary. All rights reserved.

## 👤 Artist

**African Echo**
- Email: silinkjay43@gmail.com
- Location: Kampala, Uganda
- Genre: Electronic Soul, Cinematic Music

---

**Last Updated:** June 4, 2026
