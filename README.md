# UseCookie doesn't work after an await

Look at the [Nuxt 3 documentation](https://nuxt.com/docs/getting-started/introduction) to learn more.

## Error
Using `useCookie` after an await doens't work despite the fact that feature is available `experimental { asyncContext: true }`

Error message
```
error Error: [nuxt] A composable that requires access to the Nuxt instance was called outside of a plugin, Nuxt hook, Nuxt middleware, or Vue setup function. This is probably not a Nuxt bug. Find out more at `https://nuxt.com/docs/guide/concepts/auto-imports#using-vue-and-nuxt-composables`.
    at createError (index.mjs?v=164b9a79:78:15)
    at createError (error.js?v=164b9a79:31:16)
    at NuxtError (revive-payload.client.js?v=164b9a79:9:24)
    at hydrate (parse.js?v=164b9a79:60:32)
    at hydrate (parse.js?v=164b9a79:125:19)
    at hydrate (parse.js?v=164b9a79:125:19)
    at hydrate (parse.js?v=164b9a79:60:40)
    at unflatten (parse.js?v=164b9a79:132:9)
    at parse (parse.js?v=164b9a79:16:9)
    at parsePayload (payload.js?v=164b9a79:106:10)
```

## Setup

Make sure to install the dependencies:

```bash
# npm
npm install
```

## Development Server

Start the development server on `http://localhost:3000`:

```bash
# npm
npm run dev
```

## Production

Build the application for production:

```bash
# npm
npm run build
```

Locally preview production build:

```bash
# npm
npm run preview
```

Check out the [deployment documentation](https://nuxt.com/docs/getting-started/deployment) for more information.
