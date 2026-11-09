# Hair by Lydia

## Project purpose

- Hair by Lydia is a mobile hairdresser covering Banbury and surrounding villages. The website should build trust and make it easy for visitors to enquire. 
- Local people looking for a mobile hairdresser may want to see prices and reviews because they are paying for a service in a competitive market. This can help them compare options and feel confident in Lydia’s service.
- Lydia wants visitors to see her work, meet her, and find clear ways to enquire, view the gallery, and see services and prices. 
- The site should feel professional and work well on phones, tablets and desktops.

### Initial questionnaire

- I wanted to understand Lydia's goals, existing ideas and practical needs before deciding how my skills could help.
- I asked Lydia about her bussiness,customers, preferred styles, services & prices, and how she would like to manage the site.
- I learnt that Lydia would like a professional site that still reflects her presonality and she focused on making clients feel comfortable.
- Lydia wants to discuss clients needs before confirming an appointment, so I am considering a contact form to help start that conversation. 
- Lydia wants visitors to see her work and learn about her, so I am considering a hero slideshow and an About section to showcase her transformations and personality
- I began exploring colors, style research, and weather an instagram API would work for lydia website gallery which might make updates easier. 

- [Read Lydia’s questionnaire](./evidence/questionaire-hbl.md)

### Research and early ideas

- I sat with Lydia, and she chose three competitors. We went through each website together, and Lydia shared her initial thoughts and feedback on what she liked and disliked
- I evaluated all three websites against six criteria and recorded my findings. I also checked their colour contrast and accessibility using Lighthouse and browser developer tools. These findings, together with Lydia’s feedback, will help inform my design decisions and guide further research into specific features.
- This research helped me decide to include an enquiry form, real client photos and a review carousel, as these matched Lydia's needs and the strengths I found on competitor sites. It also highlighted the importance of accessibility.

- [Read my competitor research](./evidence/competitor-research.md)

Based on Lydia's feedback and my competitor research, I identified some early features and design decisions that need further research. This document shows that research, along with my findings and takeaways.

```text
┌──────────────────────────────┐       ┌──────────────────────────────┐
│  Lydia's questionnaire and   │       │  Competitor website research │
│           feedback           │       │                              │
└──────────────┬───────────────┘       └──────────────┬───────────────┘
               │                                      │
               └──────────────────┬───────────────────┘
                                  ▼
               ┌─────────────────────────────────────┐
               │        Develop User Stories         │
               └──────────────────┬──────────────────┘
                                  ▼
               ┌─────────────────────────────────────┐
               │    Define Initial Website Features   │
               │   (User Stories + Discovery Inputs) │
               └──────────────────┬──────────────────┘
                                  │
  ┌───────────┬───────────┬───────┴───────┬───────────┬───────────┬───────────┐
  ▼           ▼           ▼               ▼           ▼           ▼           ▼
┌─────────┐ ┌─────────┐ ┌─────────┐   ┌─────────┐ ┌─────────┐ ┌─────────┐ ┌─────────┐
│Homepage │ │Services │ │  Photo  │   │ Reviews │ │  FAQs   │ │Contact &│ │Instagram│
│ & About │ │& Pricing│ │ Gallery │   │Carousel │ │ Section │ │ Enquiry │ │   API   │
│Combined │ │         │ │         │   │         │ │(Stand.) │ │         │ │Research │
└─────────┘ └─────────┘ └─────────┘   └─────────┘ └─────────┘ └─────────┘ └─────────┘
```
- [Read my feature research](./evidence/feature-research.md)

### Follow-up feedback

- After reviewing the competitors with Lydia, I asked her a second round of questions to confirm the early ideas I had from the questionnaire and the research. I wanted to check these with her before making design decisions.
- Her answers clarified several things:
  - She prefers separate pages rather than one long page.
  - She wants a hero slideshow of selected work, with "make an enquiry" as the first action visitors are encouraged to take.
  - She would like recent Instagram posts in the gallery if this proves practical, but a gallery updated with photos she provides is also acceptable.
  - The enquiry form should also ask for the client's address, and a phone number should be required.
  - She wants an automatic acknowledgement after an enquiry.
  - She is happy with a review carousel, plus a separate page for all reviews. She has given permission to publish five selected reviews.
  - She would like "from" prices shown, but not service durations, and a note that extra travel costs may apply.
  - She would rather send updates to someone else than update the site herself.
- Her answers also changed my plans. The Instagram API is now an optional feature that needs research, with a gallery I update as the fallback. Her preference not to update the site herself means I should keep updating content simple. Lydia also liked the proposed colour palette, which I will use as my starting point for design.

- [Read Lydia's follow-up feedback](./evidence/lydia-feedback.md)

## User stories

- **US01 – Homepage:** As a new visitor, I want to see Lydia's work and learn about her, so I can decide if her services are right for me.
- **US02 – Enquiry call to action:** As a potential customer, I want an enquiry link on every page, so I can easily get in touch.
- **US03 – Reviews:** As a potential customer, I want to read genuine client reviews, so I can build trust in Lydia's services.
- **US04 – Gallery:** As a potential customer, I want to view examples of Lydia's work, so I can see the quality of her styling and colouring.
- **US05 – Enquiry form:** As a potential customer, I want to ask about services or get advice, so Lydia can understand what I am looking for before confirming an appointment.
- **US06 – Services and prices:** As a visitor, I want to easily find the services and prices, so I can see what Lydia offers and how much it costs.
- **US07 – Cancellation policy:** As a visitor, I want to understand the cancellation terms and deposits, so I know the booking conditions before enquiring.
- **US08 – Training:** As a potential customer, I want to learn about Lydia's training and experience, so I can feel confident in her services.
- **US09 – Social media and contact:** As a visitor, I want to find Lydia's social media and contact links, so I can easily get in touch.

## Design decisions
- **09/11/2026 – Later design decision:** After looking at FormSubmit's privacy policy and endpoint information, I decided to keep the enquiry form simple and only ask for the contact details and information needed for first contact. I will leave out home addresses and photo uploads for now, as I want to limit the amount of personal information being collected through the website. I still need to decide if FormSubmit is suitable before using it for real enquiries.




- How did the client’s needs and research influence your design?
- Explain key choices for layout, colours, navigation and accessibility.
- Link to your wireframes or sketches.

## Features and development

- Describe the features you build and why.
- Explain any important changes or challenges during development.

## Testing

- Summarise how you tested functionality, usability and responsiveness.
- Link to testing.md for procedures, results, bugs and fixes.

## Deployment

- Explain how you deployed the finished site.
- Link to the live website when available.

## Review and future improvements

- What worked well?
- What would you improve?
- Are there any unresolved issues?

## References and supporting evidence
- [Read Lydia’s questionnaire](./evidence/questionaire-hbl.md)
- [Read my competitor research](./evidence/competitor-research.md)
- [Read Lydia's follow-up feedback](./evidence/lydia-feedback.md)
- [Read my feature research](./evidence/feature-research.md)
- [AI log (Appendix A)](./evidence/appendix-a-ai-log.md)