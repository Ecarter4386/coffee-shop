#Making CoffeeShop

first: generate a rails project and set it up for git github

```bash
rails new coffee_shop
cd coffee_shop
subl .
git init
git add .
git commit -m "first commit"
git remote add origin <url>
git push origin master

```
second: add Welcome page

```bash
rails g controller Welcome index

```

In config/routes.rb alter index route to  root welcome#index

In app/views/welcome/index.html.erb replace 

```html
Java chicory, black doppio and roast cream mocha turkish strong. Blue mountain doppio black, chicory, sugar medium, single shot a wings blue mountain turkish. Viennese et, cinnamon, turkish lungo qui cappuccino kopi-luwak. Black, dripper, to go medium espresso lungo in, and plunger pot latte sweet redeye. Half and half, galão, single shot wings beans bar that con panna macchiato dark foam galão.
```
Save to git and GitHub in terminal
```bash
git add .
git commit -m "added landing page"
git push origin master
```