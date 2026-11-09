# Roadmap

- [x] Add live work tracking for both accounts, required reasons, three-hour check-ins, private/public statistics and Master Calendar hours; verified start/switch/end, actual check-in and mobile layout; removed temporary work records.

- [x] Add approved email outreach batches of up to 20, message history and three-day reminders inside Leads; tested a real send to the connected inbox and removed the test lead.
- [x] Connect Gmail and restrict its sender to the requesting account.
- [ ] Enable WhatsApp batch sending — blocked: WhatsApp connection was declined; WhatsApp drafts remain available.

- [x] Fix Money circles from saved client fees, payments and subscriptions; verified immediate edit updates, 15 tests passed, and temporary records removed.

- [x] Make the app installable on a phone (home-screen icon, no offline caching).

- [x] Turn Total made / Pending money into rings so the profile Info block has three circles.
- [x] Slim the compact Notes block on client profiles (tighter heading, search and cards).
- [x] Hide the top navigation bar on client profile pages.
- [x] Add a saved price option to SMM projects without changing Money totals.
- [x] Remove the Services block from Eclipse client profiles, preserving saved service data.
- [x] Replace the client profile Info rows with Total made / Pending money bars and a three-option stage ring; drop the Status block.


- [x] Add master and business calendars with linked, color-coded records.
- [x] Add master and business notes with cross-references.
- [x] Reshape workspace chooser around master views and My Businesses.
- [x] Add Eclipse SMM projects, post planning and client/fee links without double-counting retainers.
- [ ] Connect and publish to social platforms — blocked: LinkedIn connection was declined; other platforms need authorized publishing connections.
- [x] Improve Money loading/progress and accurate linked live figures.
- [x] Verify signed-in note and SMM creation/readback, master cross-references, business isolation, mobile layout and 17 calculation tests; remove verification records.

- [x] Build an isolated TapTables workspace with Map, Clients, Money and Reps.
- [x] Add persistent TapTables clients, orders, payments, costs, stock and installation/support tracking.
- [x] Track assigned reps, sales and configurable commissions; keep optional care plans separate from order revenue.
- [x] Verify signed-in creation/editing, calculations, workspace isolation and all four tab shells; Google Maps live rendering/search requires user validation on an authorized app origin, because sandbox Maps testing is unsupported.

- [x] Rename the third workspace to TapTables and verify the selector.
- [x] Review taptables.store and recommend order-based business tracking sections before building the separate workspace.

- [x] Move map search to a two-stage left-panel workflow with completion ticks, criteria-based AI rating and locked results; remove status options.
- [x] Map: drop the results heading, service filter and sort control; header keeps only Add place and Log out.

- [x] Remove Follow-ups, Lead Generation and Pipeline pages and related client controls; preserve stored records.

- [x] Phase 1 database migration (lead fields, lead_activities, follow_ups, ai_insights, change_lead_stage)
- [x] Reconnect Google Maps Platform in new workspace
- [x] Lead types + data-access module (src/lib/leads.ts)
- [x] Lead section on client profile
- [x] /pipeline board route (+ Lost / Do not contact)
- [x] Phase 2A AI Qualification on client profile
- [x] Reconnect Google Maps Platform (new workspace)
- [x] Map page: split view — business list (left) + map (right), AI-rate up to 20
- [x] Use full page width on screen from image-4 to fit on one page
- [x] Lead Generation center page (UI/config only)

- [x] Clients table + CRUD, Money payments tracker, client↔money linking
- [x] Reconnect Google Maps Platform in new workspace

- [x] Client profile: remove the Lead block and place Notes above Billing.
- [x] Client profile: move the social media (SMM) block under Billing.
- [x] Client profile calendar: fee-due blocks yellow, work blocks blue.
- [x] Map: AI match notes shown as green bullet points with why/how reasons; verified on a live search and service match.
