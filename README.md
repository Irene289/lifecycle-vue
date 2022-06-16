# lifecycle-vue
I build this project to understand more about the [Lifecycle Hooks](https://v2.vuejs.org/v2/guide/instance.html#Lifecycle-Diagram) of Vue. 

Here's the DOM structure:
```html
<header>
  <nav>
  </nav>
</header>
```
Here's what the DOM be going through:
1. beforeCreate header
2. created header
3. beforeMount header
4. beforeCreate nav
5. created nav
6. beforeMount nav
7. mounted nav
8. mounted header
9. beforeUpdate header/nav (if there're any updates)
10. updated header/nav (if there're any updates)
11. beforeDestroy header
12. beforeDestroy nav
13. destroyed nav
14. destroyed header

To know better about this project, please click:
[DEMO](https://irene289.github.io/lifecycle-vue/)


## Project setup
Git clone this project
```
git clone https://github.com/Irene289/lifecycle-vue.git
```
Install
```
npm i
```
Compiles and hot-reloads for development
```
npm run serve
```

## Tools
1. Vue: 2.6.11
2. Vue CLI: 4.1.1
