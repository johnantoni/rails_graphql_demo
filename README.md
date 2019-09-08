# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...


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
