# TRIADBLUE — Claude Code Standing Instructions
# This file is read automatically at the start of every session.
# Every agent working on any TRIADBLUE repository must read this entirely before touching any file.
# They must also read: .github/TRIADBLUE_CONTINUITY_BRIEFING.txt before starting any task.

## WHO YOU ARE WORKING FOR

Dean Laskowski, founder of TRIADBLUE Inc.
Non-coder. Moves fast. Exacting standards. Does not tolerate placeholder work.
Every output must be production-ready. No exceptions.

Local machine: Mac Mini. Username: deanlewis. Path: /Users/deanlewis/
GitHub org: TRIADBLUE
Deployment: Replit
LINKBlue GitHub proxy: https://linkblue-githubproxy.up.railway.app

## DOCUMENT CONVENTIONS — EVERY PROMPT, RESPONSE, AND SEGUE

Three document types are universal across all agents and all platforms.

PROMPTS
Initial scoped instructions written by web chat for execution by Claude
Code. Naming format: "Prompt MM/DD/YYYY-N" where N is sequential FOREVER,
never resetting per day or per repo. Numbers climb across all days. The
date is just when the prompt was written; it does NOT reset N. If
yesterday's last prompt was -7, today's first prompt is -8. Drafted-but-
unfired ideas do NOT get a number until Dean approves them as the next
thing to execute.

RESPONSES
Follow-up messages sent into a running session AFTER the prompt is fired.
Naming format: "Response MM/DD/YYYY-Na" where N matches the parent prompt
number and the letter (a, b, c, ...) increments per intervention. Example:
parent prompt is 04/29/2026-3, the first follow-up is Response
04/29/2026-3a, the second is 04/29/2026-3b.

SEGUES
Handoff document written by the agent ending a session, for the agent
picking up next. Captures detailed context, mid-execution decisions, what
was being finished, what is blocking, what is next. Naming format: "Segue
from Prompt MM/DD/YYYY-N" where N is the LAST CLEANLY EXECUTED prompt in
the session (highest-numbered prompt that committed, deployed, and
verified). If a prompt was mid-flight at session end, the segue does NOT
name it as the anchor — it names the last completed prompt and describes
the mid-flight one in the body.

Every agent must write a segue when their session ends, in the context
of what they were actually doing.

PLATFORM HEADER (REQUIRED ON EVERY PROMPT)
Every prompt must include two header lines immediately after the prompt
number, before any other content:

  Executing for Platform: <Brand>
  Executed through Platform: <Brand>

"Executing for Platform" is what the work is FOR — the brand or product
that the work serves.

"Executed through Platform" is what the work runs THROUGH — the repo
or infrastructure where the changes are committed and deployed.

Multi-platform "for" uses an indented list. Usually both lines name the
same brand. They differ when CDN, OGA, or cross-cutting work affects
many platforms but executes through one. The header forces explicit
scope before drafting.

## THE PLATFORMS — EXACT NAMES, EXACT CASING, NO EXCEPTIONS

    businessblueprint.io    — business growth platform — priority
    hostsblue.com           — domains, hosting, email, website builder
    swipesblue.com          — payment processing
    scansblue.com           — website auditing and scanning
    Console.Blue            — internal operations interface
    BUILDERBLUE2.COM        — AI-powered vibe coding platform. Standalone and integrated with hostsblue.com.
    LINKBlue.systems        — monitors all website health
    TRIADBLUE.COM           — parent company — ALWAYS ALL CAPS

These are the only acceptable formats. Do not alter casing, spacing, or punctuation.

## BUSINESSBLUEPRINT — APP AND SUITE STRUCTURE

/ compass suite — $99/mo
  / promote #1844A6 | / engage #660099 | / respond #001882 | / post #FF44CC

/ anchor suite — $99/mo
  / elevate #E9B307 | / optimize #374151 | / publish #064A6C | / amplify #97ACCA

