# singular-keycloak-database-federation

Keycloak User Storage SPI for Relational Databases (Keycloak User Federation, supports postgresql, mysql, oracle and mysql).

- Keycloak User federation provider with SQL
- Keycloak User federation using existing database
- Keycloak  database user provider
- Keycloak MSSQL Database Integration 
- Keycloak SQL Server Database Integration 
- Keycloak Oracle Database Integration 
- Keycloak Postgres Database Integration 
- Keycloak blowfish bcrypt support



## Usage

    Fully compatible with Singular Studio NOCODE. See https://www.studio.opensingular.com/
    

## Configuration

Keycloak User Federation Screen Shot

![Sample Screenshot](screen.png)


## Limitations

    - Do not allow user information update, including password update
    - Do not supports user roles our groups

## Custom attributes

Just add a mapper to client mappers with the same name as the returned column alias in your queries.Use mapper type "User Attribute". See the example below:
    
![Sample Screenshot 2](screen2.png)


## Build

    - mvn clean package

## Deployment

    - Deploy `.ear` to wildfly (keycloak)
        - i.e, on a default keycloak setup, copy the `.ear` file to <keycloak_root_dir>/standalone/deployments

