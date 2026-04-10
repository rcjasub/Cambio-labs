 ---
  What I'm Building

  I'm adding a mentor layer to the existing journey platform. The goal is to let qualified
   people apply to become mentors, have our team review and approve them, and then have   
  approved mentors show up inside the platform where students can find them.

  This is broken into three connected pieces:

  1. Mentor apply flow — a person visits the platform, creates a mentor account, fills out
   their profile (bio, expertise areas, hourly rate, photo), and submits it for review.   
  They then see a status page telling them where their application stands.
  2. Admin approval dashboard — our internal team gets a new section in the admin panel   
  showing all pending applications. They can open each one, review the full profile, and  
  either approve it, reject it, or ask for changes. If changes are requested, the mentor  
  gets notified and can update and resubmit.
  3. Mentor directory — once an admin approves a mentor, that mentor's card automatically 
  appears in a new Mentors section inside the student platform. No extra steps needed.    
  Students can browse approved mentors from within the same app they already use.

  ---
  Why I'm Not Building a Separate App

  I looked at two options — build this as its own standalone website, or extend the       
  platform I already have.

  I'm extending the existing platform. The reason is simple: login, user accounts, file   
  uploads for photos, email notifications, and the admin panel all already exist. If I    
  started from scratch, I'd spend the first week just rebuilding those things before      
  writing a single line of mentor-specific code. By working inside the existing platform, 
  I can spend all three weeks on the actual features.

  ---
  Who Sees What

  A mentor is not a student. These are separate roles with completely different
  experiences.

  ┌───────────────┬───────────────────────────────────────────────────────────────────┐   
  │    Person     │                       What they can access                        │   
  ├───────────────┼───────────────────────────────────────────────────────────────────┤   
  │ Student       │ Their courses, lessons, progress — plus a new Mentors section to  │   
  │               │ browse approved mentors                                           │   
  ├───────────────┼───────────────────────────────────────────────────────────────────┤   
  │ Mentor        │ The apply form and a status page showing where their application  │   
  │ applicant     │ stands — nothing else                                             │   
  ├───────────────┼───────────────────────────────────────────────────────────────────┤   
  │ Approved      │ Their public profile visible to students in the directory         │   
  │ mentor        │                                                                   │   
  ├───────────────┼───────────────────────────────────────────────────────────────────┤   
  │ Admin         │ Everything in the admin panel, plus the new mentor review queue   │   
  └───────────────┴───────────────────────────────────────────────────────────────────┘   

  When a mentor logs in, they go straight to their status page. They do not see courses,  
  lessons, or any student content. The two experiences are fully separate.

  ---
  How the Mentor Application Works Step by Step

  Mentor creates an account
          ↓
  Fills out their profile
    (bio, areas of expertise, hourly rate, profile photo)
          ↓
  Submits application
          ↓
  Sees a status page: Pending
          ↓
  Admin reviews the application
          ↓
  Admin approves → mentor appears in student directory immediately
  Admin rejects → mentor is notified with a reason
  Admin requests changes → mentor updates and resubmits

  ---
  How Admin Review Works

  Admins see a queue of all applications organized by status — Pending, Under Review,     
  Approved, Rejected. They can filter by status, open any application to see the full     
  profile, and take one of three actions:

  - Approve — mentor goes live in the student directory instantly
  - Reject — mentor is notified with a reason
  - Request Changes — mentor receives a message, updates their profile, and resubmits     

  Every action is logged with who did it and when.

  ---
  Timeline

  ┌───────────┬──────────────────────────────────┬────────────────────────────────────┐   
  │   Dates   │       What I'm working on        │        What becomes visible        │   
  ├───────────┼──────────────────────────────────┼────────────────────────────────────┤   
  │ Apr 3–9   │ Setting up the database and      │ Nothing visible yet                │   
  │           │ technical foundation             │                                    │   
  ├───────────┼──────────────────────────────────┼────────────────────────────────────┤   
  │ Apr 10–16 │ Building the mentor sign-up,     │ Mentors can apply and check their  │   
  │           │ profile form, and status page    │ status                             │   
  ├───────────┼──────────────────────────────────┼────────────────────────────────────┤   
  │           │ Building the admin review queue  │ Admins can approve/reject;         │   
  │ Apr 17–23 │ and student mentor directory     │ approved mentors appear to         │   
  │           │                                  │ students                           │   
  ├───────────┼──────────────────────────────────┼────────────────────────────────────┤   
  │ Apr 24 –  │ Bug fixes, testing,              │ Full end-to-end demo ready         │   
  │ May 11    │ documentation, and demo prep     │                                    │   
  └───────────┴──────────────────────────────────┴────────────────────────────────────┘   

  ---
  What This Prototype Covers

  The full loop works end-to-end: a mentor applies, an admin approves them, and they      
  appear in the platform where students can find them.

  What's not included in this version:
  - Booking or scheduling sessions with a mentor
  - Payments or rate processing
  - Advanced search or filtering of mentors

  These are production-level features. The final feasibility document (due May 11) will   
  outline exactly what it would take to add them and what it would cost in time and       
  infrastructure.