# Smart Study Planner Web App

We will build a modern, responsive Smart Study Planner web application using React and Vite. The application will allow users to input subjects and an exam date, and it will generate a study plan checklist with progress tracking, persisting data via `localStorage`.

## User Review Required

> [!IMPORTANT]
> Please review the chosen tech stack and the task generation logic. I am proposing **React + Vite** for a modern component-based architecture and fast development.

> [!NOTE]
> For task generation, the plan will create a checklist of tasks evenly distributed for each entered subject leading up to the exam. If you prefer a generic to-do list per subject instead of day-by-day task generation, let me know!

## Proposed Changes

### Vite Project Setup
Create a new Vite React project at `C:\Users\tanve\.gemini\antigravity\scratch\smart-study-planner`.

#### [NEW] `package.json` & Configuration
Standard Vite + React dependencies.

---

### Core Components

#### [MODIFY] `src/App.jsx`
Main layout, local storage synchronization, motivation quote display, and component composition.

#### [NEW] `src/components/PlannerForm.jsx`
Input fields for dynamically adding/removing subjects, selecting the exam date, and a "Generate Plan" button.

#### [NEW] `src/components/TaskList.jsx`
Displays the generated tasks in a clean card layout with checkboxes, styled for a checklist aesthetic.

#### [NEW] `src/components/ProgressBar.jsx`
Visual progress indicator based on completed vs. total tasks.

---

### Styling

#### [MODIFY] `src/index.css` & `src/App.css`
- Apply clean, minimal design principles.
- Use a light theme with soft blue/purple accents.
- Modern typography (e.g., Google Fonts 'Inter').
- Responsive design tailored for mobile accessibility.
- Card layouts, subtle shadows, and neat micro-animations for interactions.

## Open Questions

> [!TIP]
> 1. Should the generated task for a subject be generic (e.g., "Study [Subject] on [Date]") or do you want specific types of tasks per subject (e.g., "Read Chapter for [Subject]", "Practice Problems for [Subject]")?
> 2. Is there a specific motivational quote you'd like to use as the default, or should I select a few to cycle through?

## Verification Plan

### Automated/Dev Tests
- Run `npm run dev` to serve the application locally.
- Use the built-in browser tool to verify UI styling, responsiveness, and state management (tasks persisting on refresh).

### Manual Verification
- The user can run the server and verify the layout, soft color scheme, mobile responsiveness, and interactive feel on their machine.
