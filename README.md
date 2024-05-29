The cleanest barebones setup for React I found with ParcelJS.

```
npm install -g parcel-bundler
```

Just initialize vanilla JS project with:

```
npm init -y
```

Install react and react-dom:

```
npm install react react-dom
```

Install:

```
npm install --save-dev @types/react @types/react-dom typescript
```

and configure typescript with `tsconfig.json`:

```
{
  "compilerOptions": {
    "esModuleInterop": true,
    "jsx": "react"
  }
}
```

The above is required, so the following import would work:

```
import React from "react";
```

Finally add basic scaffolding with `index.html`, `index.tsx` and `components/App.tsx`.

Run with:

```
parcel ./src/index.html
```