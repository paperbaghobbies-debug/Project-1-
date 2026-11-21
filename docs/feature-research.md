# Feature Research and Decisions
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
**Other Possible Research** 

When I started mapping the main website features from the user stories and Lydia’s feedback, I realised there were other things I needed to look into before I could actually build them. Features like the gallery, enquiry form and reviews carousel brought up questions about how they would work, such as getting Instagram posts onto the site, sending form submissions without extra costs, making sure the colours meet accessibility requirements and keeping images loading quickly. This meant I needed to do some more research into the technical side, accessibility, design and how data would be handled, so I could work out the best way to build each feature.

- Hosting and running costs
- Custom domain
- Enquiry form delivery
- Photo uploads with enquiries
- Portfolio gallery fallback 
- Updating prices and other content
- Header behaviour
- Fonts
- Image quality and loading
- Colour palette and contrast
- Responsive layout and rendering
- “How did you hear about Lydia?” field
- Search visibility and service area

## Feature Research and Decisions

### 1. Hosting and running costs

I looked at GitHub Pages and Cloudflare to see which would be better for hosting the website. I wanted something that would be cheap, secure and easy to manage.

GitHub Pages has some rules about using it for business websites, so Cloudflare Pages might be a better option. It also has a free plan, which could help keep costs down.

