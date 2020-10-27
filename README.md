# yellowHEAD Interview Assignments

Please follow these rules when working on **yellowHead** coding assignment:

- Candidates have 2 hours to complete the assignment.  
The time is measured from the time the email containing the assignment is sent.
- You can submit the assignment by sending a github link, to the same mail you got the assignment from.  
The github repository link you send should contain you solution.
- If you have any questions about the assignment, please send them to the following email: `yariv@nerdeez.com`

## Node Assignment


### Technologies you **HAVE** to use

During this assignment you have to use the following libraries to complete the assignments:

- [Node.js](https://nodejs.org/)
- [express.js](https://expressjs.com/)
- [Typescript](https://www.typescriptlang.org/)
- [TypeORM](https://typeorm.io/#/)
- [Apollo Server](https://www.apollographql.com/docs/apollo-server/)

Feel free to use any additional libraries of your choice, but the ones above are obligatory

- Create a new express backend application
- Your server should connect using `TypeORM` to a sqlite database
- Create a new table class `todo` that table will contain 3 columns:
  - id - primary key
  - title - string (varchar)
  - description - string (varchar)
- create a `GraphQL` query for getting all the rows of the `todo` table

```
query {
	getTodos {
		id
		title
		description
	}
}
```

- create a `GraphQL` mutation to create a new row in the table

```
mutation {
	addTodo(title: "new todo", description: "some description") {
		id
		title
		description
	}
}
```

- create tests for your API


