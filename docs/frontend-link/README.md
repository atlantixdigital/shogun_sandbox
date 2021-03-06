### frontend-link

`frontend-link` exports `Link` component that is just a wrapper around `a` element, but does client routing and few more optimizations like prefetching of pages.

Example usage:

```jsx
import { Link } from 'frontend-link'

const ExampleComponent = () => (
  <Link
    href="/about-us"
    className="my-class-name"
    replace // if we want to replace last entry in browser history instead of pushing new entry into a stack
    external // to render component as `<a>` tag and open it in new tab
  >
    About us Page
  </Link>
)
```
