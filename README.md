# Power BI Course Materials - Page Redesign

A fix and redesign for the "Power BI Course Materials" delivery page on **Data With Baraa Academy**. This addresses a broken/unbuilt page linked from the platform's purchase-confirmation email.

## The problem

The email links to `academy.datawithbaraa.com/p/power-bi-course-materials-955781/`, which currently resolves to an **unpublished Teachable template** - not the real course materials page. Visible issues on the live page:

<img width="659" height="317" alt="image" src="https://github.com/user-attachments/assets/bed5da97-7391-4b94-9519-064420baeaf8" />

<img width="959" height="473" alt="image" src="https://github.com/user-attachments/assets/0a62d119-7982-4a76-b23d-a9c7db095808" />

<img width="947" height="417" alt="image" src="https://github.com/user-attachments/assets/57bf007b-739b-4317-8212-00080843193d" />


- Headline still reads placeholder text: *"Name of Digital Download"*
- The CTA button has no destination configured
- Filler blocks (*"Example Text"*, *"Example Image with Text"*) are still in place
- The page footer states *"This product is not currently available"* - directly contradicting the purchase/confirmation email that sent people there

Net effect: someone who just signed up lands on what looks like a broken or abandoned page, which erodes trust and likely costs enrollments/downloads.

## The fix

`Power_BI_Materials_Page_Redesign.html` is a fully coded mockup of a real replacement page. Key changes:

<img width="947" height="478" alt="image" src="https://github.com/user-attachments/assets/3a35b4f4-5f13-43e2-8439-fb48a010d8a6" />

<img width="948" height="415" alt="image" src="https://github.com/user-attachments/assets/89d4ff7d-ca88-45cc-8488-8562c9d7efe4" />

<img width="948" height="412" alt="image" src="https://github.com/user-attachments/assets/5b746175-6c2f-4f59-90c0-a95b1df2b0cf" />

| Issue | Fix |
|---|---|
| No confirmation the order/signup worked | Green "Order confirmed - access unlocked" status chip at the top |
| Vague, non-functional CTA | Single clear CTA - **"Access Your Materials"** - with an actual destination |
| No visibility into what's included | A manifest card listing the real files (`.pbix`, `.pdf`, `.zip`, `.xlsx`) with checkmarks |
| No fallback if something breaks | Visible "Contact support" link directly under the CTA |
| Dead end after materials | A closing banner pointing back to the full YouTube series |
| Generic/templated look | Styled with the brand's own teal (`#09A59A`) + Power BI gold, Space Grotesk / Inter / JetBrains Mono typography |

## Files

- **`Power_BI_Materials_Page_Redesign.html`**: the coded page. Open directly in any browser (double-click, or drag into a browser window). No build step, no dependencies required.
- **`Power_BI_Materials_Page_Preview.jpg`**: a static screenshot of the page, for quick reference in emails/slides where a live HTML file isn't practical.

## Notes for handoff

- All copy (order number, email, file names) is placeholder. Swap in real values or wire up dynamic fields if implemented on Teachable.
- The CTA button (`href="#"`) needs to be pointed at the actual materials location (LMS content page, hosted files, etc.).
- Fonts used: **Space Grotesk** (headlines), **Inter** (body), **JetBrains Mono** (labels) all free on Google Fonts.
