# Data_Table

### Step-by-Step Explanation

#### 1. Set Up a New React.js Project Using Vite

1. **Initialize the Vite Project:**
   - Open your terminal and navigate to the directory where you want to create your project.
   - Run the following command to create a new Vite project:

     ```bash
     npm create vite@latest my-vite-react-app --template react
     ```

2. **Navigate to the Project Directory:**
   ```bash
   cd my-vite-react-app
   ```

3. **Install Project Dependencies:**
   - Install necessary dependencies for your project:

     ```bash
     npm install
     ```

#### 2. Install Axios and JSON Server

- Install Axios for making HTTP requests and JSON Server for creating a mock API:

  ```bash
  npm install axios json-server
  ```

#### 3. Create Components

- **ProductList:** This component will display a list of products. It will implement features like sorting, searching, pagination, and filtering.

- **ProductDetails:** This component will show detailed information about a specific product.

- **AddProduct:** This component will allow users to add new products to the system.

- **EditProduct:** This component will enable users to edit existing product details.

- **DeleteProduct:** This component will provide functionality to delete a product from the system.

#### 4. Set Up JSON Server

- **Create `db.json`:**
  - In the root directory of your project, create a `db.json` file with sample product data. For example:

    ```json
    {
      "products": [
        { "id": 1, "name": "Product 1", "price": 100 },
        { "id": 2, "name": "Product 2", "price": 200 }
      ]
    }
    ```

- **Run JSON Server:**
  - Start the JSON Server to serve the API on a local port:

    ```bash
    json-server --watch db.json --port 8000
    ```

#### 5. Implement Axios Requests in React Components

- **Fetch Products in `ProductList`:**
  - Use Axios to fetch a list of products from the JSON Server API.
  - Implement sorting, searching, pagination, and filtering logic on the client-side.

- **CRUD Operations:**
  - Handle create (POST), read (GET), update (PUT/PATCH), and delete (DELETE) operations using Axios in the respective components.

#### 6. Design the UI

- **Styling:**
  - Design the UI for each component using CSS or a CSS framework like Bootstrap.

### Summary

1. **Initialize a Vite React project.**
2. **Install necessary dependencies** including Axios and JSON Server.
3. **Create essential components**: `ProductList`, `ProductDetails`, `AddProduct`, `EditProduct`, and `DeleteProduct`.
4. **Set up JSON Server** with a `db.json` file and run it to serve a mock API.
5. **Implement Axios requests** in the React components to handle CRUD operations and additional features like sorting and searching.
6. **Design the UI** using CSS or a CSS framework.

