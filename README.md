כמובן! הנה גרסה של ההוראות כקובץ README:

```markdown
# How to Run the Application

## 1. Initialize Services

Open the project terminal and run the following command to initialize the necessary services:

```bash
docker-compose up -d
```

This will set up Redis, MongoDB, and Cassandra. The application will not function without these services.

## 2. Run the Application

Once the services are successfully initialized, launch the application using your preferred Integrated Development Environment (IDE).

## 3. Access Swagger UI

To visualize the backend APIs, open your web browser and navigate to:

```
http://localhost:8080/swagger-ui.html
```

This will bring up the Swagger UI interface where you can interact with the available endpoints.

---

# How to Use the Application

## 1. Access User Creation

In Swagger UI, find the **app-controller** section.

### 2. Create a User

- Open the `POST` endpoint for `/user`.
- Enter a name in the provided field.
- Click **Try it out**.

If the user is successfully created, you should receive a **200 OK** response.

---

## 3. Shorten a URL

- Navigate to the `POST` endpoint for `/tiny`.
- Click on the example value (the yellow window on the right) to autofill the required fields:
  - **longUrl**: For example, `https://www.google.com`
  - **userName**: Use the name you created earlier.
- Click **Try it out** to submit the request.

You should receive a shortened link in the response. Clicking on this shortened link will redirect you to the original URL.

---

## 4. View User Information

You can find the users you've created and see which URLs they’ve shortened, along with the number of clicks each shortened link has received.
```

העתק את הקוד הזה ושמור אותו כקובץ `README.md` במאגר שלך.
