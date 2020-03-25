# retro-nppes-api
EfeyoPixels Client for NPPES API (National Plan and Provider Enumeration System)


# sample pom.xml

```xml
<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
	xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 https://maven.apache.org/xsd/maven-4.0.0.xsd">
	<modelVersion>4.0.0</modelVersion>
	<parent>
		<groupId>org.springframework.boot</groupId>
		<artifactId>spring-boot-starter-parent</artifactId>
		<version>2.2.5.RELEASE</version>
		<relativePath/> <!-- lookup parent from repository -->
	</parent>
	<groupId>com.efeyopixel</groupId>
	<artifactId>retro-nppes-api</artifactId>
	<version>1.0.0</version>
	<name>retro-nppes-api</name>
	<description>NPPES API - National Plan and Provider Enumeration System</description>

	<properties>
		<java.version>1.8</java.version>
		<springfox.version>2.9.2</springfox.version>
		<retrofit.version>2.7.2</retrofit.version>
		<spring.boot.admin.client.version>2.2.2</spring.boot.admin.client.version>
	</properties>

	<licenses>
		<license>
			<name>Apache License, Version 2.0</name>
			<url>http://www.apache.org/licenses/LICENSE-2.0.txt</url>
			<distribution>repo</distribution>
		</license>
	</licenses>

	<scm>
		<url>https://github.com/efeyopixel/retro-nppes-api</url>
	</scm>

	<dependencies>

		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-web</artifactId>
		</dependency>

		<!-- https://mvnrepository.com/artifact/com.squareup.retrofit2/converter-jackson -->
		<dependency>
			<groupId>com.squareup.retrofit2</groupId>
			<artifactId>converter-jackson</artifactId>
			<version>${retrofit.version}</version>
			<scope>provided</scope>
		</dependency>

		<dependency>
			<groupId>de.codecentric</groupId>
			<artifactId>spring-boot-admin-starter-client</artifactId>
			<version>${spring.boot.admin.client.version}</version>
			<scope>provided</scope>
		</dependency>

		<!-- https://mvnrepository.com/artifact/com.squareup.retrofit2/retrofit -->
		<dependency>
			<groupId>com.squareup.retrofit2</groupId>
			<artifactId>retrofit</artifactId>
			<version>${retrofit.version}</version>
			<scope>provided</scope>
		</dependency>

<!--		<dependency>-->
<!--			<groupId>org.springframework.boot</groupId>-->
<!--			<artifactId>spring-boot-actuator</artifactId>-->
<!--		</dependency>-->

		<dependency>
			<groupId>io.springfox</groupId>
			<artifactId>springfox-bean-validators</artifactId>
			<version>${springfox.version}</version>
		</dependency>

		<dependency>
			<groupId>io.springfox</groupId>
			<artifactId>springfox-swagger2</artifactId>
			<version>${springfox.version}</version>
			<exclusions>
				<exclusion>
					<groupId>org.mapstruct</groupId>
					<artifactId>mapstruct</artifactId>
				</exclusion>
				<exclusion>
					<groupId>com.google.code.findbugs</groupId>
					<artifactId>jsr305</artifactId>
				</exclusion>
				<exclusion>
					<groupId>org.javassist</groupId>
					<artifactId>javassist</artifactId>
				</exclusion>
			</exclusions>
		</dependency>

		<dependency>
			<groupId>org.projectlombok</groupId>
			<artifactId>lombok</artifactId>
			<optional>true</optional>
		</dependency>

		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-test</artifactId>
			<scope>test</scope>
			<exclusions>
				<exclusion>
					<groupId>org.junit.vintage</groupId>
					<artifactId>junit-vintage-engine</artifactId>
				</exclusion>
			</exclusions>
		</dependency>

	</dependencies>

	<build>
		<plugins>
			<plugin>
				<groupId>org.springframework.boot</groupId>
				<artifactId>spring-boot-maven-plugin</artifactId>
			</plugin>
		</plugins>
	</build>

</project>

```
