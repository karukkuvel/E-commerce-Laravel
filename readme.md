
## Installation

1. Clone the repo and `cd` into it
2. `composer install`
3. Rename or copy `.env.example` file to `.env`
4. `php artisan key:generate`
5. Set your database credentials in your `.env` file
6. Set your Stripe credentials in your `.env` file. Specifically `STRIPE_KEY` and `STRIPE_SECRET`
7. Set your Algolia credentials in your `.env` file. Specifically `ALGOLIA_APP_ID` and `ALGOLIA_SECRET`.
8. Set your Braintree credentials in your `.env` file if you want to use PayPal. Specifically `BT_MERCHANT_ID`, `BT_PUBLIC_KEY`, `BT_PRIVATE_KEY`.
9. Set your `APP_URL` in your `.env` file. This is needed for Voyager to correctly resolve asset URLs.
10. Set `ADMIN_PASSWORD` in your `.env` file if you want to specify an admin password. If not, the default password is 'password'
11. `php artisan ecommerce:install`. This will migrate the database and run any seeders necessary.
12. `npm install`
13. `npm run dev`
14. `php artisan serve` or use Laravel Valet or Laravel Homestead
15. Visit `localhost:8000` in your browser
16. Visit `/admin` if you want to access the Voyager admin backend. Admin User/Password: `admin@admin.com/password`. Admin Web User/Password: `adminweb@adminweb.com/password`
