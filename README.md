Name: Harsh Verma (210415)
University: IIT Kanpur
Department: Economic Sciences





## 🏁 Installation

### 📦 Using Docker (recommended)

To run the project, follow these steps:

1. Install [Docker](https://www.docker.com/) on your machine.
2. Clone the project repository.
3. Navigate to the project directory.
4. Create `.env` file in the root folder and copy paste the content of `.env.sample`, and add necessary credentials.
5. Run the Docker Compose command:

```bash
docker-compose up --build --attach backend

# --build: Rebuild the image and run the containers
# --attach: only show logs of Node app container and not mongodb
```

6. Access the project APIs at the specified endpoints.

### 💻 Running locally

To run the project locally, follow these steps:

1. Install [Yarn](https://yarnpkg.com/), [NodeJs](https://www.nodejs.org/), [MongoDB](https://www.mongodb.com) and [MongoDB Compass (optional)](https://www.mongodb.com/products/compass) on your machine.
2. Clone the project repository.
3. Navigate to the project directory.
4. Create `.env` file in the root folder and copy paste the content of `.env.sample`, and add necessary credentials.
5. Install the packages:

```bash
yarn install
```

6. Run the project:

```bash
yarn start
```

7. Access the project APIs at the specified endpoints.

### 🚄 Using Railway (One-click Deploy)

To self-host the application, you can take advantage of a pre-built template that is readily available.

[![Deploy ](https://railway.app/button.svg)](https://railway.app/template/B2f7Hq)

1. Click the button above to visit railway.app.

2. Click on the **Deploy Now** button.

3. (Optional) Sign in with GitHub to deploy.

4. Fill in the Repository details:

   - Specify the repo name.
   - Checkmark for Public/Private repository.

5. For Environment variables, we have provided some default values in the `ENV` to reduce the burden, but some parameters are mandatory:

   - `PORT`: Do not change the value, let it be set to 8080 to view the swagger docs after deployment.
   - `MONGODB_URI`: Provide the MongoDB Atlas database URL. An example is prefilled for you, edit/update it to continue.
   - `NODE_ENV`: Default set to 'development' to view the logs. You may choose to change it to any other value such as 'prod' to hide them.
   - `EXPRESS_SESSION_SECRET`: It is advised to change the default value to your own secret value.
   - `ACCESS_TOKEN_SECRET`: It is advised to change the default value to your own secret value.
   - `ACCESS_TOKEN_EXPIRY`: Set to 1 day as default.
   - `REFRESH_TOKEN_SECRET`: It is advised to change the default value to your own secret value.
   - `REFRESH_TOKEN_EXPIRY`: Set to 10 days as default.

6. Once you fill in the required environment parameters, if you choose to add others such as PayPal, Google, and Razorpay, please proceed to mention your credentials in the form.

7. Click on the **Deploy** button to trigger the first build.
   - Monitor the server logs; if you come across any deployment problems, feel free to raise an issue for me to look into.

Note: Once the application is deployed, please wait for 3-5 minutes for the swagger docs to be available.

# 📜 Swagger Docs

[Swagger Docs](http://localhost:8080): http://localhost:8080
