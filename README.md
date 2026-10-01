# qhph
mi-mvp/
├── apps/
│   ├── web/                  # Frontend (SPA)
│   │   ├── src/
│   │   │   ├── components/
│   │   │   ├── pages/        # o routes/ / app/
│   │   │   ├── hooks/
│   │   │   ├── lib/
│   │   │   │   ├── firebase.ts    # init del SDK cliente (solo Auth)
│   │   │   │   └── api.ts         # cliente HTTP al back
│   │   │   ├── store/             # estado global (si aplica)
│   │   │   └── main.tsx
│   │   ├── index.html
│   │   ├── package.json
│   │   └── vite.config.ts
│   │
│   └── api/                  # Backend (API)
│       ├── src/
│       │   ├── routes/            # endpoints
│       │   ├── services/          # lógica de negocio
│       │   ├── repositories/       # acceso a Firestore/Firebase
│       │   ├── middleware/
│       │   │   └── auth.ts         # verifyIdToken
│       │   ├── config/
│       │   │   └── firebase-admin.ts
│       │   └── index.ts
│       ├── package.json
│       └── tsconfig.json
│
├── packages/
│   └── contracts/            # SOLO tipos y contratos compartidos
│       ├── src/
│       │   └── index.ts       # DTOs, tipos de request/response
│       └── package.json
│
├── .env.example
├── .gitignore
├── package.json              # scripts raíz (dev, build)
├── pnpm-workspace.yaml       # o turbo.json
├── firebase.json
├── firestore.rules          # cerradas al cliente
└── README.md
