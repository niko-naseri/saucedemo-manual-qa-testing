# SauceDemo | Manual QA & Usability Review

**Author:** Niko Naseri  
**Project type:** Independent QA portfolio project using a public demonstration website (not a paid client engagement)  
**System under test:** https://www.saucedemo.com/  
**Method:** Manual functional testing, negative checkout validation, desktop/mobile visual review.

## Why this project
Demonstrate an evidence-based QA workflow: define scenarios, compare expected and actual results, capture screenshots, distinguish reproducible defects from observations, and document scope limitations. Relevant to entry-level freelance web testing and QA roles in Finland.

## Results
- **9 functional/negative scenarios:** 9 passed in observed/reported runs.
- **3 mobile visual checks:** visual pass using Chrome DevTools iPhone 14 Pro (393 x 852), **not** testing on a physical iPhone.
- **1 content consistency finding (UX-001):** product named *Test.allTheThings() T-Shirt (Red)* depicts a sweatshirt-style long-sleeved garment. Catalog specification not available, so classified as usability/content observation, **not confirmed software defect**.
- **Intermittent authentication observation:** occasional redirects to login during checkout/product navigation. Not consistently reproduced; no known session policy or root cause. **Inconclusive**.
- **0 confirmed functional bugs** within the executed scope.

## Files
- `SauceDemo_Test_Execution.xlsx`: steps, expected vs. observed outcomes, evidence pointers, notes.
- `SauceDemo_QA_Report.pdf`: concise project summary and sample evidence.
- `evidence/`: screenshots captured during hands-on manual testing.

## Test coverage
Login with missing credentials; valid login; add/remove item; cart product verification; sort six products by ascending price; complete checkout; first/last name and postal-code required validation; visual mobile review of product, cart and checkout pages.

## Limitations & ethics
- Results reflect a series of manual sessions, not an automated suite or exhaustive regression.
- Some conditions (such as logout timing) were reported by the tester and lack timed screen recordings; these observations are not marked confirmed bugs.
- Mobile layout was inspected in Chrome DevTools only; no physical phone, mobile Safari, or touch-device testing.
- Responsive layout appearing denser on mobile is expected and not labelled a defect absent actual clipping, distortion or loss of content.
- The screenshot evidence comes from a third-party demo site; the site's owners do not sponsor or endorse this portfolio.
- Password-manager warnings originating from Chrome were excluded from product issues.

## Future improvements
Extend to cross-browser and keyboard accessibility checks; design an automated smoke-test suite with Playwright + Pytest in a separate project; introduce GitHub Actions and concise CI reports.
