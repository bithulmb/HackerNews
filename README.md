# Django + GraphQL Learning Project

**GraphQL** using **Graphene-Django**. 
This repository contains a Django project built for learning and experimenting with GraphQL, following the tutorials and concepts from howtographql.com. It serves as a practical application of GraphQL principles integrated with a Django backend, demonstrating how to set up a GraphQL API, define schemas, and resolve queries and mutations.
---

## 🚀 Features

* Django project setup
* Integration of GraphQL using Graphene
* Sample queries and mutations
* Django admin for model management
* SQLite as the database for ease of use

---

## 🛠️ Tech Stack

* Python 3.x
* Django
* Graphene-Django
* SQLite (default database)

---

## 📦 Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/bithulmb/python-graphql.git
   cd python-graphql
   ```

2. **Create a virtual environment and activate it:**

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

4. **Apply migrations and create a superuser:**

   ```bash
   python manage.py migrate
   python manage.py createsuperuser
   ```

5. **Run the development server:**

   ```bash
   python manage.py runserver
   ```

6. **Access the GraphQL Playground:**

   Visit [http://localhost:8000/graphql/](http://localhost:8000/graphql/) to test queries and mutations.

---


---

## 🧪 Example GraphQL Queries

### Query:

```graphql
query {
  users {
    id
    username
    email
  }
}
```

### Mutation:

```graphql
mutation {
  createUser(username: "john", email: "john@example.com", password: "test1234") {
    user {
      id
      username
    }
  }
}
```

---

## 📝 License

This project is open for learning and experimentation. Use it freely for educational purposes.

---

## 🙌 Acknowledgements

* [Graphene-Django Documentation](https://docs.graphene-python.org/projects/django/en/latest/)
* [Django Documentation](https://docs.djangoproject.com/)
* [GraphQL Official Site](https://graphql.org/learn/)
