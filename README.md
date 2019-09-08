# Readme

### graphiql queries

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


    query{
      users {
        id
        name
        email
      }
    }



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

