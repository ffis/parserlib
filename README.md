# Parserlib

HL7 utility that parsers hl7 messages from a directory and stores some data on mssql server

It is intended to be used with [compass](https://github.com/ffis/compass) project as 
it's meaningless and useless without it.


## Prerequisites

* NodeJS v9 or later, it might work on previously releases but they are not supported anymore.
* Microsoft SQL database with the schema created by [compass](https://github.com/ffis/compass) project.
* Git, recommended to keep the code updated in an easier way.
* Filesystem requirements are as big as the files you are going to need to handle.
* Docker environment is also recommended but it's not a truly requirement.

## Instalation process

```bash
git clone https://github.com/ffis/parserlib
```

You need to configure the _config.json_ file, set the database connection string and the directories where the files are going to be handle.

```bash
npm install
npm test
```

If all the tests run OK then you only need to run:


```bash
forever index.js
```

