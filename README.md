# Mary Gold Coins
Frok [Sunappu-Dojo/burokku](https://github.com/Sunappu-Dojo/burokku)
![image](https://user-images.githubusercontent.com/89796393/214847043-4b381253-70ed-43a7-ab91-e7280e78c3c4.png)
## Building the app

The app is in `/src`. Assets called by the app needs to be compiled using some front-end tooling, detailed below.

### Development

1. Duplicate `.env.example` to `.env` and edit it.
2. Run `npm install` (Node > 12.13) to install all the required packages and tools.
3. Run `npm run dev` and open the URL returned by the CLI.

Note: the Service Worker is broken while developing. Ignore it and check it using the [production](#production) mode.

### Production

1. Duplicate `.env.example` to `.env` and edit it.
2. Run `npm install` (Node > 14.18) to install all the required packages and tools.
3. Run `npm run build` to compile the app. The compiled app goes in `/public`.
4. Run `npm run preview` to preview it on your machine.

### Various

- Files in `/src/public` are copied as is (respecting the directory structure in `/src/public`) in the build directory.
- Lint JavaScript: `npm run lint` to scan for errors or `npm run lint-fix` to try an automatic fix.

