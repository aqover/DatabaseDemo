# express-mysql-boilerplate

This repository is a boilerplate for Typescript express application with mysql backend.

## Requirement
* Nodejs
* MySQL

## Quick Start
#### 1. Clone this repository
`$ git clone https://github.com/Pepewitch/express-mysql-boilerplate.git`
#### 2. Enter the directory
`$ cd express-mysql-boilerplate`
#### 3. Install packages
Either npm or yarn is okay. Choose one.

`$ npm install` or `$ yarn`
#### 4. Setup database
- Copy any files with `.example` namespace
- Edit those files with your own data
```
// ormconfig.example.json
{
  "type": "mysql",
  "host": "localhost",      <---- Put your own database information here
  "port": 3306,             <----
  "username": "username",   <----
  "password": "password",   <----
  "database": "test",       <----
  "synchronize": true,
  "logging": false,
  "entities": ["dist/entity/**/*.js"],
  "migrations": ["dist/migration/**/*.js"],
  "subscribers": ["dist/subscriber/**/*.js"],
  "cli": {
    "entitiesDir": "src/entity",
    "migrationsDir": "src/migration",
    "subscribersDir": "src/subscriber"
  }
}

```
```
// example.env
PORT=80                    <---- Put your application listen port
```
#### 5. Create your Entity model
Create them for yourself in `src/entity` directory using [typeorm](https://github.com/typeorm/typeorm)
#### 6. Enjoy :)
## Usage
### Development

```
$ npm run watch
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)