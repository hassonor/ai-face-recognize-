
Face Recognize with React,Node,Clarifai,postgresql

![Twitter](https://github.com/hassonor/react-robots/blob/master/demo.png)

1. Clone this repo
2. Run `npm install` both FE and BE.
3. You must add your own API key in the `controllers/image.js` file to connect to Clarifai API KEY
You can grab Clarifai API key [here](https://www.clarifai.com/)
4. Install postgresql and CREATE DB
5. CREATE TABLE users (
   id serial PRIMARY KEY,
   name VARCHAR(100),
   email text UNIQUE NOT NULL,
   entries BIGINT DEFAULT 0,
   joined TIMESTAMP NOT NULL
   );
6. CREATE TABLE login (
   id serial PRIMARY KEY,
   hash varchar(100) NOT NULL,
   email text UNIQUE NOT NULL
   )
7. Update .env.process variables
8. Run `npm start` both FE and BE.
