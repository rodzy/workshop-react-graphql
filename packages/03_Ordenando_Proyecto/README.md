# Comenzamos estructurando nuestros proyectos

Primeramente debemos pensar en como queremos estructurar nuestros proyectos y que necesitamos para trabajar, podemos tomar como referencia el diagrama de nuestro flujo del proyecto.

![PokeDigram](/.github/Diagram.png)

Podemos ver que nuestro flujo de aplicación depende de dos bloques.

| Cliente  |    Servidor   |
|----------|:-------------:|
| React.js |  Node         |
| Apollo Client |    GraphQL    |
| PokeAPI | TypeGraphQL   |
| ContextAPI | Apollo Server   |
|  | Express   |
|  | TypeORM  |

Estos dos bloques representan cada uno de los proyectos que tenemos que estructurar dentro de `packages`, le s puedes llamar como quieras, aunque en lo personal prefiero llamarles _Server_ y _Client_.

> Nota: La base de datos, la manejaremos de manera independiente ya sea por la consola de `psql` o por la interfaz de `pgAdmin` como te sea más sencillo.

Una vez tenemos las carpetas creadas nuestra estructura del proyecto debe ser algo similar a esto:

```s
├── packages
|    ├── Client
|    └── Server
├── .gitignore
├── LICENSE
├── package.json
└── README.md
```
