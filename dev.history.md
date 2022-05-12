1. Ctrl + Shift + P  => Cretae a Gradle Project
   1. 2.6.7 => java => com.silentjin => test => war => 8
   2. Spring Web, Spring Boot DevTools, Spring Data JPA, Lombok, Thymeleaf

2. Edit application.properties
   ```
    server.port=9081

    # DataSource
    spring.datasource.url=jdbc:oracle:thin:@211.202.83.76:1521:orcl
    spring.datasource.username=ism
    spring.datasource.password=ism
    spring.datasource.driver-class-name=oracle.jdbc.driver.OracleDriver
   ```

3. NPM install
   1. npm install -g @vue/cli
   2. $PROJECT_HOME/src> view.cmd create view

4. Edit package.json , vue.config.js
   1. package.json 
    ```
        "serve": "vue-cli-service serve --open --port 9082",
    ```
   2. vue.config.js
    ```
        outputDir: "../src/main/resources/static",
        devServer: {
            proxy: {
                '/api': {
                    target: 'http://localhost:9081',
                    changeOrigin: true
                }
            }
        }
    ```

5. Create HelloWorld Service
   
6. axios install
   1. npm i axios --save

7. typescript add
   1. vue.cmd add typescript

8. execute
   1. Spring Boot run
   2. npm run serve

