# 🚗 Vehiql – AI-Powered Car Marketplace

Vehiql is a modern car marketplace built with **React.js** that allows users to explore cars, compare vehicle details, save favorites, calculate monthly EMI payments, and book test drives.

🌐 **Live Website:** https://vehiql-tau.vercel.app/

## ✨ Features

- 🚘 **Browse Cars** – Explore available vehicles with detailed specifications.
- 🔍 **Search & Filter** – Find cars based on your preferences.
- 💰 **EMI Calculator** – Estimate monthly payments for your desired vehicle.
- ❤️ **Saved Cars** – Save your favorite vehicles for later.
- 📅 **Test Drive Booking** – Schedule test drives for selected cars.
- 🔐 **Authentication** – Secure sign-up and sign-in using Clerk.
- 🛠️ **Admin Dashboard** – Manage vehicle listings, bookings, and dealership settings.
- 🖼️ **Image Storage** – Manage vehicle images using Supabase Storage.
- 🤖 **AI Integration** – AI-powered functionality using Google Gemini.
- 🛡️ **Security** – Application protection using Arcjet.

## 🛠️ Tech Stack

- **Frontend:** React.js
- **Styling:** Tailwind CSS
- **UI Components:** Radix UI, Lucide React
- **Authentication:** Clerk
- **Database:** PostgreSQL
- **ORM:** Prisma
- **Storage:** Supabase
- **AI:** Google Gemini
- **Security:** Arcjet
- **Form Handling & Validation:** React Hook Form, Zod
- **Deployment:** Vercel

## 🌐 Live Demo

Explore the live application:

👉 https://vehiql-tau.vercel.app/

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone <your-github-repository-url>
cd Vehiql
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Configure Environment Variables

Create a `.env` file in the root directory and add your service credentials:

```env
DATABASE_URL="your_postgresql_connection_string"
DIRECT_URL="your_direct_database_connection_string"

NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY="your_clerk_publishable_key"
CLERK_SECRET_KEY="your_clerk_secret_key"

NEXT_PUBLIC_SUPABASE_URL="your_supabase_project_url"
NEXT_PUBLIC_SUPABASE_ANON_KEY="your_supabase_anon_key"

GEMINI_API_KEY="your_gemini_api_key"

ARCJET_KEY="your_arcjet_key"
```

Replace the placeholder values with your actual credentials. Never upload your `.env` file or secret API keys to GitHub.

### 4. Set Up the Database

```bash
npx prisma generate
npx prisma db push
```

Ensure your PostgreSQL database is configured and accessible before running these commands.

### 5. Run the Development Server

```bash
npm run dev
```

Open your browser and visit:

http://localhost:3000

## 📂 Project Structure

```text
Vehiql/
├── actions/          # Server actions and application logic
├── app/              # Application routes and pages
│   ├── (admin)/      # Admin dashboard
│   ├── (auth)/       # Authentication pages
│   ├── (main)/       # Main marketplace pages
│   └── api/          # API routes
├── components/       # Reusable UI components
├── lib/              # Utilities and service configurations
├── prisma/           # Prisma schema and database models
├── public/           # Static assets
├── middleware.js     # Middleware and security configuration
├── package.json      # Dependencies and scripts
└── README.md         # Project documentation
```

## 🚀 Deployment

The application is deployed on Vercel.

To deploy your own version:

1. Push your project to GitHub.
2. Import the repository into Vercel.
3. Configure all required environment variables.
4. Connect your PostgreSQL database and Supabase project.
5. Deploy and test the application.

## 🔒 Security

- Keep API keys and database credentials private.
- Configure authentication and authorization properly.
- Restrict admin access to authorized users.
- Configure database permissions and storage policies securely.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome.

1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Push the branch to GitHub.
5. Open a pull request.

## 📄 License

No license has been specified yet. Add a `LICENSE` file if you intend to distribute this project as open-source software.

---

**Built with ❤️ using React.js and modern web technologies.**

🌐 **Live Demo:** https://vehiql-tau.vercel.app/
