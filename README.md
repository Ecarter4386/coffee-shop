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

### Third: Add Drinks

```bash
rails g scaffold Drink name:string size:integer price:decimal
rails db:migrate
rails s
```

(in class our database messed up because we had a property called type which is reserved. we had to commit the changes to a new git branch and then go back to the master to fix it. messed with migrations to fix the database)
In browser, go to http://0.0.0.0:3000/drinks to add several drinks to the database.

Save to git and github in terminal


```bash
git add .
git commit -m "added drinks scaffold"
git push origin master
```








