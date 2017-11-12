# potluck


A potluck application: allow guests to 
1. Add a dish the guest wish to bring to the potluck. 
2. Search dishes in the dish list.   
3. Display all dishes for the potluck

Experience this app live on Heroku: https://potluch-dishes.herokuapp.com


IPO diagram for the Potluck App

| Input                                 | Processing                                                      | Output                                           |
| ------------------------------------- | --------------------------------------------------------------- | ------------------------------------------------ |
|                                       |                                                                 | welcome page, prompt user to choose              |
| choose add a dish                     | go to route "/adish"                                            |                                                  |
|  --add first name, last name and dish | get first name, last name and dish (post method)                | display addition result on HTML                  |
|                                       | If validation has errors, go back to "/adish"                   |                                                  |
| choose search by a dish               | go to route "/searchdish"                                       |                                                  |
| --enter a dish name                   | get dish name, search such dish in database, and return result  | display dish searched result on HTML             |
|                                       | If no match, return no match message                            |                                                  |
| choose search by a chef               | go to route "/searchchef"                                       |                                                  |
| --enter a chef name                   | get chef name, search such chef in database, and return result  | display chef searched result on HTML             |
|                                       | If no match, return no match message                            |                                                  |
| choose display all dishes/chefs       | go to route "/displayall"                                       |                                                  |
|                                       | search all records in the database                              | display all dishes/chefs in the database on HTML |
|                                       |                                                                 |                                                  |
