[JSON documentation](https://github.com/typicode/json-server)

## Package
npm init

## Json server
>npm install -g json-server(the first time you do it)\
>npm install --save json -server


### Starting the JSON server
[json-server --watch db.json](https://github.com/typicode/json-server)\
Replace your test sccript in package.json to "json:server": `json-server --watch db.json`

- Create a new file - db.json


## Errors
[![Image from Gyazo](https://i.gyazo.com/a17c5fb8cd21a6900bc681496c5bf4b8.png)](https://gyazo.com/a17c5fb8cd21a6900bc681496c5bf4b8)

<u>What solved it</u>\
[Stack overflow](https://stackoverflow.com/questions/25290986/how-to-fix-eacces-issues-with-npm-install)

```
sudo chown -R `whoami` ~/.npm
sudo chown -R `whoami` /usr/local/lib/node_modules
```

>npm run json:server\
(jso:server is from script- package.json)

## GET SINGLE USER
>http://localhost:3000/users/1
>(With 1 being the id)
<br>
## GET ALL USERS 
>http://localhost:3000/users

## FILTER COMPANY BY NAME
>http://localhost:3000/companies?name=Contact\
>http://localhost:3000/companies?name=Contact&name=DXC

## PAGINATION & LIMIT
>http://localhost:3000/companies?_page=1&_limit=2

## SORTING
>http://localhost:3000/companies?_sort=name&_order=asc
(can also have desc)

## USERS AGE RANGE(NUMBERICAL)
>http://localhost:3000/user?age_gte=17\
(get= greater than or equal)\
>http://localhost:3000/user?age_gte=30&age_lte=50

## FULL SEARCH
>http://localhost:3000/user?q=Lisa
