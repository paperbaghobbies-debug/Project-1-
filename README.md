# Hair by Lydia

## Project purpose

- Hair by Lydia is a mobile hairdresser covering Banbury and surrounding villages. The website should build trust and make it easy for visitors to enquire. 
- Local people looking for a mobile hairdresser may want to see prices and reviews because they are paying for a service in a competitive market. This can help them compare options and feel confident in Lydia’s service.
- Lydia wants visitors to see her work, meet her, and find clear ways to enquire, view the gallery, and see services and prices. 
- The site should feel professional and work well on phones, tablets and desktops.

## Design approach

I used Jesse James Garrett’s five planes to help me work out the website, starting with what it needed to do and then moving on to how it would look:

- **Strategy:** Understand what Lydia wants from the website and what potential clients need.
- **Scope:** Use this information to decide which features to include, such as the gallery, reviews and enquiry form.
- **Structure:** Decide how the content should be organised into pages and how visitors will find services, prices and contact details.
- **Skeleton:** Plan the layout and navigation so the important information and enquiry links are easy to find.
- **Surface:** Choose the colours, fonts and images to match Lydia’s brand while making sure the website is easy to read.

I also used ideas from the Agile Manifesto by making changes as I received feedback, rather than sticking to my first ideas. For example, Lydia’s feedback changed some of my plans for the gallery and enquiry form. I recorded these changes and the reasons behind them in my research so I could use them when making the designs and building the website.

- [Navigating the Five Planes of UX: Structure Plane](https://medium.com/design-bootcamp/designing-delight-your-ultimate-guide-to-the-structure-plane-f8c5f273bd9b)
- [Manifesto for Agile Software Development](https://agilemanifesto.org)
- [Code Institute - User Experience Essentials](https://lms.codeinstitute.net/learner_module/show/129021?lesson_id=574949&section_id=2215212)

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

 After reviewing the competitors with Lydia, I asked her a second round of questions to confirm the early ideas I had from the questionnaire and the research. I wanted to check these with her before making design decisions.
 Her answers clarified several things:
  - She prefers separate pages rather than one long page.
  - She wants a hero slideshow of selected work, with "make an enquiry" as the first action visitors are encouraged to take.
  - She would like recent Instagram posts in the gallery if this proves practical, but a gallery updated with photos she provides is also acceptable.
  - Lydia initially asked for the enquiry form to include the client’s address and require a phone number. After considering privacy, I decided not to collect home addresses through the initial form. Lydia confirmed that clients can provide sensitive details later by email, after first contact. 
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

## Acceptance criteria

The following checks are for the user stories documented so far. They are planned checks and will be marked as completed once they have been tested on the built website. 

### US01 – Homepage
- The homepage clearly introduces Lydia and her mobile hairdressing business.
- The hero slideshow displays selected photos of Lydia's hair work.
- The slideshow rotates slowly so visitors have time to view each image.
- Visitors can pause the slideshow and use controls to move forwards and backwards through the images.
- The slideshow controls work on mobile, tablet and desktop.
- An About Lydia section includes a photo of Lydia and an introduction about her.
- The About Lydia section includes information about her skills and training.
- The About Lydia section includes links to the Gallery and Enquiry pages.
- A featured reviews carousel appears on the homepage.
- The reviews carousel is clickable and takes visitors to the full Reviews page.
- The homepage layout works on mobile, tablet and desktop without content being cut off or causing horizontal scrolling.
- Images resize correctly and remain clear on different screen sizes.
### US02 – Enquiry call to action
- A clear **“Make an enquiry”** button is included in the header on every page.
- An enquiry link is also included in the footer on every page.
- All enquiry links take visitors to the enquiry form.
- Links and buttons are easy to see and tap on mobile devices.
- Visitors can reach the links using the Tab key.
- A visible focus style shows which link or button is selected.
- Pressing Enter activates the selected link and takes the visitor to the correct page.
- Keyboard navigation follows a sensible order and does not get stuck.
### US03 – Reviews
- Genuine reviews supplied by Lydia are displayed on the Reviews page.
- All five reviews provided by Lydia are included, with the option to add more in the future.
- Reviews are displayed in separate cards, arranged in rows of three on larger screens.
- The layout adjusts to fit smaller screens without cutting off content or causing horizontal scrolling.
- A featured reviews carousel appears on every page except the Reviews page.
- The reviews carousel rotates slowly and includes controls to pause, move forwards and move backwards.
- Clicking the reviews carousel takes visitors to the full Reviews page.
- Review text is clear and easy to read on different screen sizes.
### US04 – Gallery
- The gallery displays examples of Lydia's hair styling and colouring work.
- Recent Instagram posts are used if they can be displayed reliably on the website.
- If using Instagram posts is not practical, the gallery uses photos supplied by Lydia.
- The gallery can be updated with new photos as Lydia provides them.
- Images resize correctly and remain clear on mobile, tablet and desktop.
- The gallery layout is easy to view and navigate on different screen sizes.
- Visitors can view the images without content being cut off or causing horizontal scrolling.
### US05 – Enquiry form
- The form collects the contact details Lydia needs to respond, including a required email address and phone number.
- Visitors must provide a short description of the service they are interested in or the advice they need.
- The form does not ask for a home address or photo uploads at first contact.
- An optional “How did you hear about Lydia?” dropdown includes Word of mouth, Google/search, Instagram, Facebook, Other and Prefer not to say.
- When a form is submitted successfully, the enquiry is sent to Lydia and the visitor receives a confirmation.
- The form service's delivery, privacy and automatic acknowledgement features are checked before it is used for real enquiries.
- The form works on mobile, tablet and desktop without content being cut off or causing horizontal scrolling.
### US06 – Services and prices
- Each service includes its name, a description and a starting price.
- Visitors are told that extra travel costs may apply.
- Visitors can easily scroll through the services and find the information they need.
- The services page works on mobile, tablet and desktop without horizontal scrolling or content being cut off.
### US07 – Cancellation policy
- The FAQ explains that cancellations made with at least two days' notice have no cancellation fee.
- It explains that cancellations made with one day's notice have a 50% fee of the booked service cost.
- It explains that same-day cancellations or not attending an appointment have a 100% fee of the booked service cost.
- It explains that any outstanding cancellation fees must be paid before future appointments can be confirmed.
- It explains that a deposit may be required when booking.
- Visitors can easily find and read the cancellation policy on mobile, tablet and desktop.
### US08 – Training
- The About section includes Lydia's training and experience once she has provided the details.
- All information is checked with Lydia to make sure it is accurate and does not include anything she has not confirmed.
- Visitors can easily find and read the information on mobile, tablet and desktop.
### US09 – Social media and contact
- WhatsApp, Instagram and Facebook icons are included in the footer and on the Enquiry page.
- Each icon takes visitors to the correct social media account or contact link.
- The icons have labels that make them understandable to visitors using assistive technology.
- The links are easy to use on mobile, tablet and desktop, including when navigating with a keyboard.


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