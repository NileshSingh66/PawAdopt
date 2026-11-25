# PawAdopt 🐾

**PawAdopt – Pet Adoption Platform**

Maintained by **Nilesh Singh**

PawAdopt is a pet adoption platform where users can submit pets for adoption, while administrators review and approve pet listings before they become publicly visible.

## 🚀 Tech Stack

- Next.js
- React.js
- TypeScript
- MongoDB
- NextAuth.js
- Cloudinary

## ✨ Features

- Pet listing submission and management.
- Admin review and approval of pet listings.
- Approved pets are displayed publicly.
- Cloudinary integration for pet image uploads.
- Authentication using NextAuth.js.
- Automatic account restrictions after five rejected pet submissions.
- Admins can remove account restrictions.

## ⚙️ Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/NileshSingh66/PawAdopt.git
cd PawAdopt
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Configure Environment Variables

Create a `.env.local` file in the root directory and add the following variables:

```env
MONGODB_URI=your_mongodb_uri
NEXTAUTH_SECRET=your_nextauth_secret
NEXTAUTH_URL=http://localhost:3000
NEXT_PUBLIC_BASE_URL=http://localhost:3000

CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
```

Replace the placeholder values with your actual credentials.

**Important:** Never upload your `.env.local` file or expose your API keys and secrets on GitHub.

### 4. Run the Development Server

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

## 🌐 Production Deployment

The application is configured for deployment on Vercel.

Set the following environment variables in your Vercel project:

```env
NEXTAUTH_URL=https://paw-adopt.vercel.app
NEXT_PUBLIC_BASE_URL=https://paw-adopt.vercel.app
```

Also configure your production database, authentication secret, and Cloudinary credentials.

### Google OAuth Configuration

Add the following authorized redirect URI to your Google OAuth configuration:

```text
https://paw-adopt.vercel.app/api/auth/callback/google
```

## 📂 Project Structure

The application uses the Next.js App Router.

The main application page can be modified in:

```text
app/page.tsx
```

## 📚 Useful Resources

- [Next.js Documentation](https://nextjs.org/docs)
- [React Documentation](https://react.dev/)
- [MongoDB Documentation](https://www.mongodb.com/docs/)
- [NextAuth.js Documentation](https://next-auth.js.org/)
- [Cloudinary Documentation](https://cloudinary.com/documentation)
- [Vercel Deployment](https://vercel.com/docs)



PawAdopt – Helping pets find their forever homes. 🐾

