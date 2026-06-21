This governs the product, the scope, and the quality bar for this run. Treat it as the highest-priority directive layered above every phase.

PRODUCT
Build a small but exceptionally polished web product: a digital greeting-card / postcard creator. A visitor picks one of a few beautiful visual themes, writes a short message and a signature, and gets a shareable link. Opening that link shows the card full-screen with a tasteful reveal animation. A compact gallery shows the most recently created cards. Derive a neutral, friendly product name and slug yourself from the concept — no reference to any tooling, vendor, platform, or internal process in any on-screen name.

SCOPE — hard cap, do not exceed

- At most 3 epics. Each epic at most 3 small tasks.
- Ship the smallest implementation that fully works and looks great. Build nothing beyond what the create / share / gallery flow needs. No auth, no accounts, no admin panel, no payments, no analytics, no notifications.
- Keep the founding documents short and focused. Do not expand scope between phases — the plan you commit to at the start is the plan you ship.

QUALITY BAR — visual design is the single most important success criterion

- The UI must be genuinely beautiful and modern, not a wireframe: a cohesive color system, refined typography and generous spacing, a strong hero, fully responsive layout (mobile and desktop), and subtle, tasteful motion (reveal and transitions). Treat this as a portfolio-grade showcase piece.
- The themes the user can pick for a card must each look distinctly gorgeous (e.g. layered gradients, soft shadows, elegant type pairings).
- Use a clean modern frontend stack (React) with a well-structured design system / CSS. Cover accessibility basics: sufficient contrast, visible focus states, semantic markup.

PERSISTENCE — minimal, emulated, zero real infrastructure

- The datastore connection is already provisioned for you as DATABASE_URL (present in the project .env and in the run context). It is an embedded SQLite file standing in for a managed Postgres. Use that DATABASE_URL for the small amount of persistence the cards need: store a created card, fetch one by id, list the most recent.
- Do NOT install or stand up any external or real database, container, broker, or background service. Do not add Postgres, Supabase, Docker, Redis, or any server process. Persistence is limited to the provided embedded store only.
- Minimal working functionality is the goal — just enough that the live demo behaves flawlessly and looks stunning. Favor polish over breadth everywhere.

Everything else follows the standard pipeline unchanged: brainstorm the founding documents, scaffold, provision, implement with TDD, self-review, finalize, deploy, and verify the live site returns 200.
