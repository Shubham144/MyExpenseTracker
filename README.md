# MyExpenseTracker

Personal single-user expense tracker using ASP.NET Core 8, SQL Server, IIS and React/Vite.

Features: single Alchemist login; SQL-stored password hash with SQL-only password changes; INR-only Bank/Cash accounts; editable accounts; expense/income CRUD; static categories; monthly category budgets; 12-month dashboard.

Setup: run `database/schema.sql`; generate a hash with `dotnet run --project tools/PasswordHashTool -- "your-password"`; update the Alchemist row in SQL Server; configure the SQL connection; run the API and React app. See `docs/IIS.md` for IIS and `docs/CLOUDFLARE_TUNNEL.md` for public HTTPS without a client VPN.

Never commit production credentials or tunnel tokens. Keep SQL Server private.