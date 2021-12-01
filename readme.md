Tailwind simple starter steps
1. Make a new folder and cd into it then run ```git init```. Add a ```.gitignore``` file and add ```node_modules``` as text to the top of the file
2. Run command ```npm init -y``` and replace the script section in the ```packag.json``` file this command makes with the below piece of code
```
  "scripts": {
    "dev": "vite"
  },
```
3. Run ```npm install -D tailwindcss@latest postcss@latest autoprefixer@latest vite```
4. Run ```npx tailwindcss init -p```
5. Make a new file styles.css file  ```touch styles.css```
6. Add below css to ```styles.css```
```
@tailwind base;
@tailwind components;
@tailwind utilities;
```
7. Make a index.html file ```touch index.html```
8. Add below HTML to index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>Document</title>
</head>
<body>
    <h1 class="text-4xl font-bold text-center text-blue-500">header 2</h1>
</body>
</html>
```
9. Run ```npm run dev```
10. Open browser at ```http://localhost:3000/```