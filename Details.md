 How the Mentor System Fits Into the Platform

  The Short Version                                                                                                                              
  Mentors are just instructors with a different onboarding path. The platform already has instructor roles, permissions, login, invitations,  
  and a marketplace — we're building the front door (application form + admin review). Everything behind that door already exists.

  ---
  Step by Step

  1. Admin shares a course-specific link

  From the course settings in webadmin, the admin generates an invite link for that specific course. Here's exactly how that looks:

  1. Admin creates a course (e.g., "UX Design Bootcamp")
  2. Admin opens that course in the webadmin panel
  3. Admin clicks "Invite Mentor / Instructor"
  4. System generates a link tied to that specific course
  5. Admin sends that link to the mentor candidate

  The link knows which course it belongs to, so when the candidate opens it, the form already shows the course name. No dropdowns, no
  guessing.

  2. Candidate fills out the application

  No account needed. They land on a public form, it shows the course name, they fill in their background and submit. System creates a pending 
  record and pings the admin.

  3. Admin reviews and approves

  In webadmin there's a review queue. Admin opens an application, reads it, clicks Approve or Reject. On approval, the system assigns the     
  instructor role to that person on that specific course and fires off an invitation email.

  4. Mentor sets their password and logs in

  The approval email has a one-time link. They set a password, log in, and land straight in their course. No extra steps.

  5. What they see after logging in

  They're in webadmin, scoped to their course only. They can grade submissions, write teacher notes, and manage the perks marketplace for that
   course. They can't see anything outside their course — enforced by the existing permission system.

  6. Marketplace / 1:1 sessions

  Once approved, a mentor can create a perk listing in their course marketplace — something like "Book a 1:1 session with me." Students spend 
  their earned points to claim it. The perk already has provider and manager email fields built in for exactly this.

  ---
  What Already Exists vs. What We're Building

  ┌────────────────────────────────┬───────────────┐
  │            Feature             │    Status     │
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
  └────────────────────────────────┴───────────────┘

  ---
  Do We Need a Status Page?

  Probably not. A confirmation email covering "we got your application, expect to hear back in X days" handles most of it. The only case for a
   status page is if the review takes weeks and the applicant wants to check without digging through their inbox — that's a team call, not a  
  technical requirement.

  ---
  Why Not Just Google Forms

  The form itself isn't the problem. It's everything after.

  With Google Forms: someone submits → lands in a spreadsheet → admin manually reads it → copies the email → goes into the platform → creates 
  the user → assigns the course → sends an invite. That's 5-6 manual steps every time, with room for typos, wrong course assignments, or the  
  invite never getting sent.

  With this system: admin reads the application, clicks Approve, and everything else happens automatically — account creation, role
  assignment, course access, invite email. The link the admin shared already knows the course, so there's no matching step either.

  Google Forms is fine for collecting data. It's not a workflow tool. This replaces those 6 manual steps with one click.

  ---
  Quick Answers

  ┌─────────────────────────────────────────────────┬─────────────────────────────────────────────────────────────────────┐
  │                    Question                     │                               Answer                                │
  ├─────────────────────────────────────────────────┼─────────────────────────────────────────────────────────────────────┤
  │ Do mentors need a separate portal?              │ No. They log into the existing admin panel, scoped to their course. │
  ├─────────────────────────────────────────────────┼─────────────────────────────────────────────────────────────────────┤
  │ Can a mentor apply to multiple courses?         │ Only if they receive a link for each one.                           │
  ├─────────────────────────────────────────────────┼─────────────────────────────────────────────────────────────────────┤
  │ Who can approve?                                │ Any admin.                                                          │
  ├─────────────────────────────────────────────────┼─────────────────────────────────────────────────────────────────────┤
  │ Can a mentor be removed?                        │ Yes. Admin removes their role. Access is gone immediately.          │
  ├─────────────────────────────────────────────────┼─────────────────────────────────────────────────────────────────────┤
  │ How does the mentor know what they applied for? │ The form shows the course name from the link.                       │
  └─────────────────────────────────────────────────┴─────────────────────────────────────────────────────────────────────┘