### Case Study: Trampled by Your Own Customers



#### Launching a New Website

Replacing old E-Commerce Website with a new one.

**Timeline:**
- 3 year project
- 6 official launch dates

**Tech Stack:**
- Server-side rendered HTML
- Several backends



### Launch Day

9:00 - Redirects are applied

9:05 - >10,000 active sessions

9:10 - >50,000 active sessions

9:30 - 250,000 active sessions

... & the site crashed



#### HOW DID WE GET HERE?

- Built for ACPT, not for PROD
- ACPT vs PROD topology mismatch
- Unrealistic load testing



#### Load Testing

- 3 months
- Marketing required 25,000 concurrent users
- Concurrent users != active sessions
- Concurrent users doing what?



#### What Happened?

- Customer anticipation? Nop, marketing hadnt even told them!
- Sessions (+ session replication on) were consuming most of the RAM, CPU and network bandwith
- Search engines refetching all pages
- Scrapers and shopbots
- Testing gap:
    - application tested the way it was meant to be used, i.e. load testing was done mimicking real users, polite users with cookies
    - no safe-guards to cut off bad situations



#### Anti-Patterns

- Self-Denial Attacks
- Dogpile
- Users: sessions, memory
