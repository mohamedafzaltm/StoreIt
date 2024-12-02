# Store It - File Storage & Sharing Platform

A modern file storage and sharing platform built with Next.js 15, TypeScript, and Appwrite.

## Setup Guide

### Prerequisites
- Node.js (v18 or higher)
- npm or yarn
- Appwrite Account

### 1. Clone and Install Dependencies
```bash
git clone <your-repo-url>
cd store-it
npm install
```

### 2. Appwrite Setup
1. Create an account at [Appwrite Cloud](https://cloud.appwrite.io)
2. Create a new project
3. Go to "Storage" and create a new bucket
   - Enable "Read" and "Write" permissions
4. Go to "Database" and create a new database
5. Create two collections:
   - Users Collection
   - Files Collection
6. Create an API key with the following permissions:
   - files.read
   - files.write
   - documents.read
   - documents.write

### 3. Environment Variables
Create a `.env.local` file in the root directory:
```env
NEXT_PUBLIC_APPWRITE_ENDPOINT="https://cloud.appwrite.io/v1"
NEXT_PUBLIC_APPWRITE_PROJECT="your-project-id"
NEXT_PUBLIC_APPWRITE_DATABASE="your-database-id"
NEXT_PUBLIC_APPWRITE_USERS_COLLECTION="your-users-collection-id"
NEXT_PUBLIC_APPWRITE_FILES_COLLECTION="your-files-collection-id"
NEXT_PUBLIC_APPWRITE_BUCKET="your-bucket-id"
NEXT_APPWRITE_KEY="your-api-key"
```

### 4. Run the Development Server
```bash
npm run dev
```
Open [http://localhost:3000](http://localhost:3000) in your browser.

## Features
- File Upload & Management
- File Sharing
- Real-time Search
- File Type Filtering
- Storage Usage Analytics
- Responsive Design

## Tech Stack
- Next.js 15
- TypeScript
- Tailwind CSS
- Appwrite
- React Hook Form
- Shadcn UI

## Project Structure
- `/app` - Next.js app router pages
- `/components` - Reusable UI components
- `/lib` - Utility functions and configurations
- `/public` - Static assets
- `/types` - TypeScript type definitions

## Support
For any issues or questions, please contact me on tm.mohamedafzal@gmail.com