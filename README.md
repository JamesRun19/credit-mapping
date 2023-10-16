# create-svelte

Everything you need to build a Svelte project, powered by [`create-svelte`](https://github.com/sveltejs/kit/tree/master/packages/create-svelte).

## Creating a project

If you're seeing this, you've probably already done this step. Congrats!

```bash
# create a new project in the current directory
npm create svelte@latest

# create a new project in my-app
npm create svelte@latest my-app
```

## Developing

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```bash
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

## Building

To create a production version of your app:

```bash
npm run build
```

You can preview the production build with `npm run preview`.

> To deploy your app, you may need to install an [adapter](https://kit.svelte.dev/docs/adapters) for your target environment.

## Installing/configuring the Project locally

The following Python Libraries must be installed before running the app:

```bash
pip install Flask flask_cors PyPDF2 sentence-transformers nltk
```

The database must be running on a server and configured in the /src/lib/db.ts file:

```bash
import postgres from 'postgres';
export const sql = postgres({
    host: 'localhost',
    database: 'creditmap_db',
    port: 5432
});
```

To run the app, type in the terminal:
```bash
npm run dev
```

Once running, we must start the flask server:
Run the file - backend/app.py

The application should now be running on: http://localhost:5173/


