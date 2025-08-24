# Zeolf - Business Consulting Website

## Overview

Zeolf is a business consulting website with appointment scheduling, resource management, and social media post planning capabilities. This repository contains a wrapper structure that makes it easy to run the application from the root directory.

## Features

- **Appointment Management**: Schedule, track, and manage client appointments
- **Resource Management**: Create and manage business resources and materials
- **Social Media Integration**: Plan and schedule social media posts

## Database Structure

The application uses SQLite with the following main tables:

### Appointments Table
- `id`: Primary key
- `client_name`: Client's name
- `client_email`: Client's email address
- `company`: Client's company (optional)
- `appointment_type`: Type of appointment (consultation, demo, meeting)
- `date`: Appointment date and time
- `duration`: Length of appointment in minutes
- `notes`: Additional notes
- `status`: Current status (scheduled, confirmed, completed, cancelled)
- `assigned_to`: Staff member assigned to the appointment
- `created_at`: Creation timestamp
- `updated_at`: Last update timestamp

### Resources Table
- `id`: Primary key
- `title`: Resource title
- `description`: Resource description
- `status`: Publication status (draft, published)
- `created_at`: Creation timestamp
- `updated_at`: Last update timestamp

### Social Posts Table
- `id`: Primary key
- `platform`: Social media platform
- `content`: Post content
- `imageUrl`: URL to attached image (optional)
- `scheduledFor`: Scheduled publication date
- `status`: Post status (draft, scheduled, published)
- `created_at`: Creation timestamp
- `updated_at`: Last update timestamp

## Quick Start

This is a wrapper directory for the Zeolf project. You can run npm commands from this directory, and they will be automatically redirected to the project subdirectory.

### Available Commands

```bash
# Start the development server
npm run dev

# Build the project
npm run build

# Start the production server
npm run start

# Check TypeScript types
npm run check

# Push database schema changes
npm run db:push

# Install dependencies
npm install
```

### Alternative Methods

You can also use the batch files to start the application:

```bash
# Run the development server
run-dev.bat

# Build the project
run-build.bat

# Start the production server
run-start.bat
```

## Project Structure

The actual project is located in a subdirectory. This parent directory contains wrapper scripts to make it easier to run commands from this location.