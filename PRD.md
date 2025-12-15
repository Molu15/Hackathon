Here is the refined PRD/Prompt. I have updated the Objective and Design Requirements to explicitly include the "Unique Theme" (tri-state toggle) milestone while keeping your strict technical constraints.

The Prompt for AntiGravity
Role: Senior Front-End Engineer & Jekyll Specialist Context: I am creating a personal portfolio site using the "Academic Pages" Jekyll theme (hosted on GitHub Pages). I have uploaded my CV (A4 - 1.pdf) as the source of truth for the content.

Objective: Analyze the uploaded CV to generate site content (Markdown/Config) AND implement a custom "CV Theme" feature that users can toggle alongside the standard Dark/Light modes.

Technical Constraints (Strict):

I am working on a Jekyll site (Academic Pages template).

Do not introduce new frameworks or JavaScript libraries.

Modify only existing layouts, includes, Markdown, CSS, or vanilla JavaScript to ensure the build remains stable on GitHub Pages.

Milestone 1: Content Extraction & Structure


Profile: Extract my contact details, bio, and photo reference from the "PERSÖNLICHE DATEN" and "MEIN PROFIL"  sections.



Education: Map the "AUSBILDUNG" section to the Education page, noting specifics like "Masterstudent" and "Semester Abroad".




Experience: Map the "BERUFSERFAHRUNG" section  to the Experience/CV page. Include roles like "Werkstudent - HMI ADAS/AD" and "Pflichtpraktikum - UX Consulting".




Skills: Map "KOMPETENZEN" (Figma, Adobe Suite, Unity, Java, etc.)  to a Skills section.





Translation: Translate all German content (e.g., "Werkstudent," "Grundkenntnisse") into professional English.

Milestone 2: "Unique Theme" Feature (Tri-State Toggle)

Requirement: Do not override the default site style globally. Instead, modify the existing Light/Dark mode toggle to function as a 3-way switch: Light Mode → Dark Mode → Vanessa's CV Mode.

CV Mode Design: When "CV Mode" is active, the site should visually mimic my uploaded CV:

Color Palette: Use the specific background and text colors found in the PDF.

Typography: Use a clean, sans-serif font stack that matches the professional look of the CV.

Layout cues: Adjust spacing or borders to reflect the CV’s structured "block" design.

Implementation: Use vanilla JavaScript to handle the toggle logic (cycling through 3 data-theme states) and SCSS/CSS variables to define the visual overrides for the .cv-theme class.

Deliverables: Please provide the code for:

_config.yml (Populated with my user details).

_pages/about.md (Homepage with bio/intro).

_pages/cv.md (Structured timeline of education/experience).

_includes/masthead.html (Or relevant include: Updated HTML for the toggle button).

assets/js/main.min.js (or script block: Updated vanilla JS for the 3-state toggle logic).

assets/css/style.scss (SCSS adding the specific .cv-theme styling variables).