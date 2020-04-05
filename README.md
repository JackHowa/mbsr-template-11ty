# MBSR Template

This is for people who are signed up for Mindfullness-based Stress Reduction curriculum. The goal is for this to be a calm, informed and trustworthy tool to help people practice mindfulness. 

# Status 

[![Netlify Status](https://api.netlify.com/api/v1/badges/05801d79-90c8-4122-ab81-9325167f753f/deploy-status)](https://app.netlify.com/sites/mbsr-template/deploys)

[![Lighthouse score: 100/100](https://lighthouse-badge.appspot.com/?score=100)](https://lighthouse-dot-webdotdevsite.appspot.com//lh/html?url=https%3A%2F%2Fmbsr-template.netlify.com%2F)

# Roadmap

## MVP 

- [ ] List of all readings available
  - [ ] Readings Split By Week
  - [ ] Readings styled in calm and readable way
  - [ ] Minimal typos and formatting issues
- [ ] All audio available published
  - [ ] Able to stream on website
  - [ ] Split up links to streams or podcast by week 
- [ ] Week breakdowns (show readings and audio assignments for each week)

# Design

- [UI and colors via Figma](https://www.figma.com/file/2y476nV5FdF8NI4QdEa0Ns/mbsr-2?node-id=1%3A127)

# Features

- [ ] Dark mode to reduce eye strain 
- [ ] Offline storage of meditations and yoga audio for uninterrupted experience
- [ ] Payment processing with apple pay integration for seamless sign-up 
- [ ] Big, accessible buttons and text for participants with limited vision or dexterity 
- [ ] Native tasteful notifications of updates for daily practice notifications 
- [ ] Progress meter showing week and day, remembering that
  - [ ] Also, limitations on looking ahead for mindful, in-the-moment experience
  - [ ] Login and user memory 
  - [ ] Possibly sign-in with apple for privacy with patient
- [ ] Doodle calendar for scheduling when people would like to meet live
- [ ] Would be cool to use eleventy or other static site generator for serverless architecture
  - Good for iteration and performance and fun 



# Credit: ElevenTail

A project scaffold for quickly starting a site build with:

- [Eleventy](https://11ty.dev) for templates and site generation
- [Tailwindcss](https://tailwindcss.com) for a utility first CSS workflow
- [PurgeCSS](https://www.purgecss.com/) for optimizing CSS output
- [UglifyJS](https://www.npmjs.com/package/uglify-js) for a simple JS build pipeline
- [Netlify CLI](https://www.npmjs.com/package/netlify-cli) for Netlify dev pipeline and local replication of prod environment

## Prerequisites

- [Node and NPM](https://nodejs.org/)
- [Netlify CLI](https://www.npmjs.com/package/netlify-cli)


## Running locally

```bash

# install Netlify CLI globally
npm install netlify-cli -g

# install the project dependencies
npm install

# run the build and server locally
netlify dev
```


## Previewing the production build

When building for production, an extra build step will strip out all CSS classes not used in the site. This step is not performed during the automatic rebuilds which take place during dev.

```bash

# run the production build
npm run build
```


## Styling with TailwindCSS

This site uses TailwindCSS to offer utility CSS classes and provide a rapid means to styling the site. This means that most styling can be done without writing any additional CSS. Instead, utility classes can be added directly to the HTML. This may not be to everyone's tastes, but it can provide some very rapid development and also offer surprising levels of familiarity for those used to working in this way (since the conventions and classes are not _per site_.)

While running/developing locally, the `npm run start` command will recompile the site as files are saved and this includes the CSS pipeline from Tailwind.

### Global CSS utilities.

A small number of bespoke CSS rules are provided for efficiency of repeated or global classes. These reside in `src/site/_includes/css/tailwind.css`
