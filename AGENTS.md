<!-- LOVABLE:BEGIN -->
> [!IMPORTANT]
> This project is connected to [Lovable](https://lovable.dev). Avoid rewriting
> published git history — force pushing, or rebasing/amending/squashing commits
> that are already pushed — as it rewrites history on Lovable's side and the
> user will likely lose their project history.
>
> Commits you push to the connected branch sync back to Lovable and show up in
> the editor, so keep the branch in a working state.
<!-- LOVABLE:END -->

- Navigation is selected by URL namespace: SA has Map, Clients, Money, SMM, Calendar and Notes; TapTables has Map, Clients, Money, Reps, Calendar and Notes; master views have their own navigation to prevent workspace state leaking.
- Map category searches use an explicit locked result set, and AI rating receives a separate user criterion; panning must not replace reviewed results.
- TapTables persists only in owner-scoped tt_* tables with composite owner foreign keys; SA records must never be reused or mutated by TapTables features.
- TapTables order totals derive from saved line quantities/prices/costs; stock on hand is an explicit balance, not automatically decremented, to avoid duplicate fulfilment adjustments.
- TapTables commissions use each order's saved rate applied to collected revenue; care-plan contracted values remain separate from order income, and payments cannot exceed an order's balance.
- The business hub aggregates owner-scoped source records read-only; editable planning records live in separate sa_* and tt_* tables with owner-linked client foreign keys so master views do not duplicate or move business data.
- SMM projects reference SA clients and report their full existing retainers once per client; never add these figures to Money as additional fees or claim unconnected platform publishing succeeded.
- SMM project prices are saved quoted amounts, separate from client retainers; editing a quote must not mutate billing or collected revenue.
- Mobile installability is manifest-only (public/manifest.webmanifest, public/icons, head tags in src/routes/__root.tsx); add no service worker, offline caching or vite-plugin-pwa unless the user explicitly asks for offline use.
- SA Money uses shared monthly-money calculations and source query keys; saved unpaid monthly rows replace inferred fee balances to avoid duplicate forecasts, and edit invalidations refresh cached totals before navigation.
- Lead email sends require a server-checked owner sender grant and persistent attempt IDs; never expose a connected mailbox to unrelated app accounts or replay ambiguous send outcomes.
- Work tracking uses owner-only base reads and authenticated database functions for minimal shared presence; private session data stays hidden, role titles confer no privileges, and every continued task starts a capped session segment.
