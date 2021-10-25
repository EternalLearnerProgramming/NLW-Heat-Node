# NLW Heat Node

> Project developed at the Next Level Week Heat event organized by Rocketseat. This project aims to build the backend of an application to send comments. Applied technologies: NodeJS, TypeScript, Prisma ORM and Socket.io.

<br/>

## Requirements

Before starting, make sure you have met the following requirements:
* Node version 14.17.6 or greater;
* Yarn or NPM;
* Git.

<br/>

## How to Run

To run the project, follow these steps:

Go to the directory where you want to clone the project and run:
```
git clone https://github.com/alaodev/nlw-heat-node.git
```

Then: 
```
cd nlw-heat-node
```

Now:
```
yarn or npm i // To install de dependencies.
```

To create the database schemas, run the command and then give a name to your migration:
```
yarn prisma migrate dev or npm prisma migrate dev
```

Finally, execute:
```
yarn dev or npm run dev
```

By default, the aplication will run on port 3000. If you want, you can change the port accessing the file /src/server.ts:
```js
import { serverHttp } from "./app";

const PORT = 3000;

serverHttp.listen(PORT, () => console.log(`Server is running on PORT ${PORT}`));
```
