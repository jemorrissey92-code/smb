# AI Agent Instructions for Fractional Growth Officer AI System

## Project Overview
This is an AI-powered marketing strategy platform that delivers enterprise-grade growth consulting to small service businesses (contractors, trades, local professionals) at fractional costs. Built on Claude AI with local New England market expertise.

**Core Mission:** Democratize strategic marketing expertise previously only available to $10K+/month agency clients.

## Architecture & Tech Stack
- **Current:** HTML/React (CDN) single-page app with Gemini AI integration for proposal automation
- **Future:** Next.js web app + Supabase CRM + Pinecone vector DB for RAG + Vercel hosting
- **Layers:** UI → AI Engine (Gemini/Claude) → Knowledge Base (playbooks/templates) → Integrations (Google APIs, Notion, SEO tools)

## Domain Knowledge
- **Target Market:** RI/MA/CT small businesses ($250K-$5M revenue, 1-25 employees)
- **Priority Verticals:** Skilled trades (HVAC/plumbing/electrical), home services, local professionals
- **Marketing Channels:** Google Business Profile, Local SEO, Social Media, Email, Paid Ads, Website optimization
- **Key Principles:** Strategy before tactics, simplicity scales, local-first, owner-centric, measurable outcomes

## User Personas
- **Mike (Tradesman):** 38-55, owner-operator, skeptical of marketing, wants phone to ring, time-starved
- **Sarah (Solopreneur):** 28-42, scaling service business, overwhelmed by options, needs structured guidance

## Development Patterns
- **Playbooks:** Channel-specific frameworks (e.g., GBP optimization: complete profile → post weekly → respond immediately → request reviews)
- **Templates:** Industry-tailored content (trades focus on visual proof, services on reviews/referrals)
- **Local Focus:** New England market data, seasonal considerations, competitive landscape
- **Measurement:** ROI-focused recommendations with specific KPIs (lead cost, conversion rates, customer acquisition cost)
- **AI Integration:** Use Gemini API for content generation (e.g., `callGemini(prompt, systemInstruction)` with JSON parsing for structured outputs)
- **UI Patterns:** Modal-based AI interactions, real-time preview panels, print-optimized layouts
- **State Management:** React useState for form data, array manipulation for dynamic lists (e.g., proposal items)

## Implementation Guidelines
- Reference `prd` file for detailed requirements and user flows
- Build for delegation: owners want to hand off execution to staff
- Prioritize simplicity: avoid overwhelming interfaces/features
- Include local market context in all recommendations
- Structure outputs as actionable playbooks, not generic advice
- Focus on measurable outcomes with clear success metrics
- **AI Prompting:** Use system instructions for structured JSON outputs, clean markdown from responses
- **Print Functionality:** Include `@media print` styles, hide `.no-print` elements, show `.print-only` for PDF generation
- **Error Handling:** Graceful API failure with user alerts, loading states with spinners

## Key Files
- `prd`: Complete product requirements and technical architecture
- `index.html`: Current implementation with React/Gemini integration
- Future: `/playbooks/` for channel-specific strategies, `/templates/` for industry content