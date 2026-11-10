# Appendix A: AI Log

## Declaration of AI use
I used Google Gemini to generate a rough template diagram for mapping my website features (see [feature-research.md](./feature-research.md)). I then refined it, gave Gemini changes and direction, and dismissed some of its suggestions. I also used Copilot in VS Code to draft wireframes from my sketches and project research. The separate records below describe each interaction, what I accepted or rejected, and the changes I directed. I reviewed the AI outputs rather than treating them as authoritative.

The wireframe draft is saved in [wireframes.md](./wireframes.md).

## How I used the AI
- **Tool:** Google Gemini
- **Date generated:** 9 November 2026
- **Evidence saved:** 9 screenshots of my prompts and Gemini's responses, taken on 9 November 2026
- **Purpose:** To produce a rough template diagram showing how Lydia's feedback and my competitor research lead to the website's features.
- **My role:** I decided the process and features, directed each change, and checked every output against Lydia's needs and my research.

## Interaction log
| # | What I asked or directed | What Gemini produced | My decision | Evidence |
|---|---|---|---|---|
| 1 | Asked for a wireframe or similar diagram that would show nicely in Markdown, based on my own process diagram | A Mermaid diagram and a text outline | Rejected. It did not work for me | [Screenshot 1](./Ai-screenshots/gemini-01-initial-mermaid-outline.png) |
| 2 | Told Gemini the output "doesn't work at all" | Offered two text-based formats | Chose the ASCII flowchart | [Screenshot 2](./Ai-screenshots/gemini-02-outline-rejected.png) |
| 3 | Followed up on the text-based options | An ASCII box flowchart | Kept it as a base | [Screenshot 3](./Ai-screenshots/gemini-03-ascii-flowchart.png) |
| 4 | Asked for Markdown or Mermaid code so it would display nicely | A Mermaid snippet with styling | Did not use it. I kept the ASCII version | [Screenshot 4](./Ai-screenshots/gemini-04-mermaid-snippet.png) |
| 5 | Directed changes: FAQs on their own, Homepage and About combined, the review carousel as its own feature, and "Services & Pricing" instead of area information | Applied my changes (see next row) | My own direction | [Screenshot 5](./Ai-screenshots/gemini-05-refinement-feedback.png) |
| 6 | Reviewed the updated version | An updated ASCII flowchart with my changes applied | Accepted the changes, then asked for fewer steps | [Screenshot 6](./Ai-screenshots/gemini-06-updated-ascii.png) |
| 7 | Said there were too many steps and set the flow: competitor research and Lydia's feedback, then user stories, then features | A condensed diagram | Accepted | [Screenshot 7](./Ai-screenshots/gemini-07-fewer-steps.png) |
| 8 | Reviewed the condensed version | A streamlined diagram with 6 feature boxes | Accepted as my template | [Screenshot 8](./Ai-screenshots/gemini-08-streamlined-diagram.png) |
| 9 | Asked for an Instagram API feature and the research it might need | Added an "Instagram API & Feed Research" box | Accepted. I will do the research myself | [Screenshot 9](./Ai-screenshots/gemini-09-instagram-api-box.png) |

## Suggestions I dismissed
- The Mermaid diagram and outline format, because it did not display well for my needs.
- The first layout, because it grouped FAQs with About, kept Homepage and About separate, did not show reviews as a feature, and mixed services with area information.
- The long process (compare findings, requirements mapping, link feedback to requirements), because it had too many steps. I replaced it with a shorter flow through user stories.

## My work and the AI's work
- **AI-generated:** the rough diagram layout and formatting.
- **My own work:** the process I mapped, the feature decisions, all the corrections above, and the research and conclusions in [feature-research.md](./feature-research.md). The AI output was a template only. I checked it and changed it before using it.

## Reference
Google Gemini (2026) *Response to a prompt about mapping website features from user stories* [Gemini]. Conversation URL unavailable; no public link was retained. [Accessed 9 November 2026].

## Copilot in VS Code: wireframe interaction
- **Tool:** Copilot in VS Code
- **Date:** 9 November 2026
- **Purpose:** Turn my mobile hand sketches, client feedback and feature research into a first-draft set of website wireframes.
- **My role:** I checked the plan and wireframes against my sketches and requirements, pointed out omissions, directed corrections, and reviewed the revised draft. I am keeping the AI's work honest by recording both the initial mistakes and my decisions, rather than presenting the output as if it were correct first time.
- **Evidence saved:** 16 screenshots of the prompts and responses from this interaction, taken on 9 November 2026.

