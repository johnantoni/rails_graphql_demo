# Readme

### graphiql queries

##### create user

    mutation {
      createUser(input: {
        name: "joe",
        email: "joe@joe.com"
      }) {
        user {
          id
          name
          email
        } errors
      }
    }

##### get all users

    query{
      users {
        id
        name
        email
      }
    }

##### get user with id 1

    query{
      user(id: 1) {
        id
        name
        email
      }
    }


## setup

    bundle install
    bundle exec rails server

    cd frontend
    yarn install
    yarn start


## running

* rails graphiql = http://localhost:3000/graphiql
* apollo frontend = http://localhost:3001/