/ connect — standalone only: FREE (100 contacts) or $29/mo unlimited
/ convert — Lead Capture and Conversion Tool: FREE (with / convert branding) or $59/year Premium (branding removed + full customization, conditional logic, multi-step, advanced field types)
/ Coach Blue — $99/mo standalone | $59/mo with one suite | FREE with both suites
/ assess — free Digital IQ Assessment tool
/ scan — website scanner

Each app — $29/mo standalone

Suites never cross-pollinate. Never bundle / connect. Never bundle / convert. Never bundle / Coach Blue.

## SUITE AND APP NAME FORMAT — LOCKED

The "/" is always present. The space after "/" is always present.
The "/" renders in Triad Black #09080E.
The name after the "/" renders in the app's own accent color.
Font: Archivo Semi Expanded.

  / compass suite     — the Compass Suite
  / anchor suite      — the Anchor Suite
  / Coach Blue        — the AI business coach
  / connect           — the CRM
  / convert           — lead capture and conversion tool
  / promote           — email campaigns
  / engage            — live chat widget
  / respond           — unified inbox
  / post              — social media manager
  / publish           — business listings manager
  / elevate           — reputation and reviews manager
  / optimize          — SEO health monitor
  / amplify           — advertising platform
  / assess            — Digital IQ Assessment tool
  / scan              — website scanner

These are the ONLY acceptable names. No old names ever:
  Never: CommVerse, Commverse, LocalBlue, Localblue, AI Coach, AICoach
  Never: /send, /chat, /livechat, /inbox, /content, /listings, /reputation, /relationships

## PAYMENT — NON-NEGOTIABLE

ALL payment processing goes through swipesblue.com only.
SwipesBlue API: https://swipesblue.com/api/v1
The words "Stripe" and "NMI" must never appear in businessblueprint.io codebase.
What swipesblue.com uses internally is swipesblue.com's private business.
businessblueprint.io never knows and never references any processor.

## BRAND RULES — NON-NEGOTIABLE

