Could not resolve dependencies for project    
Failure to find  in https://repo.maven.apache.org/maven2  
    
    
```    
source ~/.bash_profile
// 최상위 pom.xml위치에서 실행
sudo mvn -U clean install
```
```
pom.xml

  <repositories>
    <repository>
      <id>local-repo</id>
      <name>local Repository</name>
      <url>/Users/yerimlee/.m2/repository</url>
    </repository>
  </repositories>
```
```
그리고 하위 원하는 어플리케이션 pom파일 위치에서
sudo mvn -U clean install 실행
```
```
    <dependency>
        <groupId>org.projectlombok</groupId>
        <artifactId>lombok</artifactId>
        <version>1.18.20</version>
        <scope>provided</scope>
    </dependency>

```
