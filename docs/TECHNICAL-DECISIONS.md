# Technical Decisions — ARUSnya

## 1. Next.js App Router

**Decision:** Use Next.js App Router for the web application.

**Rationale:**
- Provides structured routing and layouts.
- Supports server-side rendering and server-side data access where appropriate.
- Integrates with the Vercel deployment platform.

## 2. Supabase and PostgreSQL

**Decision:** Use Supabase with PostgreSQL for application data.

**Rationale:**
- Provides a relational database.
- Supports structured queries and data management.
- Reduces the operational overhead of maintaining a separate database server.

## 3. AI-Assisted Summarization

**Decision:** Use an AI language model to help summarize news in Indonesian.

**Rationale:**
- Makes articles more accessible to Indonesian readers.
- Helps readers understand key points more quickly.

**Trade-off:** AI-generated summaries can omit context or contain inaccuracies, so they should not be treated as a substitute for the original reporting.

## 4. Automated News Ingestion

**Decision:** Use scheduled automation to retrieve and process news.

**Rationale:**
- Reduces the need for manual updates.
- Helps keep the article collection refreshed.

**Trade-off:** Data freshness depends on the news provider, schedule reliability, rate limits, and processing success.

## 5. Managed Deployment

**Decision:** Deploy the application using Vercel.

**Rationale:**
- Integrates with the Next.js ecosystem.
- Simplifies deployment and hosting workflows.

## Summary

These decisions prioritize maintainability, automated content processing, and a practical deployment workflow for a small news platform.