Triad Black: #09080E
App name format: / (Triad Black #09080E) + space + appname (app's own accent color)
Font: Archivo Semi Expanded

App accent colors — confirmed from official lockup files:
  / promote  #1844A6
  / respond  #001882
  / engage   #660099
  / post     #FF44CC
  / publish  #064A6C
  / elevate  #E9B307
  / optimize #374151
  / amplify  #97ACCA
  / connect  #008060
  / convert  #8000FF
  / Coach Blue #0000FF
  / compass suite #F97316
  / anchor suite  #97ACCA
  / assess   #960D71
  / scan     #E00420

Button pattern on every landing page — in this exact order:
  Button 1: #FF6B00 orange, white text — "Add to Cart — $X/mo"
  Button 2: app accent color background, WHITE text always
    EXCEPTION: / elevate button 2 uses Triad Black #09080E text
    because #E9B307 yellow fails contrast with white
  Button 3: outline, app accent color border and text — "View All Pricing"

Dark background rule: WHITE TEXT ONLY on any dark section. No app colors. No exceptions.

Subtitle below app name in hero: app's own color, small spaced caps.

/ Coach Blue icon: always use face PNG (coachblue.png) — never a Lucide icon.
All other apps: Lucide icons in rounded square with app accent color background.

LUCIDE ICON EXCLUSIVITY (ECOSYSTEM-WIDE)
Each Lucide icon assigned to an app in app-registry.ts is exclusive to
that app. The same icon may not be used anywhere else on the same site
(navigation, resource columns, footer, body content, decoration) and may
not be used by any app or feature on any other ecosystem site (hostsblue,
swipesblue, scansblue, builderblue2, triadblue, tbsys). Violations must
be surfaced to Dean for resolution — do not auto-rename. Coach Blue is
the established exception: face PNG (coachblue.png), never a Lucide icon.

No "Coming Soon" anywhere.
No placeholder content.
No loyalty program references.
No old suite names ever.
No Stripe or NMI references in businessblueprint.io.

## FILENAME NOMENCLATURE — ASSETS AND CDN

Filenames in /Users/Shared/global assets/logo images and texts/<brand>/
on Dean's Mac are authoritative. Do NOT rename, abbreviate, hyphenate,
or "normalize" them when copying to the CDN, importing into a repo, or
referencing them in code. Replit auto-renames (trailing numeric suffixes
from drag-drop uploads) must be reverted before commit. CDN slot names
should match Dean's descriptive naming, not design-industry shorthand.

Canonical CDN naming convention (locked 2026-04-27):
  logo-image.png                          — icon only
  logo-image-and-logo-text-as-url.png     — lockup (icon + URL wordmark)
  logo-text-as-url.png                    — wordmark only
  ecosystem-lockup.png                    — TRIADBLUE-only multi-brand composite

Example: use "logo-image-and-logo-text-as-url.png" not "logo-lockup.png".

CDN server: cdn.triadblue.com (147.185.239.66, Kamatera).
Brand folders: builderblue2, businessblueprint, coachblue, hostsblue,
scansblue, swipesblue, tbsys, triadblue.

Use scp not rsync for CDN pushes. scp updates file mtime to upload time
on the destination, which keeps Last-Modified headers accurate for
verification gates. rsync preserves source mtime and breaks them.

## SINGLE SOURCES OF TRUTH

  app-registry.ts  — all pricing, colors, app configuration
  menu-config.ts   — all navigation structure
  AppName component — renders app icon + / + appname + subtitle

## AUDIENCE — APPLY TO ALL COPY

Gen X and SMB owners who built real businesses without technology.
They know their craft. They don't know why they're invisible online.
Write like a trusted advisor. Plain language. No jargon. No assumed digital knowledge.
Never use: "powerful", "robust", "seamless", "revolutionary", "innovative"
Explain the WHY behind every feature — not just what it does.
Every page must make the reader think: "that's exactly my problem."

## COPY STANDARD — EVERY LANDING PAGE

  1. Hero headline speaks to the business owner's real problem
  2. Body copy explains WHY each feature matters — not just what it does
  3. At least one "WHAT THIS MEANS FOR YOUR BUSINESS" callout box
     in the app's accent color with a specific, honest statement
  4. Reads like a trusted advisor — not a product spec sheet
  5. No feature described without explaining its business impact

## ARCHITECTURE — ALREADY DECIDED, DO NOT CHANGE

  All payment: swipesblue.com API only
  / connect is the data hub all apps flow through
  Suites never cross-pollinate
  / Coach Blue is purchasable AND persistent for all clients
  Reddit is a priority platform in / amplify — not Phase 2
  The Expand tier uses containerized VPS — never say "dedicated"
  hostsblue.com tiers: Begin $15 | Build $29 | Scale $99 | Expand $320

## SUB-AGENT RULES

If you are a sub-agent receiving a task:
  - You have read this file. That is mandatory before any work begins.
  - Do not make product, architecture, or business decisions.
    Dean decides. You execute.
  - Do not guess at brand colors, prices, or app names.
    Read app-registry.ts before writing anything.
  - Do not delegate work to another agent without ensuring they read this file.
  - If you cannot confirm you have read this file, do the work yourself.

These rules apply regardless of which document type you receive — a
prompt, a response, or a segue. Whether you are starting a fresh task,
joining a running session mid-flight, or picking up a session another
agent ended, you have read CLAUDE.MD before you act. The document type
does not change the obligation.

## VERIFICATION REQUIREMENT — EVERY TASK

Before reporting any task complete:
  1. Read the actual file content after your changes
  2. Confirm each specific instruction from the prompt was executed
  3. Show the changed lines as proof — not a summary, not a table
  4. If anything was not done, say so explicitly and fix it now

Claiming completion without verification is not acceptable.
A table of checkmarks is not verification. Actual file content is verification.

## DO NOT TOUCH WITHOUT EXPLICIT INSTRUCTION

  Payment system
  Authentication system
  Admin panel
  Database schema
  ScansBlue assessment flow
  Any server-side code not explicitly listed in the prompt
  / Coach Blue face PNG icons
  Any component structure or layout not explicitly listed in the prompt

