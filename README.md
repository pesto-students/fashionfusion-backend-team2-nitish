
# Fashion Fusion REST API
This is a REST API built using Node.js and Express.js for eCommerce. It provides endpoints for user authentication, product management,and order management.


## Features

- User registration
- User login and logout
- Product creation, update, deletion, and retrieval
- Order creation, update, deletion, and retrieval
- Image upload for products
- JWT-based authentication

## Tech Stack
**Backend:**
- Node.js
- Express.js
- MongoDB
- Mongoose
- JWT

**Image Upload:** 
- Cloudinary API

**Data Storage:** 
- MongoDB

**User Authentication:**
- JSON Web Tokens (JWT)
## API Reference

#### User Authentication
- `POST /api/v1/auth/register` -              Register a new user.
- `POST /api/v1/auth/login` -                 Login with an existing user.
- `PUT /api/v1/auth/profile` -                Update user profile
-`POST /api/v1/auth/forgot-password` -        User can create new password with required details.

#### Products
- `POST /api/v1/product/create-product` -           Admin can create the product.
- `PUT /api/v1/product/update-product/:pid` -       Admin can update a particular product.
- `DELETE /api/v1/product/delete-product/:pid`-     Admin can delete a particular product.
- `GET /api/v1/product/get-product` -               Get products.
- `GET /api/v1/product/get-product/:slug` -         Get a single product.
- `POST /api/v1/product/product-filters` -          Filter product.
- `GET /api/v1/product/product-count` -             Get product count.
- `GET /api/v1/product/product-list/:page` -        Get product per page.
- `GET /api/v1/product/search/:keyword` -           Search Product.
- `GET /api/v1/product/related-product/:pid/:cid`-  Get similiar products.
- `GET /api/v1/product/product-category/:slug` -    Get category-wise products.

#### Category 
- `POST /api/v1/category/create-category` -       Create category.
- `PUT /api/v1/category/update-category/:id` -    Update category.
- `GET /api/v1/category/get-category` -           Get all category.
- `GET /api/v1/category/single-category/:slug` -  Get single category.
- `DELETE /api/v1/category/delete-category/:id` - Delete category.

#### Order
- `GET /api/v1/auth/orders` -                 Get Orders
- `GET /api/v1/auth/all-orders` -             Get All orders
- `PUT /api/v1/auth/order-status/:orderId`-   Update Order Status           



## Installation


1. Clone the repository.


```
git clone https://github.com/pesto-students/fashionfusion-backend-team2-nitish
```
2. Install the dependencies.

```
npm install 
```

3. Set the environment variables in a .env file in the root directory of the project. 
Example:
```
PORT=5000
MONGO_URL=mongodb://localhost/ecommerce
JWT_SECRET=your_secret_key_here
JWT_LIFETIME=1d

```

5. Start the application.

```
npm run dev

```
## Feedback

Please let us know your thoughts on my app by sending any suggestions or feedback to kumaravishek2015@gmail.com.
