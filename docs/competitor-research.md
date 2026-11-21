# Competitor Research

This document records my findings and observations from competitor research.
I am documenting my competitor website evaluations and client feedback to establish clear design features to adopt and avoid for my project.

## Lydia's Direct Feedback and Site Impressions

I sat with Lydia, and she chose three competitors. We went through each website together, and Lydia shared her initial thoughts and feedback on what she liked and disliked.


## 1.Hairnovate [source: https://hairnovate.co.uk]
 **Likes:** 
- Star ratings displayed alongside client reviews.
 **Dislikes & Critiques:** 
- Dislikes the overall layout. 
- A single, long-scrolling page feels boring and unengaging. 
- Unlikely to convert or win over new clients.

## 2.Emz Hair & Wellness [source: https://emzhair.co.uk]
 **Likes:** 
- Clean typography and font choices. 
- Active-section indicator in the navigation bar.
- The "Request Appointment" form structure closely matches our desired enquiry path.
 **Dislikes & Critiques:** 
- Lydia felt that the slideshow was similar to the one we are considering, but that its images did not show real client transformations.
- Image resolution is noticeably low.


## 3.Matthew Grant Hairdressing [source: https://www.matthewgranthairdressing.co.uk]
**Likes:** 
- Navigation bar design and smooth sticky behavior. 
- The call to action button in the "About Me" section could link directly to Services and Portfolio on our site. 
- The review carousel draws attention and is very interactive.
**Dislikes & Critiques:** 
- Feels impersonal and clinical.

### Dev Research 

I evaluated all three websites against six criteria and recorded my findings. I also checked their colour contrast and accessibility using Lighthouse and browser developer tools. These findings, together with Lydia’s feedback, will help inform my design decisions and guide further research into specific features.

### 1.Hairnovate [source: https://hairnovate.co.uk]

- **Layout & branding:** I found the layout unengaging and more like a basic digital leaflet. I also couldn’t find real examples of hair work to help build trust.
- **Gallery / portfolio:** I couldn’t find a dedicated gallery showing client transformations.
- **Prices & services:** I found a clear price list for cuts, blow-dries and colour treatments.
- **Enquiry route / CTA:** I found consultation and deposit information, but no quick online enquiry form.
- **Mobile responsiveness:** I found the single-page layout easy to scroll through on a mobile screen.
- **Accessibility:** The page looked readable to me, but Lighthouse flagged a colour-contrast error. 

### 2.Emz Hair & Wellness [source: https://emzhair.co.uk]

- **Layout & branding:** I liked the clean layout, stylish fonts and active-section indicator in the navigation.
- **Gallery / portfolio:** I found a slideshow on the homepage and a separate gallery showing hairstyle photos. I could not verify whether the slideshow image showed real client work,but it appeared low-resolution to me.
- **Prices & services:** I found a clear list of services and prices.
- **Enquiry route / CTA:** I found the “Request Appointment” form similar to the enquiry process I’m considering for my site.
- **Mobile responsiveness:** I found the layout easy to use on mobile, with readable text and touch-friendly navigation.
- **Accessibility:** Lighthouse flagged a colour-contrast issue.

### 3.Matthew Grant Hairdressing [source: https://www.matthewgranthairdressing.co.uk] 
- **Layout & branding:** I liked the polished layout and noticed that the navigation changes from transparent to sticky as you scroll.
- **Gallery / portfolio:** I found professional imagery and liked that the About section links to the services and portfolio.
- **Prices & services:** I found the service categories clearly organised.
- **Enquiry route / CTA:** I noticed prominent “Book Online” links and easy-to-find contact details.
- **Mobile responsiveness:** I found the mobile navigation and touch targets easy to use.
- **Accessibility:** The layout and text looked clear to me, but Lighthouse flagged colour-contrast issues and images without alt attributes.

### Development Takeaways

Based on Lydia’s feedback and my research, I will use the following points to guide the website’s design and features:

 **Enquiry form:** Lydia likes to discuss a clients hair goals and provide a brief consultation before confirming an appointment. I will build an enquiry form that helps start this conversation instead of designing a full booking system.
**Real client transformations:** Lydia wants her work to be highlighted, I will use clear, high-quality photos in the gallery and slideshow to showcase here skills.
**Reviews:** Lydia liked star ratings alongside reviews, and I found the review carousel an interesting design feature. I will consider showing selected reviews on pages, with Reviews having its own standalone page.
**Navigation:** I liked the navigation bar I saw in Matthewgrant research. I will make the site easy to navigate and explore whether a header that is clear and and easy to use and responsive.
- **Services and prices:** I found clear price lists useful so I will make Lydia’s services and prices easy to find and understand.
- **Page layout and personality:** Lydia disliked a long scrolling page, and she felt that one site felt impersonal. I will organise the content into clear sections and use a warm, personal style that reflects Lydia’s personality.
- **Accessibility:** I will aim for readable text, sufficient colour contrast, descriptive image alt text and layouts that work well on mobile devices.

### Screenshot Evidence

I captured screenshots of the three competitor websites to support my observations about their layouts and features. I also used Lighthouse to check accessibility, including colour contrast. The Lighthouse screenshots show automated findings and do not represent a full accessibility assessment.

- **Hairnovate:** [Page layout and About section](./screenshots/hairnovate-ref-1.png), [reviews and gallery](./screenshots/hairnovate-ref-2.png), [mobile layout](./screenshots/hairnovate-ref-3.png), [Lighthouse results](./screenshots/hairnovate-ref-4.png), [Lighthouse accessibility and contrast findings](./screenshots/hairnovate-ref-5.png).
- **Emz Hair & Wellness:** [Homepage and navigation](./screenshots/emz-ref-1.png), [appointment enquiry form](./screenshots/emz-ref-2.png), [gallery](./screenshots/emz-ref-3.png), [mobile layout](./screenshots/emz-ref-4.png), [Lighthouse accessibility and contrast findings](./screenshots/emz-ref-5.png).
- **Matthew Grant Hairdressing:** [Homepage and navigation](./screenshots/mgh-ref-1.png), [About section and links](./screenshots/mgh-ref-2.png), [mobile view and Lighthouse performance results](./screenshots/mgh-ref-3.png), [reviews](./screenshots/mgh-ref-4.png), [Lighthouse accessibility and contrast findings](./screenshots/mgh-ref-5.png).