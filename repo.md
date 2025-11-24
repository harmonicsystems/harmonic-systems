# Harmonic Systems Repository Structure

## Monorepo Architecture with Turborepo

```
harmonic-systems/
├── apps/
│   ├── studio-web/          # Main studio website & landing
│   ├── house-concerts/      # Concert booking platform
│   ├── lullaby-lab/         # f₀ analysis & parent tools
│   ├── folk-lineage/        # Cultural documentation system
│   └── loop-builder/        # Musical loop creation tool
│
├── packages/
│   ├── ui/                  # Shared component library
│   │   └── tokens/          # Low-stimulation design system
│   ├── audio-core/          # Audio processing utilities
│   ├── auth/                # Shared authentication
│   ├── db/                  # Database schemas & migrations
│   └── config/              # Shared configuration
│
├── services/
│   ├── api/                 # Unified backend API
│   └── workers/             # Background jobs (audio processing)
│
├── infrastructure/
│   ├── terraform/           # Infrastructure as code
│   └── docker/              # Container definitions
│
├── content/
│   ├── sessions/            # Session plans & curricula
│   ├── traditions/          # Folk music documentation
│   └── resources/           # Participant resources
│
└── tools/
    ├── scripts/             # Build & deployment scripts
    └── migrations/          # Data migration tools
```

## Quick Start Commands

```bash
# Clone and setup
git clone https://github.com/[your-username]/harmonic-systems.git
cd harmonic-systems
pnpm install

# Development
pnpm dev                     # Start all apps in dev mode
pnpm dev --filter studio-web # Start specific app

# Build
pnpm build                   # Build all apps
pnpm build:studio           # Build studio website

# Deploy
pnpm deploy:vercel          # Deploy to Vercel
```

## Design Principles

### Low-Stimulation UI by Default
- Muted colors (#2c3e50, #7f8c8d)
- Generous whitespace
- No auto-playing media
- Predictable interactions
- Clear visual hierarchy

### Progressive Enhancement
- Works without JavaScript
- Enhanced with interactivity
- Offline-capable where appropriate
- Fast on slow connections

### Data Ownership
- Export everything
- No vendor lock-in
- Local-first where possible
- Clear data retention policies

## Git Branch Strategy

```
main                        # Production-ready code
├── develop                 # Integration branch
└── feature/[name]         # Feature branches
```

## Environment Variables

```env
# .env.example
DATABASE_URL=
NEXTAUTH_SECRET=
STRIPE_SECRET_KEY=          # For sliding scale payments
TWILIO_ACCOUNT_SID=        # For SMS reminders (optional)
AWS_S3_BUCKET=             # For audio storage
```

## Initial Milestones

1. **Week 1-2**: Studio landing page live
2. **Week 3-4**: Basic session booking
3. **Month 2**: House concerts MVP
4. **Month 3**: Lullaby Lab prototype
5. **Month 4-6**: Folk Lineage & Loop Builder

## Contributing Guidelines

This is primarily a personal practice platform, but if you're interested in contributing:

1. Focus on accessibility first
2. Respect the analog-first philosophy
3. Test with slow connections
4. Consider neurodivergent users
5. Document cultural sources

## License

[Consider: MIT for open tools, proprietary for curricula]

---

*Building digital infrastructure for analog experiences.*