# GO, GraphQL

Categories and Courses relation GraphQL working playground

---

## Prepare

1. Clone repository:
    ```
    git clone https://github.com/wandersonsangreal/go-graphql
    ```
2. GO Version

    ```
    go version: 1.24
    ```

3. Install dependencies

    ```
     go mod tidy
    ```

4. Create .db file and tables

    ```
    touch database/data.db
    ```

    ```
    sqlite3 database/data.db
    ```

    ```
     > create table categories (id string, name string, description string);
    ```

    ```
     > create table courses (id string, name string, description string, category_id string);
    ```

    Run:

    ```
    go run cmd/server/server.go
    ```

4. Access:
    ```
    http://localhost:8080
    ```
