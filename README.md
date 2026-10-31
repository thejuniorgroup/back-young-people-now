# back-young-people-now

Site scripts for the Campaign for Youth Wellbeing (Back Young People Now) Webflow site.

They load through jsDelivr, pinned to a release tag, from two script tags registered in Webflow (Site settings > Custom code is not used for these):

| File | Loads in | What's inside |
|---|---|---|
| `bypn-head.js` | <head> | Logo loading animation, sub-page block styles and hovers, extra scroll-animation variants |
| `bypn-footer.js` | end of <body> | Menu open/close, marquee, placard logger, cookie banner + GoatCounter consent, FAQ accordion, voices rail drag, menu stagger + current page, CMS nav data and join buttons, page header helper, long text + On this page, scroll animations |

Each file is the original scripts joined in their original order, with a comment naming each one.

## Updating

1. Edit the file here and commit.
2. Create a new release tag (v1.0.1, v1.1.0...).
3. In Webflow, register the new version with the jsDelivr URL for that tag and its SRI hash, then publish.

URLs follow this pattern:
https://cdn.jsdelivr.net/gh/thejuniorgroup/back-young-people-now@v1.0.0/bypn-footer.js

Pinned tags never change, so a broken edit can't reach the live site until it's tagged and switched over in Webflow. To roll back, point Webflow at the previous tag.
