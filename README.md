# Anjuman E Islam Shikaripura — Private Management Website

Professional English full-stack website for marriage hall availability/enquiries and Anjuman administration.

## Included
- Responsive public website with live date-based hall availability checks
- Booking enquiry form (creates **pending enquiries only**; never auto-confirms)
- Required booking documents section
- Private admin dashboard for enquiries, rentals, rent/advance amounts, agreements/tenders and expiry dates, donations, office records, and hall bookings
- Searchable/admin table views and enquiry approve/reject workflow
- Supabase PostgreSQL backend with Row Level Security (RLS)
- Private Supabase Edge Function deployment implementation
- Vercel-compatible static/serverless implementation under `/api`
- Realistic sample records where source records were unavailable

## Live deployment
The production preview uses the Supabase Edge Function `anjuman-private` in project `dssrjvbdmavahvesnmyq`.

The URL and access credentials are intentionally not stored in this source archive. Keep the credentials from the ChatGPT handoff private.

## Local validation
Run:

```bash
npm test
```

This checks the project structure and JavaScript syntax.

## Data safety
Public enquiries are inserted with status `pending`. No external booking or payment is automatically submitted or confirmed. Administrative records are protected by RLS and a server-controlled admin session header.
