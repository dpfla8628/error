### error
Failed to bind properties under 'spring.datasource.hikari' to com.zaxxer.hikari.HikariConfig    
Failed to load driver class com.mysql.jdbc.Driver in either of HikariConfig class loader or Thread context classloader    
   
### solution
driver-class-name: com.mysql.jdbc.Driver 
-> driver-class-name: org.mariadb.jdbc.Driver
