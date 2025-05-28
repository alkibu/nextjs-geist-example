# Detailed Plan for "On-the-Way Vehicle Breakdown Repair Management System"

## Information Gathered
- The system consists of three main interfaces:
  1. Driver App Interface
  2. Mechanic App Interface
  3. Admin Dashboard
- The system should be mobile-first, intuitive, and focused on emergency usability.
- Features include:
  - Driver App: Help request form, camera upload, GPS location pinning, problem type selection, live mechanic tracking, payment, and rating.
  - Mechanic App: Real-time job alerts, route navigation, job status updates, repair summary upload.
  - Admin Dashboard: Monitor requests, approve mechanics, manage roles, analytics, dispute handling.
- Use Tailwind CSS for styling with a modern black and white theme.
- Use Google Fonts for typography.
- Use existing UI components from `src/components/ui`.
- Mark client components with "use client" directive where React hooks are used.
- Ensure large buttons, real-time updates, and reliable experience in low-connectivity areas.

## Plan

### File Structure and Components
- `src/app/driver/`
  - `page.tsx` - Main Driver App page with request form and map.
  - `components/`
    - `HelpRequestForm.tsx` - Form for requesting help.
    - `CameraUpload.tsx` - Camera button and photo upload.
    - `LocationPinButton.tsx` - Button to pin GPS location.
    - `ProblemTypeSelect.tsx` - Dropdown/select for problem types.
    - `LiveMechanicMap.tsx` - Map showing mechanic location.
    - `PaymentAndRating.tsx` - Payment options and rating UI.
- `src/app/mechanic/`
  - `page.tsx` - Main Mechanic App page with job alerts and navigation.
  - `components/`
    - `JobAlerts.tsx` - Real-time job alerts with images and location.
    - `RouteNavigation.tsx` - Navigation to breakdown site.
    - `JobStatusUpdate.tsx` - Update job status stages.
    - `RepairSummaryUpload.tsx` - Upload repair/service report.
- `src/app/admin/`
  - `page.tsx` - Admin Dashboard main page.
  - `components/`
    - `RequestMonitor.tsx` - Monitor breakdown requests and progress.
    - `MechanicApproval.tsx` - Approve mechanics and manage roles.
    - `Analytics.tsx` - Service analytics and history.
    - `DisputeHandler.tsx` - Handle disputes and feedback.

### Styling and UX
- Use Tailwind CSS utility classes for layout and styling.
- Use Google Fonts imported in the head for modern typography.
- Large buttons and clear UI elements for emergency usability.
- Responsive design for mobile-first experience.
- Use React hooks for state management and real-time updates.
- Use existing UI components from `src/components/ui` for consistency.

## Dependent Files to be Edited
- New files under `src/app/driver/`, `src/app/mechanic/`, and `src/app/admin/`.
- Possibly update `next.config.ts` if needed for external APIs or images.
- Use existing UI components from `src/components/ui`.

## Follow-up Steps
- Implement the components and pages as per the plan.
- Test responsiveness and usability on mobile devices.
- Implement real-time updates and map integration.
- Add payment integration and service rating.
- Verify offline/low-connectivity behavior.
- Run and test the full system locally.

---

Please confirm if you approve this detailed plan so I can proceed with implementation.