Sources:
- [Cloudflare plans](https://www.cloudflare.com/plans/#application-services)
- [Cloudflare Pages pricing](https://www.cloudflare.com/plans/free/)
- [GitHub Pages limits](https://docs.github.com/en/pages/getting-started-with-github-pages/github-pages-limits)
- [Cloudflare Pages vs Workers](https://flaviocopes.com/cloudflare-pages-vs-workers/)

I am thinking of using Cloudflare Pages if it supports all the features I need. I still need to check its limits and whether it is suitable for Lydia's business.

I also need to work out the costs for the domain, hosting, enquiry form and any future website updates.

### 2. Custom domain

- Lydia wants her own domain for the website and would like to keep the cost low. Her preferred name is "Hairbylydia-Banbury", and she expects to own and pay for it herself.
- I looked at Cloudflare's information about domain prices to get an idea of how much it might cost.

Source:
- [How much does a domain name cost?](https://www.cloudflare.com/learning/dns/how-much-does-a-domain-name-cost/)

- I am thinking of using Cloudflare for the domain if it works with the hosting. I still need to check whether the name is available, decide on the ending, such as .co.uk or .com, and compare the registration and renewal prices.

### 3. Enquiry form

- The website needs an enquiry form that sends messages to Lydia without adding too much cost.
- I looked at Cloudflare Email Service and FormSubmit. Cloudflare could be an option, but I need to test whether it will work with the website. FormSubmit says it offers free forms and submissions and stores submissions for 30 days.

Sources:
- [Cloudflare Email Routing](https://www.cloudflare.com/developer-platform/email-routing/)
- [FormSubmit](https://formsubmit.co/)
- [FormSubmitEndpoints](https://formsubmit.co/documentation)
- [FormSubmit Privacy Policy](https://formsubmit.co/privacy.pdf)

- I think FormSubmit could be suitable for Lydia because she only needs the form for first contact with potential clients. It can send enquiries straight to her email without needing a backend, so I plan to keep the form simple and only collect basic contact details and a short description of the enquiry, leaving home addresses and photos until after Lydia has spoken to the client.
- Although Lydia originally wanted to collect home addresses, I have decided to keep the initial enquiry form simpler by only asking for basic contact details and a short description of the enquiry. This should reduce the amount of personal information collected through the website and help limit privacy risks.


### 4. Photo uploads with enquiries

- Lydia mentioned that it might be useful for clients to upload photos when sending an enquiry.
- I am thinking of leaving photo uploads out of the form for now. Instead, clients could send their photos to Lydia through WhatsApp or email after she has replied. This would keep the form simple and avoid collecting photos straight away.
- I asked lydia this on 09/11/2026 over the phone and she confirmed that this can be kept until after first contact with her.

## 5. Portfolio gallery and Instagram

- Lydia would like her Instagram work to be used on the website, and she would prefer the gallery to show her recent posts if possible.
- I looked into the Instagram API to see if it would be possible to show her posts automatically. I also looked at Meta's policies and some discussions about displaying Instagram photos on websites.

Sources:
- [Instagram API with Facebook Login](https://developers.facebook.com/documentation/instagram-platform/instagram-api-with-facebook-login)
- [Meta content and intellectual-property policy](https://www.meta.com/en-gb/help/policies/2202628709913826/)
- [Displaying an Instagram gallery discussion](https://stackoverflow.com/questions/12478772/how-do-i-use-instagrams-api-to-display-a-gallery-of-my-own-photos)

- I would like to use the Instagram API if it works properly and is not too difficult to maintain. If this is not possible, I can make a normal gallery using photos Lydia provides.
- I still need to test the Instagram option and check what access is needed.

## 6. Updating prices and photos

- Lydia originally said she could update her own prices and photos, but later said she would rather send updates to someone else to make.
- She expects photos to be updated about once a month and prices about once a year or less.
- I looked into Cloudflare Workers KV and ways of editing website content, but I think making a system for Lydia to update everything herself would be more complicated than she needs.
- I am thinking of keeping the website simple and having Lydia send any new photos or prices to someone else to update for her. I still need to work out who would do this and whether there would be any extra costs.

Sources:
- [Cloudflare Workers KV](https://www.cloudflare.com/products/kv/)
- [Cloudflare discussion about editing a website](https://community.cloudflare.com/t/edit-code-of-website-with-cloudflare/478014)

## 7. Reviews and review carousel

- Lydia wants some of her client reviews to be shown on the website so visitors can see what other people think of her services.
- I looked at how to make review carousels accessible and also looked at some examples of how they work.

Sources:
- [Accessible carousel guidance](https://www.a11y-collective.com/blog/accessible-carousel/)
- [Reviews carousel example](https://github.com/antonADev/reviews-carousel)
- [Carousel implementation video](https://www.youtube.com/watch?v=nbNBe2bAw8c)

- I am thinking of making my own review carousel using HTML, CSS and JavaScript. It would move slowly between reviews and have buttons to go back, move forward and pause the carousel.
- I also want to make sure visitors can still read the reviews if JavaScript is not working. The reviews could also be shown as cards on a separate Reviews page.
- I am not planning to use Google Reviews. Lydia has chosen five reviews to feature and has given permission for them to be used. I still need to check the original reviews for their ratings and service details so I do not include anything that has not been provided.

## 8. Header design

- Lydia liked the transparent sticky header on one of the competitor websites and wanted to see if a similar style would work for her website.
- I looked at different examples of sticky headers and how they change when scrolling. I also looked at how they work on mobile screens.

Sources:
- [Transparent scrolling headers](https://uicookies.com/snippets/transparent-scroll-header/)
- [Scroll-linked header effects](https://uicookies.com/snippets/scroll-linked-header-effects/)
- [Sticky header changes](https://vinish.dev/sticky-header-changes-on-scroll)
- [CSS header design](https://wpdean.com/css-header/)
- [Sticky header mobile and SEO considerations](https://www.j-a-b.net/how-to-design-a-sticky-header-that-does-not-hurt-mobile-ux-or-seo/)
- [CSS sticky positioning](https://sizzy.co/blog/css-position-sticky)

- After discussing it with Lydia on 28/10/2026, she decided not to use a transparent header because her logo would not look right against it. Instead, she agreed to have a taupe header that stays at the top of the page.
- I will use a fixed taupe header and test it on smaller screens to make sure it does not cover the page content.

## 9. Fonts

- Lydia wants to keep Noto Serif Display Extra Condensed for "Hair by Lydia" on the main branding image and Luxurious Script for the other branding.
- I checked both fonts and their licences to make sure they can be used on the website.

Sources:
- [Noto Serif Display](https://fonts.google.com/specimen/Noto+Serif+Display)
- [Noto Serif Display licence](https://github.com/google/fonts/blob/main/ofl/notoserifdisplay/OFL.txt)
- [Luxurious Script](https://fonts.google.com/specimen/Luxurious+Script)
- [Luxurious Script licence](https://github.com/google/fonts/blob/main/ofl/luxuriousscript/OFL.txt)

- I will use the fonts Lydia has chosen for the branding. I also need to choose a simpler font for the main text so that the website is easy to read. I can show Lydia the font before making a final decision.

## 10. Image quality and loading

- Images are an important part of the website because they show Lydia's hair work. I want them to look clear and load properly without making the website slow.
- I looked at lazy loading and responsive images to see how images can be made to work better on different screen sizes.

Sources:
- [Lazy loading performance](https://www.debugbear.com/blog/lazy-loading-performance)
- [Lazy-load performance](https://pagespeed.one/en/know-how/lazyload)
- [Responsive images – MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Guides/Responsive_images)
- [Responsive images with srcset](https://docs.imgix.com/en-US/getting-started/tutorials/responsive-design/responsive-images-with-srcset)

- I plan to use responsive images where needed and lazy load images further down the page so they do not all have to load straight away.
- I will also test the gallery to make sure the images look good and do not take too long to load.

## 11. Colours and contrast

- Lydia wants the website to use warm beige, cream and brown colours.
- I sampled the taupe colour from her logo background as `#7F7367` and used the WebAIM Contrast Checker to test different colour combinations.

Sources:
- [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/)
- [WCAG 2.2 contrast guidance](https://www.w3.org/WAI/WCAG22/Understanding/contrast-minimum.html)
- [WCAG 2.2 non-text contrast guidance](https://www.w3.org/WAI/WCAG22/Understanding/non-text-contrast.html)

These were the results I got:

| Text colour | Background colour | Contrast | Result |
|---|---|---:|---|
| White `#FFFFFF` | Taupe `#7F7367` | 4.61:1 | WCAG AA |
| Dark brown `#342B24` | Cream `#FAF3EB` | 12.58:1 | WCAG AAA |
| Dark brown `#342B24` | Muted gold `#C6A15B` | 5.70:1 | WCAG AA |

- I am thinking of using taupe for the navigation bar with white text, cream or off-white for the background, dark brown for normal text and muted gold for buttons.
- I will check the colours again when they are being used on the actual website, including when buttons are hovered over or selected.

## 12. Responsive layout

- I used what I learned from my freeCodeCamp Responsive Web Design certificate and looked at more information about making websites work on different screen sizes.
- I also looked at how websites are displayed and how JavaScript can affect page content.

Sources:
- [Responsive design – MDN](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/CSS_layout/Responsive_Design)
- [Chrome DevTools device mode](https://developer.chrome.com/docs/devtools/device-mode/)
- [HTML templates](https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/template)
- [JavaScript SEO basics](https://developers.google.com/search/docs/crawling-indexing/javascript/javascript-seo-basics)
- [Rendering approaches](https://developers.google.com/solutions/content-driven/hosting/rendering)
- [Client-side template discussion](https://stackoverflow.com/questions/16255859/client-side-templates-in-script-tags-advantages-disadvantages)
- [JavaScript templating engines](https://hackernoon.com/pros-and-cons-of-popular-javascript-templating-engines)

- I plan to build the website with a mobile-first layout using flexible CSS and media queries. I can use Flexbox where it is useful.
- I will keep the main website content in HTML and only use JavaScript when it is needed for features such as the slideshow and review carousel.
- I will test the website at different screen sizes and, if possible, on a real phone as well.

## 13. "How did you hear about Lydia?" field

- Lydia would like to know how people find her business.
- I am thinking of adding an optional dropdown to the enquiry form with these choices:

  - Word of mouth
  - Google/search
  - Instagram
  - Facebook
  - Other
  - Prefer not to say

- The answer would be included in the email Lydia receives when someone sends an enquiry. I do not think extra tracking is needed for this.
- I still need to check that Lydia is happy with the options and test that the answer is included in the email.

## 14. Search visibility and service area

- Lydia wants more people to find her business online and make enquiries. She is a mobile hairdresser covering Banbury and surrounding areas and does not currently use Google Business Profile.
- I looked at Google's SEO guidance to learn more about page titles, search results and how websites are found. I also looked at Google Business Profile and its rules. I found some articles about keywords for hair salons, which gave me ideas for wording to use on the website.

Sources:
- [Google SEO starter guide](https://developers.google.com/search/docs/fundamentals/seo-starter-guide)
- [JavaScript SEO basics](https://developers.google.com/search/docs/crawling-indexing/javascript/javascript-seo-basics)
- [Google title links](https://developers.google.com/search/docs/appearance/title-link)
- [Google search snippets](https://developers.google.com/search/docs/appearance/snippet)
- [Google Business Profile](https://support.google.com/business/answer/7091)
- [Google Business Profile eligibility](https://support.google.com/business/answer/3038177)
- [Seopital – Hair salon SEO keywords](https://www.seopital.co/blog/the-best-hair-salon-seo-keywords)
- [MarketKeep – SEO keywords for hair salons](https://marketkeep.com/seo-keywords-for-hair-salons/)
- [Ron Kot – SEO keywords for hair salons](https://www.ronkot.com/best-seo-keywords-for-hair-salons/)
- [Digitally Top – SEO for hair salons](https://digitallytop.com/digital-marketing/seo-for-hair-salons/)

- I plan to use separate pages for the main website content, with clear page titles, headings and links.
- I will also include information about Lydia's services and the areas she covers, using Banbury and surrounding villages in the website text.
- I am not including Google Business Profile in the current plan.
- I still need to check the service area with Lydia. The website can help people find her business, but I cannot guarantee where it will appear in search results.