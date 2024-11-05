# create commands

```angular2html
npm init
```

to create packge.json file

https://tailwindcss.com/docs/installation

```angular2html
npm install -D tailwindcss
```

added package-lock.json & node_modules

```
npx tailwindcss init
```

added tailwind.config.json
initialize tailwind (tailwind configs)

Add the paths to all of your template files in your tailwind.config.js file.

```angular2html
 content: ["./src/**/*.{html,js}"],
```

All the files with these extensions can use tailwind

```angular2html
  content: ["./*.html"],
```

یعنی هر فایلی در روت پروژه با پسوند html

create input.css file -> tailwind main config
to use tailwind classes

به جای src در روت پروژه ایجاد شده این فایل

run tailwind

```angular2html
npx tailwindcss -i ./src/input.css -o ./src/output.css --watch
```

به جای ران کردن مستقیم این کامند این قسمت رو به package.json اضافه میکنیم

```angular2html
  "scripts": {
        "watch" : "npx tailwindcss -i ./input.css -o ./css/style.css --watch"
},
```

this command runs the input.css file using -i flag
then create the output.css file using -o flag
using command --watch : after every save above commands will run

```angular2html
npm run watch
```