| # | What I asked or directed | What Copilot produced | My decision | Evidence |
|---|---|---|---|---|
| 1 | Asked for a wireframe plan based on my rough hand notes, with room to clarify details after seeing a first draft | Summarised my notes and existing project information as a mobile-first page plan | Used the summary as a starting point for asking to see text drafts; the page ideas and structure came from my sketches and project work | [Screenshot 1](./Ai-screenshots/copilot-01-wireframe-plan.png) |
| 2 | Asked to see my wireframe ideas in chat so I could make changes | Presented my page structures as text wireframes for the shared header, Home, Services & Prices, Gallery, Reviews, FAQ, Enquiry / Contact and footer | Reviewed the presentation and specified layout refinements in the next prompt | [Screenshot 2](./Ai-screenshots/copilot-02-initial-wireframes.png), [Screenshot 3](./Ai-screenshots/copilot-03-initial-home-and-navigation.png), [Screenshot 4](./Ai-screenshots/copilot-04-initial-services.png), [Screenshot 5](./Ai-screenshots/copilot-05-initial-gallery.png), [Screenshot 6](./Ai-screenshots/copilot-06-initial-reviews.png), [Screenshot 7](./Ai-screenshots/copilot-07-initial-faq.png), [Screenshot 8](./Ai-screenshots/copilot-08-initial-enquiry.png), [Screenshot 9](./Ai-screenshots/copilot-09-initial-footer.png) |
| 3 | Asked for Lydia's photo to sit left of the About text, the About content and review carousel to be centered in their containers, full shared headers and footers instead of placeholders, a 3-by-3 review-card layout with a Load more control, and "All rights reserved" in the footer | Revised the wireframes to show these changes | Approved the revised draft and asked for it to be added to `wireframes.md` with the screenshots. I asked for no commit so I could review the changes first | [Screenshot 10](./Ai-screenshots/copilot-10-layout-change-request.png), [Screenshot 11](./Ai-screenshots/copilot-11-revised-home.png), [Screenshot 12](./Ai-screenshots/copilot-12-revised-services.png), [Screenshot 13](./Ai-screenshots/copilot-13-revised-gallery.png), [Screenshot 14](./Ai-screenshots/copilot-14-revised-reviews.png), [Screenshot 15](./Ai-screenshots/copilot-15-revised-faq.png), [Screenshot 16](./Ai-screenshots/copilot-16-revised-enquiry.png) |
| 4 | Pointed out that the new AI log did not follow the existing record closely enough and needed to distinguish what I requested, what the AI missed, and what I rejected or corrected | Updated this section to use the same interaction-log, decisions, and authorship structure, and to record mistakes separately from rejected suggestions | Requested a clear record that I checked and corrected the AI output. No screenshot was supplied for this follow-up | Not captured in the supplied screenshots |
| 5 | Clarified that the 3-by-3 Reviews grid and footer wording were design changes requested after seeing the first draft, not necessarily ignored instructions; also noted the carousel pause control and mismatch between the wireframe and US03 | Reworded the log to distinguish design revisions from later design choices, and added pause controls to the displayed carousels | Asked for the record to accurately reflect the order of decisions. No screenshot was supplied for this follow-up | Not captured in the supplied screenshots |
| 6 | Clarified that the page structures were based on my sketches and ideas, so they should not be described as AI-generated | Corrected the authorship description to credit my work for the structures and the AI only for presenting them as text wireframes | Confirmed that the project structure and content ideas are mine; AI assistance was in formatting and drafting their text representation. No screenshot was supplied for this follow-up | Not captured in the supplied screenshots |
| 7 | Clarified that the hand sketches are basic original framework, while the updated prompted wireframes represent the refined direction; specified that the review carousel belongs on every page except Reviews, and explained that review details are placeholders, About placement needs Lydia's confirmation, and success/error prompts do not need separate wireframes | Updated the Enquiry wireframe with the carousel and pause control, and clarified the open About-page decision and enquiry-form behavior | Confirmed the review-carousel placement. Review names, text and star ratings in the wireframes are placeholders. The About-page arrangement awaits Lydia's confirmation. No screenshot was supplied for this follow-up | Not captured in the supplied screenshots |
| 8 | Explained that the FormSubmit automatic acknowledgement is handled by the service, simple success/error prompts will be implemented without separate wireframes, and proofreading can be completed later because the noted issues are minor wording/spelling points | Recorded these as implementation and later proofreading work rather than missing wireframe requirements or substantive design issues | No separate wireframe state is needed for these prompts. Proofreading is deferred until later review. No screenshot was supplied for this follow-up | Not captured in the supplied screenshots |

## Design revisions I requested after reviewing the first draft
- I asked for pages to show the full shared header and footer instead of "Shared header" and "Shared footer" placeholders.
- I asked for Lydia's photo to sit left of the About text, with the content centered in its container.
- After seeing the first Reviews draft as a list, I requested a design change to a three-by-three card grid with a Load more control. This was a revision I asked for after reviewing the draft, not an instruction Copilot had previously missed.
- I asked for "All rights reserved" to be added to the footer. This was also a later design change.
- I later pointed out that the wireframe carousels needed pause controls to match the existing acceptance criteria, and added them to the draft.

## Clarifications and remaining design decisions
- The hand sketches are the basic starting point; the updated prompted wireframes express the refined design direction. The review carousel is intended on every page except Reviews, including Enquiry / Contact. The Enquiry screenshot records an earlier draft and does not show this later clarification; the current wireframe reflects the clarified requirement.
- The review cards, names, text and star ratings shown in the wireframes are placeholders, not verified review content or ratings.
- Lydia's feedback records a preference for separate pages. Confirm with her whether the About section may remain on Home; if not, add a separate About page and navigation link.
- A simple form success or error prompt is planned for implementation and does not need its own wireframe. FormSubmit is intended to provide the automatic acknowledgement email; check delivery and privacy suitability before using it for real enquiries.
- The wording and spelling points identified in the review are minor proofreading items that can be addressed later, not substantive design or requirements failures.
- I previously described the Enquiry carousel as a transcription mismatch because it was absent from one draft screenshot. That description did not account for the difference between the basic sketches, the prompt-based updated drafts and the clarified all-pages requirement; the intended current design is now recorded above.

## My work and Copilot's work
- **My own work:** The hand sketches, page structure, content ideas, project research, requirements, and design decisions. These informed the wireframe draft and were not originated by the AI.
- **AI assistance:** Copilot helped express my sketches and directions as text-based wireframe drafts and helped format revisions. I reviewed those drafts and updated the wireframe to reflect my later clarifications before keeping it in [wireframes.md](./wireframes.md).

The wireframes remain a draft for my review, not a final visual design.
