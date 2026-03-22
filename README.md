# Instagram Post Saving App

A web application that allows users to save and organize Instagram posts for content inspiration and reference.

## Features

- 🔖 Save Instagram posts via URL or screenshot upload
- 📁 Organize saved posts into custom categories and folders
- 🔍 Search and filter saved posts
- 📝 Add personal notes to saved posts
- 📤 Export saved posts as image collections
- 🔐 User authentication and personalized content

## Tech Stack

- **Frontend**: Next.js 15, React 19, TypeScript
- **Backend**: Supabase (PostgreSQL, Authentication, Storage)
- **Styling**: Tailwind CSS
- **Deployment**: Vercel (recommended)

## Getting Started

### Prerequisites

- Node.js 18+ 
- A Supabase project

### Installation

1. Clone the repository:
```bash
git clone <your-repo-url>
cd instagram-post-saving-app
```

2. Install dependencies:
```bash
npm install
```

3. Set up environment variables:
```bash
cp .env.example .env.local
```

Fill in your Supabase credentials in `.env.local`:
```env
NEXT_PUBLIC_SUPABASE_URL=your_supabase_project_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
SUPABASE_SERVICE_ROLE_KEY=your_supabase_service_role_key
```

4. Run the database migrations:
   - Go to your Supabase project dashboard
   - Navigate to SQL Editor
   - Copy and run the contents of `supabase/migrations/001_initial.sql`

5. Start the development server:
```bash
npm run dev
```

6. Open [http://localhost:3000](http://localhost:3000) in your browser.

## Database Schema

The app uses two main tables:

- **saved_posts**: Stores Instagram posts with metadata, notes, and categories
- **categories**: User-defined categories for organizing posts

## Features Roadmap

### Phase 1 (Current)
- [x] User authentication
- [x] Basic database schema
- [ ] Save posts via URL
- [ ] Basic post organization

### Phase 2 (Planned)
- [ ] Screenshot upload functionality
- [ ] Advanced search and filtering
- [ ] Category management
- [ ] Personal notes system

### Phase 3 (Future)
- [ ] Export functionality
- [ ] Mobile app version
- [ ] Bulk operations
- [ ] Content recommendations

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License.