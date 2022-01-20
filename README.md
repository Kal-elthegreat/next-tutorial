# next-tutorial

notes to self:

**Setup**
- create app w/ `npx create-next-app <app-name>`
- `npm run dev` to spin up localhost


**Navigation**
- all directories created in `pages` directory will create a new route. ie. `/pages/newRoute/index.js`
- use `Link` from `/next/link` to navigate between pages
- be sure to hoist `href` from <a> into parent <Link>
- classes/attr should be added to <a> and not <link>

**Assets**
- can add assets to `public` directory
- `Image` from `next/image` component handles optimization inherently. Lazt loaded by default
- `Head` component handles metadata like `title`
- `Script` from `next/script` to use 3rd part js. Takes a `strategy` prop and `onLoad` prop. May be others. See documentation
- CSS styling support for: css, sass, css modules, styled jsx (styling done in the js), and others
- Global styling, can create the file anywhere but can only import styling in `/pages/_app.js`
- `/pages/_app.js` is a top level component common across all pages, can be used to keep state when navigating pages
- *be sure to restart dev once you add `/pages/_app.js`*
  
