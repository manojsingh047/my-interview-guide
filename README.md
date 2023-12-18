# my-interview-guide - frontend

Problem Solving - https://github.com/manojsingh047/DSnA/blob/master/patterns.md

## Browser and JS Concepts
- Run over this youtube series to quickly brush-up JS concepts - https://www.youtube.com/playlist?list=PLlasXeu85E9cQ32gLCvAvr9vNaUccPVNP
- For browser and JS - https://www.youtube.com/playlist?list=PLNYkxOF6rcIAKIQFsNbV0JDws_G_bnNo9

## JS Polyfills :
- bind, apply, call
- filter, map, reduce
- promise - https://medium.com/@manojsingh047/polyfill-for-javascript-promise-81053b284e37
- Run promises in sequence - https://gist.github.com/manojsingh047/b891472954ae276daa86f5a880b48a50
  

## Security and vulnerability
- https://medium.com/@manojsingh047/understanding-frontend-security-ff6585395534

## Accessibility
-https://www.youtube.com/watch?v=jCLhYRRNF2E&list=WL&index=2&ab_channel=ReactConferencesbyGitNation
(HTML5 Semantic elements for screen readers, Keyboard navigation for the app, color combination especially saturation level, drag and drop using keyboard)

## Performance and Optimizations
- https://medium.com/@manojsingh047/light-weight-websites-98a79249035
- https://www.youtube.com/watch?v=k-A2VfuUROg&ab_channel=GoogleChromeDevelopers
- https://bitsofco.de/web-performance-metrics-cheatsheet/
- https://dev.to/wgolledge/an-overview-of-performance-in-javascript-applications-2obb

###
Network Perf
- Compression - Gzip, Brotli
- Image / Video optimization 
  - webp 
  - video on loop instead of GIF
  - serve images using srcset for different screen devices
  - sprite images
  
- CDNs for static content
- Adaptive serving based on user bandwidth
- Caching - static content caching using http header SWR

Bundling
- Minification
- Tree Shaking
- Code splitting for lazy loading of JS
- https://slides.com/lucianomammino/unbundling-the-javascript-module-bundler-dublinjs
- https://www.youtube.com/watch?v=w8uxbpdjor0&ab_channel=DublinJS

JS Perf
- async, defer attributes for scripts loading
- heavy work on web worker
  
Rendering Perf
- Critical rendering path
- Follow PRPL Pattern for faster FCP
    - Push most critical content first - lazy loading, http2 push,
    - Render the initial route asap 
        - deliver critical css js inline
        - avoid render blocking js
        - SSR for initial load
    - Preload / Prefetch the next set of content - Resource prioritization using rel=preload, prefetch tags
    - Lazy load other route and content - use service worker

- RAIL Model

## Detecting Memory Leaks
- https://www.youtube.com/watch?v=YDU_3WdfkxA&ab_channel=GoogleChromeDevelopers

## Authentication
```to be added```
- SAML, OIDC
- session, jwt

## Design guide:
- general guide - https://www.youtube.com/watch?v=5llb2fGKl9s&t=2137s&ab_channel=JSerJSer
- netflix - https://www.youtube.com/watch?v=Tu-hZ6lqNtY&t=23s
- instagram - https://www.youtube.com/watch?v=LCnkSLRJRwM&ab_channel=JSer
- messenger - https://www.youtube.com/watch?v=utWopFyY5cE&ab_channel=JSerJSer
- progress bar - https://www.youtube.com/watch?v=21ZgaFSRc_4&ab_channel=JSer
- youtube - https://www.youtube.com/watch?v=x9NgcwwFp7s&list=WL&index=3&t=2324s&ab_channel=WebDevInterview
- chat app - https://www.youtube.com/watch?v=LEaiGjffLEs&ab_channel=Front-EndEngineer
  
    #Common Patterns (F N D A C) 
    - Functional (Features)
    - Component Architecture (Screens for the functional requirements) - tree of components hierarchy can be drawn and create simple box model  
    - Api design (including all meta data like headers etc)
        1. List down all the REST endpoints with HTTP methods, and request payload
    - Data entities using typescript types notation
    - Non-Functional requirements
        1. Optimizations - Network perf, rendering perf, JS perf
        2. Good UX
        3. Localization
        4. Logging 
        5. Accessibility
        6. Authentication / Authorization
        7. PWA
        8. Security
        9. CI / CD
        10. Analytics


## Coding Principles
- SOLID in JS - https://www.youtube.com/watch?v=UQqY3_6Epbg&list=PLZlA0Gpn_vH9kocFX7R7BAe_CvvOCO_p9&index=1&ab_channel=WebDevSimplified

## Design Patterns
- Factory, Builder - https://www.youtube.com/watch?v=-1YhP5IOBCI&t=549s&ab_channel=JackHerrington
- Visitor, Iterator - https://www.youtube.com/watch?v=SZ2kAkMdAZE&ab_channel=JackHerrington
- State Pattern - https://www.youtube.com/watch?v=yZt7mUVDijU
- Command & Memento Patterns - https://www.youtube.com/watch?v=H2kxc_ZrSPI&t=1149s&ab_channel=JackHerrington
- Memento - https://www.youtube.com/watch?v=0eOMPadRNmI&list=WL&index=23&ab_channel=JohnLindquist
 
## Advanced Topics:
- Critical rendering path
- Streaming SSR - https://www.youtube.com/watch?v=o3JWb04DRIs
- Module Federation
- Shadow DOM
- Apollo GraphQL federation
- Error logging


