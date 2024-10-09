# About Project

Next.js project with Tauri to packge to app

## Getting Started

git the repo 

```bash
git clone https://github.com/ASouwn/tauri-next-app-example.git your-project-name
```

rewrite the `package.json` file and `src-tauri/tauri.config.ts` file

```json
{
  "name": "tauri-next-app-hello-world", // change this name to your project name
  "version": "0.1.0",
  "private": true,
  "scripts": {
    ...
  },
  "dependencies": {
    ...
    "tauri-next-app-hello-world": "file:" // replace this line too
  },
  ...
}
```

```json
{
  "$schema": "../node_modules/@tauri-apps/cli/config.schema.json",
  "productName": "tauri-next-app-hello-world", // change this name
  "version": "0.1.0",
  "identifier": "com.asouwn.tauri-next-app-hello-world", // change this identifier
  ...
  },
  "app": {
    "windows": [
      {
        "title": "tauri-next-app-hello-world", // change this title
        ...
      }
    ],
    "security": {
      "csp": null
    }
  },
}
```

Then run the following command

```bash
npm install

npm run tauri dev

# to get the .exe file
npm run tauri build
```

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

