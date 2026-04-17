## How the Mentor System Fits Into the Platform                                                                                                                                                                                                                                                                                                                                                                                                                                       
  ###                                                                                                                                                                                                                    
  
  Mentors apply through a public form that lives inside the platform — no login or
  account needed to access it. Admin approves the application, and the mentor's
  offering automatically gets listed in the course marketplace. The mentor never
  needs an account or access to anything else inside the platform.

  ---

  ### Step by Step

  **1. Admin shares a course-specific link**

  From the course settings in webadmin, the admin generates an invite link for that
  specific course. Here's exactly how that looks:

  1. Admin creates a course 
  2. Admin opens that course in the webadmin panel
  3. Admin clicks "Invite Mentor"
  4. System generates a link tied to that specific course
  5. Admin shares that link — same link can be sent to as many candidates as needed

  The link is course-specific, so every submission through it is automatically tied
  to the right course. No dropdowns, no guessing.

  **2. Candidate fills out the application**

  The link opens a public page inside the platform — no login needed, same way you
  can view any public webpage without an account. The form shows the course name so
  the candidate knows exactly what they're applying for. They fill in their name,
  contact info, and what they're offering, then submit. They get a confirmation email
  that their application was received.

  **3. Admin reviews and approves**

  Submissions land directly in webadmin. Admin opens the review queue, reads the
  application, and clicks Approve or Reject. The mentor gets an email either way.

  **4. Mentor gets added to the marketplace**

  Once admin clicks Approve, the mentor's offering automatically gets listed in the
  course marketplace. Students can see it and spend their earned points to claim it.
  No extra steps from the admin.

  ---

  ### What the Mentor Sees

  Just the form and a confirmation message after submitting. They get one email:

  - One when admin approves or rejects

  They never log in. They never see the course, the students, or anything else inside
  the platform.

  ---

  ### What Already Exists vs. What We're Building

  **Already there:**
  - Auth, roles, permissions
  - Invitation emails + login flow
  - Admin user management
  - Perks marketplace

  **Building this:**
  - Public application form (lives inside the platform, no login required)
  - Admin review queue

  ---

  ### Do We Need a Status Page?

  Probably not. The one emails handle it — one on submission, one on decision.
  (UPDATED)

  ---

  ### Why Not Just Google Forms

  The form itself isn't the problem. It's everything after.

  With Google Forms: someone submits → lands in a spreadsheet → admin manually reads
  it → copies the info → goes into the platform → creates the perk listing manually.
  That's 5-6 steps every time, with room for things to fall through the cracks.

  With this system: admin reads the application directly in webadmin and clicks
  Approve. The marketplace listing gets created automatically. Everything stays inside
  the platform — no switching between tools, no copy-pasting, no missed submissions.

  Google Forms is fine for collecting data. It's not a workflow tool. This keeps
  the entire process inside the platform.

  ---

  ### Quick Answers

  **Does the mentor need an account or login?**
  No. They only ever see the public application form.

  **How do they access the form without logging in?**
  The form is a public page inside the platform — no login needed, same way you
  can visit any public webpage without an account.

  **Can the same link be used for multiple mentors?**
  Yes. Admin generates one link per course and shares it with as many candidates
  as needed. Every submission gets tied to that course automatically.

  **Who approves applications?**
  Any admin, from the review queue in webadmin.

  **What happens after approval?**
  The mentor's offering is automatically added to the course marketplace. No extra
  steps needed.

  **Can a mentor be removed from the marketplace?**
  Yes. Admin removes the listing. Done.

  **How does the mentor know which course they applied for?**
  The form shows the course name pulled from the link they were sent.

  **Is this fully integrated into the platform?**
  Yes. The form lives inside the platform, submissions go straight into webadmin,
  and approval triggers the marketplace listing automatically. No external tools.