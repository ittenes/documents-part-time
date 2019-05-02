# WebDev Jury Guidelines

## Setup

- You will have 10 minutes with each student so he/she can present the project and you can ask questions and give feedback
- After all the students have presented, each member of the jury will vote the best 3 projects
- The jury as a whole must agree and generate consensus around the top 3 projects, selected to present in the Hackshow
- Some criteria or fundamentation on why to choose each project has to be debated
- One member of the jury will announce one project and explain to the students why it has been chosen — and rotate, according to preference


## Expected deliverables

- Frontend application deployed to heroku
  - Responsive UI (mobile-first)
  - Authentication flows (login/signup with local credentials and/or social login)
  - Dynamic components in application header (authentication status)
  - Authorization of routes depending on authentication state and/or user roles
  - Complete user journey on the core features of the app
- Backend REST API deployed to heroku
  - Appropriate HTTP verbs and paths describing the resources
  - Consistent responses
  - Resilient to errors
  - Validations
- User stories updated according to the project status
- Simple wireframes and description of the user journey
- Project slide deck including challenges, lessons learned and highlights

## To review

Note:

The following items are are just examples of questions to students, for them to demo and/or show the code, or simply describe what they have done (or not done).

The available time should allow for short conversations on 1/2 of the following topics.

### User experience
- Are the main application features easy to reach via the navigation elements?
- Are the forms easy to use and do they have clear validation messages?
- Are the features completed (as opposed to some of the features don’t quite work because they are not ready yet)?
- Is the design consistent between pages/components?

### Frontend
- Does the URL path reflect the state of the application?
- Does the application automatically navigate the user after the user actions, according to the user journey?
- Are the pages composed of small, single responsibility, components?
- Can the student identify how the frontend is integrated with external libraries and APIs (e.g. bootstrap, materialize, Google Places lookups, etc…)
- Is the console clean, displaying no errors other than REST 4xx responses?
- Is the markup consistent and semantic, using CSS classes/ids?
- Is the CSS code simple, using short selectors and avoiding anti-patterns such as !important?
- Is the source code consistently formatted and annotated?

### Backend
- Can the student explain the data model and the relationships?
- Can the student describe the project’s rest API, including resources and verbs?
- Can the student identify the building blocks of the rest API (e.g. database connection, models, routes, session setup, CORS setup, error handling, logging, …)?
- Can the student explain how the backend is integrated with external APIs (e.g. Google OAuth flow, Spotify API backend calls, etc…)
- Is the source code consistently formatted and annotated?

### Presentation
- How well does the student explain the process and solution?
- Does the student refer to the application flows and features in a structured manner (e.g., using User Stories)?
- Does he/she demonstrate a clear understanding of underlying technologies  in a professional manner (SPA, Sessions and cookies, HTTP, API Integrations)?
- Is the student comfortable showing and explaining code samples (using Github or the IDE)?
