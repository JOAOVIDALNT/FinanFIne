## BACKEND
Design to be a mvc project, the idea is to avoid overengineering and embrace simplicity.

#### GOALS
- [ ] DEVELOP THE MVP
- [ ] COVER MVP WITH TESTS
- [ ] DEPLOY THE MVP INTO A CONTAINER WITH DOCKER
- [ ] DEPLOY THE MVP ON A CLOUD SERVICE


#### CONTROLLERS
##### BALANCE CONTROLLER
At balance controller, we should register, update and delete our incomes and expenses, for the MVP it's just what we have for an user.

##### USER CONTROLLER
At user controller, we should register, recover and authenticate our users.

#### ENTITIES
##### INCOME
- amount -> not null
- date -> not null
- installment -> not null (fix at one on mvp)
- bill -> nullable [entity] - if it's a credit card accout must have a bill
- due date (feature) -> not null [datetime] - default -> today
- paid (feature) -> not null [boolean]
- paid date -> nullable [datetime]
- category (feature) -> not null [entity] - going to have global a user categories
- account (feature)
- user (temporary) -> in the future we should associate incomes and expenses into the account
##### EXPENSE
- amount
- date
- installment
- bill
- due date (feature)
- paid (feature)
- category (feature)
- account (feature)
- user (temporary) -> in the future we should associate incomes and expenses into the account

##### USER
- 