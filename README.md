# react-fashion-commerce

React storefront for a fashion catalogue - browse products, manage a cart, and
check out. Redux holds cart and product state.

## Stack

- React 18
- Redux for cart and product state
- Bootstrap / CSS for layout
- `estoreserver/` - a small Node/Express service backing the app
- Feature flags via `flags.yaml`

## Layout

```
src/            React app - components, store, pages
public/         static assets
estoreserver/   backing service
flags.yaml      feature flags
```

## Run it

Front end:

```
npm install
npm start
```

Backing service:

```
cd estoreserver
npm install
npm start
```

Create `.env` with:

```
REACT_APP_API_URL=http://localhost:4000
```

## Notes

- Work in progress - not every flow is finished.
- `REACT_APP_API_URL` is read at build time, so restart the dev server after
  changing it.
