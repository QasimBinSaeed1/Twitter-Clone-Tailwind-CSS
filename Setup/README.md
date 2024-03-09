# How to setup Tailwind CSS

## Step 1: Install tailwindcss via npm by running the following commands

``` 
npm install -D tailwindcss
npx tailwindcss init
```

## Step 2: Add the paths to all of your template files in your `tailwind.config.js` file. Update tailwind.conf.js file to include this line:
```
content: ["*.html"],
```
OR
```
 content: ["*.{html,js}"]
```

## Step 3: create src/input.css to include:
```
@tailwind base;
@tailwind components;
@tailwind utilities;
```

## Step 4: Include the src/output.css file to your html
```html
<link rel="stylesheet" href="./src/output.css">
```
## Step 5: Run the following command:
```
npx tailwindcss -i ./src/input.css -o ./src/output.css --watch
```