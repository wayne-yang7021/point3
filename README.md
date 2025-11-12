# Point3 - Online Music Studio Booking & Management System

**Point3** is an online booking and management system designed for **0.3 Music Classroom**, Taiwan’s largest music school.  
It allows users to easily reserve rehearsal rooms online with instant email notifications, while administrators can manage all bookings, view schedules, and update room details through a dedicated backend dashboard.


## Features

- Online booking system for rehearsal rooms  
- Real-time schedule viewing  
- Automatic email notifications  
- Admin dashboard for booking management  
- Shared PostgreSQL database for both user and admin interfaces  
- Deployed with Vercel for scalability and reliability


## Tech Stack

| Layer | Technologies |
|-------|---------------|
| Frontend | Next.js, TypeScript, Tailwind CSS |
| Backend | Next.js API Routes, Prisma ORM |
| Database | PostgreSQL (Neon.tech) |
| Email Service | Nodemailer |
| Deployment | Vercel |

---

## Local Installation and Testing

Follow the steps below to run **Point3** locally on your machine.

### 1. Clone the repository

```bash
git clone https://github.com/wayne-yang7021/point3.git
cd point3
```


### 2. Install dependencies

```bash
yarn install
```

### 3. Create an .env.local file in the root directory
```bash
POSTGRES_URL=postgresql://HankWu37878:0pZn8WfrVqMI@ep-dawn-sun-82751177.ap-southeast-1.aws.neon.tech/point3?sslmode=required
NEXT_PUBLIC_BASE_URL=http://localhost:3000
```

| Replace credentials with your own valid Postgres connection string if needed.

### 4. Run database migrations
```bash
yarn migrate
```

### 5. Start the development server
```bash
yarn dev
```

The app should now be running at http://localhost:3000

### Live Demo

- User Site: https://point3.vercel.app/
- Admin Dashboard: https://point3-admin.vercel.app/

### Future Improvements

- Improved UI/UX for better usability
- Add user authentication and profile management
- Integrate payment gateway for online booking
- Real-time notifications and analytics dashboard for administrators
