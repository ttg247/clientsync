# ClientSync

ClientSync is a SaaS web application that enables users to sync and manage their HubSpot CRM contacts and tasks via a clean custom dashboard.

Built with Laravel (API backend) and Vue 3 + Pinia (frontend), ClientSync demonstrates a full-stack integration with the HubSpot API, user authentication, and scoped multi-user data management.

---

## Features (MVP)

- User registration and login with Laravel Breeze (API mode)  
- Secure token-based authentication (Laravel Sanctum)  
- Sync and display HubSpot contacts scoped per user  
- Create and update contacts/tasks syncing with HubSpot API  
- Vue 3 frontend with Pinia state management  
- Protected API routes ensuring users see only their own data  

---

## Tech Stack

- Backend: Laravel 12, Sanctum, Breeze (API)  
- Frontend: Vue 3, Pinia, Vite  
- Database: MySQL  
- External API: HubSpot CRM API  

---

## Setup & Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/clientsync.git
    cd clientsync
    ```

2. Install PHP dependencies:

    ```bash
    composer install
    ```

3. Install Node.js dependencies:

    ```bash
    npm install
    npm run dev
    ```

4. Configure environment:

    - Copy `.env.example` to `.env`  
    - Set your database credentials  
    - Add your HubSpot API key or token  

    ```env
    HUBSPOT_API_KEY=your_hubspot_api_key_here
    ```

5. Run database migrations:

    ```bash
    php artisan migrate
    ```

6. Start the Laravel server:

    ```bash
    php artisan serve
    ```

7. Access the frontend app (configured via Vite):

    - The app should be accessible at `http://localhost:3000` or as configured.

---

## API Endpoints

- `POST /api/register` — Register a new user  
- `POST /api/login` — Login and receive auth token  
- `GET /api/clients` — Fetch authenticated user’s HubSpot contacts  
- (More endpoints to be added)

---

## Future Improvements

- Add HubSpot OAuth for user-specific API tokens  
- Implement multi-tenant architecture for organizations/teams  
- Integrate Stripe billing for SaaS subscriptions  
- Add task and engagement management syncing  
- Unit and integration testing  

---

## License

MIT License © Tedtek

---

## Contact

For questions or support, reach out at tedteksolutions@gmail.com
