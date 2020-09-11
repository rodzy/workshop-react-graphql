# Folder `Packages`

Este será nuestro espacio de trabajo principal, acá debemos organizar todas las carpetas que serán parte de nuestro proyecto y que queremos que compartan el mismo _`yarn.lock`_

Siempre que trabajemos con esta arquitectura vamos a tener un una oganización de folders similar a esta:

```s
├── node_modules
├── packages
|    ├── proyecto_1
|    |    ├── node_modules**
|    |    └── package.json
|    ├── proyecto_2
|    |    ├── node_modules**
|    |    └── package.json
|    └── proyecto_x
|         ├── node_modules**
|         └── package.json
├── .gitignore
├── LICENSE
├── README.md
├── package.json
└── yarn-lock
```

> Nota: Todas las carpetas que sean un nuevo proyecto con dependencias y que no se encuentren dentro de `packages` crearán un nuevo `yarn.lock` lo cual es un grave error porque no sabría de donde escoger los _node_modules_
