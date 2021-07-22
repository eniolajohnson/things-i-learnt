# things-i-learnt

This repository will be a note-taking reminder on new things I learn on days I don't code.

## 22nd July, 2021 - Manual QA Testing: BUGS

## **What is a bug?**

A bug is something that is preventing us as a company from delivering a project to a customer successfully.

If we look further - this is something that prevents our customers from running their business as intended.

It can take very clear form e.g. customers can not pay online for a product or add to cart button does not work. It can also take more subtle forms, for example, some text is written incorrectly, there are some spelling errors, small deviations in alignment, which damages brand image and decreases the credibility of an online channel.

## **What is a bug specifically - the types of bugs**

This “something that does not work” can take the following forms that we aim to find, describe and report. There are the following types of bugs we look at: 

- CONTENT

    This bug concerns deviation in textual or visual copy from what is expected. Expected here is design and a lot of COMMON SENSE regarding UI, notifications, call to actions, and generally text matching the purpose of a page or a block on a page.

    It can be a spelling error in text or heading, can be a notification message that is not yet translated e.g. we show “Product is added to the cart” on a site that is expected to run in Arabic.

    It also can be some “Lorem ipsum” text that was put by the developer to test a feature and everybody got used to it and forgot to change. Missing content is also a bug e.g. when you click a link “About us” and it is either not clickable or shows an empty page or a page with test data.

    **Summary**

    - Not clickable link e.g. in footer to About us, Contacts, History
    - Spelling errors
    - Link not leading anywhere or to some “demo landing page”
    - Capitalisation errors or wrong punctuation e.g. spaces before commas
    - Not translated UI text or notifications (e.g. add to cart, view cart, invalid email)
    - Not translated text on a different site language version e.g. we have 3 languages and German site shows some pages and product descriptions still in English
    - Demo or test content - text (lorem ipsum)
    - Demo or test content - images
    - Missing content, where it is expected to be

    **How to report such a bug?**

    You need to think about the easiest way to locate it i.e site area, where it does occur e.g. Home, Product listing page or Cart page, URL of the page, where it does occur and a screenshot with an problem area marked clearly by e.g. red frame.

    The behaviour of this bug is usually static and it is usually present across all browsers and devices.

    Example

    [https://lh3.googleusercontent.com/yQhN-U61BDqEq5SeuhLQ3vo2UGilvHYVQ0QAQNRx283LL-Y0WdP_Qa_WfQLHqi63A2MSEPhivKCRB6lykd4Nvy6NWscqQzvu5LLFAdTQdy25_TI7YawlHW2xyDpHFzMwwU9eQ9ue](https://lh3.googleusercontent.com/yQhN-U61BDqEq5SeuhLQ3vo2UGilvHYVQ0QAQNRx283LL-Y0WdP_Qa_WfQLHqi63A2MSEPhivKCRB6lykd4Nvy6NWscqQzvu5LLFAdTQdy25_TI7YawlHW2xyDpHFzMwwU9eQ9ue)

    > Managing content bugs is EXTREMELY important for a successful project. There are cases when a project is fully functional, visually correct, but … we failed to inform customers on the inventory of the content they need to provide… so, it is the last moment and we tell them that they need to translate a bunch of their pages about Values, Brand History, Testimonials and even contacts…

    > Creating and monitoring the CONTENT that is necessary for a site to be successfully delivered is a very important task.


- VISUAL

    This bug is about deviations of site **visual layout** from what was confirmed in designs or style guide.

    Visual bugs can be for example sizes, colours and types of fonts that differ from agreed in design mockups. It can be spacings, margins that are different on the site than in provided designs. Some sites rely on a minimalist design that only looks beautiful if all spacings, margins and the overall grid is pixel-perfect.

    **Summary**

    - Pixel-perfect revision of gaps between actual delivered project and confirmed designs
    - Pixel-perfect revision under conditions of changes in screen size from desktop to tablet and mobile - RESPONSIVE DESIGN CHECK
    - Any changes in colors, sizes, positioning, margins, order of elements from designs or style guide
    - Any visual inconsistencies, that is, all margins are 150px from the screen, but one CMS page has just 40 px
    - Wrong ones or absence of hover effects, state of selected elements
    - Content does not fit an area, overflows it or is mis-aligned e.g. not centered
    - Missing designs elements e.g. particular background or background colors
    - Revision of all active elements such as links, buttons, input fields, error messages and their states e.g. when I click into an input field, does it change its border color to look like an active element?

    **How to report such a bug?**

    - Naturally, you need to indicate the site area e.g. checkout or home
    - URL to get there and
    - a screenshot with a framed area indicating, where exactly the problem is.
    - Additionally, you have to explain what is the expected result or link to a confirmed design or make a side-by-side comparison of actual delivery and confirmed designs.

    How to report bugs that appear only on certain screen resolution (break point)?

    - Naturally, we need a screenshot and the SCREEN SIZE that leads to this bug.

    *Example:*

    [https://lh5.googleusercontent.com/jgnz1he572GJjEKzRRBOhQ0J4VWg0y5AeZ-MqJZp5DUHgCpVbqWiVWg7nPaqrd2qINsk064DzpA8gZKLMDufTEV7z-JOtANREmE8f3_tCGD5Yg9F62-LXlpUOpRNTwHmNQ4sBe3Z](https://lh5.googleusercontent.com/jgnz1he572GJjEKzRRBOhQ0J4VWg0y5AeZ-MqJZp5DUHgCpVbqWiVWg7nPaqrd2qINsk064DzpA8gZKLMDufTEV7z-JOtANREmE8f3_tCGD5Yg9F62-LXlpUOpRNTwHmNQ4sBe3Z)

- CROSS-BROWSER

    Cross-browser bugs happen when our code is written incorrectly, which results in different browsers displaying the site differently to the extent that is harmful for the business.

    Simply put - cross-browser bugs are the ones that demonstrate that the feature or certain visual block is behaving correctly in one browser, BUT… is not working correctly in another.

    **Summary**

    - Cross-browser issues usually result in new VISUAL bugs that are spotted in a certain browser or browser version
    - Cross-browser issues also can result in FUNCTIONAL bugs, when certain operations can be performed in one browser, but can not be executed in another
    - There can be cases, when cross-browser issues also affect performance and some browsers would load the page much longer than another

    **How to report such bug?**

    - The same as VISUAL bugs + need to indicate which browsers are OK and which are not OK.

    **Q & A**

    Can you start cross-browser testing without figuring out what are the browsers we have committed to support on this project?

    Yes, in this case, you can test in the latest Chrome, Safari and Edge. But usually, in a project, there is very clear information on what browser support is included in the project price and we should only test in the supported ones.

    What is a critical thing to note in a bug description for a cross-browser?

    Naturally, browser name and version, where a bug occurs, so that developer can figure out how to reproduce it and then check that it is working OK in this browser version.

    Should I report minimal deviations in fonts or alignments, if they do not break the design?

    Generally, no, but better double check with the PM of the project. Our aim at QA to find the things that materially break functionality and user experience, so we have to first focus on these rather than minor deviations if these come unnoticed.

- CROSS-DEVICE

    Cross-device is similar to cross-browser, but the difference in behavior here is device specific. For example, a layout is correct in Chrome on iPhone, but does not have part of the image in Chrome on Android.

    Particular devices to test will be listed by PM, but usually we use iPhone, Android phone, and Apple and Android versions of a tablet.

    **How to report such bug?**

    - The same as VISUAL, but indicating a particular device, where there is a deviation from the norm.

- FUNCTIONAL

    The functional bug is a behaviour that does not work as intended or does not work at all. This is a type of bug, where you need to describe explicit steps on how to reproduce it because it concerns something a bit more complex than just missing content or wrong alignment.

    For example

    - You choose in the filter on product listing page to show “clothes of color “red”, but clothes of all colours are shown after filtering is completed
    - You see that page tells it has loaded 26 products, but there are actually only 14
    - After email is added to the newsletter signup form, it tells that “Thank you, email is added”, but there is no such email in the database
    - Product listing page “NEW ARRIVALS” shows 404 page instead of showing assigned products
    - Product image gallery shows broken images or missing images, see URL for details
    - Product price of a product is different on product listing page and on product detail page
    - When searching in search for exact product name, the product does not show up in the search suggestions
    - Checkout shows infinite loader after credit card data is submitted and order is not placed
    - After submitting username and password to login to customer account and clicking “Login” button the site shows “Internal server error”
    - When clicking “About us” link in the footer, the page shows 404 error
    - While VAT tax rate in back end is set to 25%, the front end calculates it as 21% when seeing prices on product listing page, detail page, cart and checkout
    - Customer group DEALERS has special prices set in the back end for all products, but usual retail prices are shown when a member of DEALERS group logs into the store and browses catalog, adds product to cart or tries to checkout
    - Customer submits name and surname for product engraving, but these do not show up in the order details in the back end after the order is placed

    **How to report such bug?**

    - A good title is 90% of the success! Check the above examples, you can generally understand what the issue is and where to locate it, how to reproduce it. However, for the avoidance of any doubt, for functional bugs, it is a MUST to add specific “how to reproduce the bug” steps and also describe the actual result you got versus expected result that a developer should aim for fixing the bug.

    Example

    After adding any product item to a cart, the site shows 404 page

    [https://lh5.googleusercontent.com/_kgsqZc0nOMLnz4mWmzHYj2wLQK9pV6Jmveg-nQBnpbtC9YFyCD3uTIxh11SSMM7T4YYsyhIX7n2NdmQlcRzZ3yKEE-rVz-_-mKsktcRydg_RS4LRY6ok-ULAu1Y05-Js-JkWwmf](https://lh5.googleusercontent.com/_kgsqZc0nOMLnz4mWmzHYj2wLQK9pV6Jmveg-nQBnpbtC9YFyCD3uTIxh11SSMM7T4YYsyhIX7n2NdmQlcRzZ3yKEE-rVz-_-mKsktcRydg_RS4LRY6ok-ULAu1Y05-Js-JkWwmf)


- PERFORMANCE

    This is a bug related to a time necessary for a page to load or product to be added to a cart or search to return search result, login form to let user in and so on. Time is of essence here. A general guideline is that no operation can exceed 2-3 seconds, if it takes more most probably there is some technological flaw that needs to be addressed.

    Summary

    - First page load, try incognito and remove all cache
    - Search results
    - Filtering of products on the listing page
    - Check the Kb size of the images on the page, sometimes, some banner can be 2Mb and delay page load for few seconds
    - On the product listing page - see the sizes (dimensions and Kb) of the images, these should be some 25-30Kb, but there are cases of these being 600-700Kb and naturally these force users to load some 25-30Mb extra per page!
    - Listing page first loading
    - Pagination
    - Adding product to cart
    - Placing an order
    - Logging in and logging out of customer account

    **How to report?**

    - Site area, specific URL, steps taken e.g. choosing some filters, time it takes, video will help there!
