VOID MC TIERS — LIVE DATABASE VERSION

WHAT THIS VERSION DOES
- Public index.html reads players from Supabase.
- admin.html lets you sign in and add/update/delete players.
- Changes are stored online, so you can publish the website once and keep adding players.
- Tier system: HT1/MT1/LT1 through HT5/MT5/LT5.
- Gamemodes: AXE PVP, CART PVP, DIA KIT, E-MACE, NETPOT, SMP KIT, SPEAR MACE, TANK, UHC, VANILLA CRYSTAL.

ONE-TIME SETUP
1. Create a Supabase project.
2. Open SQL Editor and run supabase.sql.
3. Open Authentication -> Providers -> Email and enable Email.
4. Open Project Settings -> API and copy the Project URL and anon/publishable key.
5. Put them in supabase-config.js.
6. Upload index.html, admin.html and supabase-config.js to your GitHub repository.
7. Enable GitHub Pages.
8. Visit /admin.html, create your admin account, then add players.

IMPORTANT SECURITY NOTE
The public site can read players, while only signed-in users can write under the included policies.
For a production server, restrict the write policies to a specific admin role/account rather than every authenticated account.
