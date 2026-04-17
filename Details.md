How the Mentor System Fits Into the Platform
                                                                                                                                                                                                                                                                                     
  ---
  The Short Version                                                                                                                                                                                                                                                                               
  Mentors are just instructors with a different onboarding path. The platform already has instructor roles, permissions, login, invitations, and a marketplace — we're building the front door (application form + admin review). Everything behind that door already exists.                  
  
  ---
  Step by Step

  1. Admin shares a course-specific link
  From the course settings in webadmin, admin generates an invite link for that course. They send it to whoever they want to recruit. The link knows which course it belongs to.

  2. Candidate fills out the application
  No account needed. They land on a public form, it shows the course name, they fill in their background and submit. System creates a pending record and pings the admin.

  3. Admin reviews and approves
  In webadmin there's a review queue. Admin opens an application, reads it, clicks Approve or Reject. On approval, the system assigns the instructor role to that person on that specific course and fires off an invitation email.

  4. Mentor sets their password and logs in
  The approval email has a one-time link. They set a password, log in, and land straight in their course. No extra steps.

  5. What they see after logging in
  They're in webadmin, scoped to their course only. They can grade submissions, write teacher notes, manage the perks marketplace for that course. They can't see anything outside their course — that's enforced by the existing CASL permission system.

  6. Marketplace / 1:1 sessions
  Once approved, a mentor can create a perk listing in their course marketplace — something like "Book a 1:1 session with me." The perk already has provider and manager email fields built in for exactly this. Students spend their earned points to claim it.

  ---
  What Already Exists vs. What We're Building

  ┌────────────────────────────────┬───────────────┐
  │                                │               │
  ├────────────────────────────────┼───────────────┤
  │ Auth, roles, permissions       │ Already there │
  ├────────────────────────────────┼───────────────┤
  │ Invitation emails + login flow │ Already there │
  ├────────────────────────────────┼───────────────┤
  │ Admin user management          │ Already there │
  ├────────────────────────────────┼───────────────┤
  │ Perks marketplace              │ Already there │
  ├────────────────────────────────┼───────────────┤
  │ Public application form        │ Building this │
  ├────────────────────────────────┼───────────────┤
  │ Admin review queue             │ Building this │
  ├────────────────────────────────┼───────────────┤
  │ Applicant status page          │ Building this │
  └────────────────────────────────┴───────────────┘

  The three screens in the screenshots are the only new pieces. They wire into infrastructure that's already running.

  ---
  Quick Answers to the Obvious Questions

  Do mentors need a separate portal? No. They log into webadmin like any instructor, scoped to their course.

  Can a mentor apply to multiple courses? Only if they receive a link for each one. Each link is course-specific.

  Who can approve? Any admin. Could be scoped to org-level admins down the line.

  Can a mentor be removed? Yes. Admin pulls their role from the course in user management. Access is gone immediately.

  How does the mentor know what they applied for? The form shows the course name from the link, and the status page confirms it.

  Why not just Google Forms
  
  With Google Forms, someone submits → it lands in a spreadsheet → an admin manually reads it → copies the email address → goes into the      
  platform → creates the user → assigns the course → sends an invite email. That's 5-6 manual steps every single time, with room for typos,   
  wrong course assignments, or the email just never getting sent.

  With this system, the admin reads the application and clicks Approve. Everything else happens automatically — account creation, role        
  assignment, course access, invite email. The link the admin shared already knows the course, so there's no matching step either.