# DZGER
<!DOCTYPE html>
<html lang="fa" dir="rtl">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>دزدگیر اماکن</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="manifest" href="./manifest.webmanifest">
    <meta name="theme-color" content="#0891b2" />
    <style>
      body {
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
      }
    </style>
  <script type="importmap">
{
  "imports": {
    "react/": "https://esm.sh/react@^19.1.0/",
    "react": "https://esm.sh/react@^19.1.0",
    "react-dom/": "https://esm.sh/react-dom@^19.1.0/"
  }
}
</script>
<link rel="stylesheet" href="/index.css">
</head>
  <body class="bg-gray-900">
    <div id="root"></div>
    <script>
      if ('serviceWorker' in navigator) {
        window.addEventListener('load', () => {
          navigator.serviceWorker.register('./service-worker.js').then(registration => {
            console.log('ServiceWorker registration successful with scope: ', registration.scope);
          }, err => {
            console.log('ServiceWorker registration failed: ', err);
          });
        });
      }
    </script>
  <script type="module" src="/index.tsx"></script>
</body>
</html>
