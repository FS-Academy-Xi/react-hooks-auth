# API Auth for Single Page Applications

## Session-Based Auth vs Token-Based Auth

Implementing authorization and authentication into a full-stack application is a
challenging process that will test your knowledge of frontend and backend code.
If you decide you need to implement auth for your project, make sure you have a
good understanding of the workflow, and work on implementing auth in a smaller
project to get practice.

The two labs linked in this section discuss two alternative approaches to auth:

- Session-based auth relies on Rails built-in session mechanism, similar to
  handling auth in Phase 2 Rails. Since it relies on **cookies**, session-based
  auth isn't a good choice for React Native projects.
- JWT auth introduces a new technology, JSON Web Tokens, to handle
  authentication between the client and server. JWT auth does not rely on
  cookies, so it's a better choice for React Native projects. However, tokens
  need to be stored somewhere, and traditional options (`localStorage` or
  `sessionStorage`) are not secure - they can be accessed by XSS attacks.

Based on your project's needs, and your comfort level with auth in Rails, choose
the strategy that is right for you!

## Resources

- https://scotch.io/tutorials/the-ins-and-outs-of-token-based-authentication
- https://stackoverflow.com/questions/35291573/csrf-protection-with-json-web-tokens/35347022#35347022
- https://www.thegreatcodeadventure.com/jwt-storage-in-rails-the-right-way/
- https://pragmaticstudio.com/tutorials/rails-session-cookies-for-api-authentication
