# Use Next.js to Query a Single Record From Supabase

## ✅Sequin Remix: No changes

Add static pages for each lesson following Jon's example.

## [📹 Jon's Video](https://egghead.io/lessons/supabase-use-next-js-to-query-a-single-record-from-supabase) & Overview

In this video, we look at building a pre-rendered static page for each of our lessons from Supabase. We use a Next.js dynamic route to create a page that can display the details for a lesson, and specify a finite list of possible urls with the getStaticPaths function.

The getStaticProps function will then be called for each of these lessons, and passed a params object to determine which page is currently being built. This is where we make a request for additional data from Supabase - in this case, the lesson's description. Again, the request will only happen once at build time, rather than each time the user requests the page.

Additionally, we use the Next.js `<Link>` component to enable client-side transitions from the landing page to each of the lesson details pages. This means we do not need to do a full page load from the server each time the user navigates to a new page. the `<Link>` component will pre-fetch each of our lesson's detail pages, while the user is browsing the list.

---

## [👉 Next lesson](/06-implement-third-party-authentication-with-github-in-next-js-using-supabase)