##### 시작전에...

번역을 전문으로 하는 사람도 아니고 영어를 잘하는 사람도 아닙니다.
천~~~~~~~천히 봐가면서 공부를 하기 위한 목적이므로 더딘 번역이 될듯합니다.


# Part I. Spring Boot Documentation

이 섹션은 Spring Boot에 대한 레퍼런스 문서를 간단히 설명합니다. map으로서 문서들을 제공합니다.
This section provides a brief overview of Spring Boot reference documentation. It serves as a map for
the rest of the document

## Chapter 1. About the Documentation

Spring Boot 레퍼런스 가이드는 아래 링크에서 이용가능합니다.

* [HTML](https://docs.spring.io/spring-boot/docs/2.0.0.RELEASE/reference/html)
* [PDF](https://docs.spring.io/spring-boot/docs/2.0.0.RELEASE/reference/pdf/spring-boot-reference.pdf)
* [EPUB](https://docs.spring.io/spring-boot/docs/2.0.0.RELEASE/reference/epub/spring-boot-reference.epub)

최신 버전 문서는 [https://docs.spring.io/spring-boot/docs/current/reference/](https://docs.spring.io/spring-boot/docs/current/reference/)에서 이용 가능합니다.

이 문서는 본인 또는 타인에게 제공하기 위한 배포 목적으로 사본을 만들 수 있습니다.
비영리적인 목적이ㅣ여야 하며, 각 복사본에는 저작권이 명시되어야 합니다.
전자, 인쇄로서 배포여부와는 상관 없이 공지되어야 합니다.

*you do not charge any fee for such copies and further provided that each copy contains this Copyright
Notice, whether distributed in print or electronically.*

## Chapter 2. Getting Help

Spring Boot에 문제가 있는 경우 아래의 방법으로 도움을 드릴 수 있습니다.

* "How-to documents"를 참고하세요. 많은 질문에 대한 문제 해결 방법이 있습니다.
* Spring를 배우세요. Spring Boot는 많은 다른 Spring 프로젝트를 기반으로 만들어 졌습니다. [spring.io](spring.io) 웹 사이트를 확인하여 많은 참고 문서들을 확인 할 수 있습니다. 처음 Spring를 시작해 본다면 [guides](https://spring.io/guides)를 시도해 보세요.
* 물어보세요. 우리는 [stackoverflow](https://stackoverflow.com)에서 spring-boot 테그의 질문들을 모니터링하고 있습니다.
* [github.com/spring-projects/spring-boot/issues](github.com/spring-projects/spring-boot/issues)에 버그들을 이슈로 남겨주세요.

Note

>문서를 포함한 Spring Boot의 모든것은 open source입니다. 문서에 문제를 발견하거나 개선할 부분을 찾으면 [기여해주세요.](https://github.com/spring-projects/spring-boot/tree/v2.0.0.RELEASE)

## Chapter 3. First Steps

Spring Boot 또는 Spring을 시작하는 경우 다음 따라 시작하세요.

* 시작하기: Overview | Requirements | Installation
* 튜토리얼 : Part 1 | Part 2
* Running your example: Part 1 | Part 2


## Chapter 4. Working with Spring Boot  

Ready to actually start using Spring Boot? We have you covered:

* Build systems: Maven | Gradle | Ant | Starters  
* Best practices: Code Structure | @Configuration | @EnableAutoConfiguration | Beans and Dependency Injection  
* Running your code IDE | Packaged | Maven | Gradle  
* Packaging your app: Production jars  
* Spring Boot CLI: Using the CLI  

##Chapter 5. Learning about Spring Boot Features  

Spring Boot의 핵심적인 부분을 좀 더 배우고 싶다면 아래의 내용을 참고해 주세요.:  

* Core Features: SpringApplication | External Configuration | Profiles | Logging  
* Web Applications: MVC | Embedded Containers  
* Working with data: SQL | NO-SQL  
* Messaging: Overview | JMS  
* Testing: Overview | Boot Applications | Utils  
* Extending: Auto-configuration | @Conditions  

##Chapter 6. Moving to Production  

실사용으로서 Spring Boot Application을 사용할 때를 위해 아래와 같은 몇가지를 제공합니다.  

* Management endpoints: Overview | Customization  
* Connection options: HTTP | JMX  
* Monitoring: Metrics | Auditing | Tracing | Process  

##‘Chapter 7. Advanced Topics

고급 사용자를 위한 몇가지 주제를 가지고 있습니다.

* Spring Boot Applications Deployment: Cloud Deployment | OS Service  
* Build tool plugins: Maven | Gradle  
* Appendix: Application Properties | Auto-configuration classes | Executable Jars  

## Chapter 8. Introducing Spring Boot

Spring Boot는 상용화 수준의 Spring 기반의 어플리케이션이 단독적으로 쉽게 실행 할 수 있게 해줍니다. 우리는 Spring 플랫폼과 서드파티 라이브러리의 의견을 수렴하여 시작하였습니다. 때문에 최소한의 문제를 가지고 시작되었습니다. 대부분의 Spring Boot 어플리케션은 Spring 설정의 아주 적은 부분만을 필요로합니다.

Spring Boot를 사용하여 `Java -jar` 또는 좀더 전통적인 war 배포를 통해 Java 어플리케이션을 생성할 수 있습니다. 우리는 또한 "spring scripts" 실행할 수 있도록 커멘드 라인을 제공합니다.

우리의 목표는 다음과 같습니다. :

* 모든 Spring 개발에 대하여 빠르고 광범위한 시작 경험을 제공합니다.
* 기본에서 벗어나는 요구사항에 대하여 빠르게 시작 할 수 있습니다.
* 임베디드 서버, 보안, 메트릭, health checks, 외부 설정과 같이 기능 외적인 부분에 대한 것들을 지원합니다.
* 코드 생성이 절대 없고 xml 설정을 필요로 하지 않습니다.


## Chapter 9. 시스템 요구사항  

Spring Boot 2.0.0.RELEASE는 Java 8 또는 Java 9와 Spring Framework 5.0.4.RELEASE 이상이 필요합니다. Maven 3.2+와 Gradle 4를 사용합니다.

### Servlet Containers

Spring Boot는 아래의 Servlet Containers 내장하고 있습니다.

| 이름 | Servlet Version |
|---|---|  
| Tomcat 8.5 | 3.1 |  
| Jetty 9.4 | 3.1 |  
| Undertow 1.4 | 3.1 |  

Servlet 3.0+의 compatible container를 통하여 Spring Boot를 배포 할 수 있습니다.

## Chapter 10. Installing Spring Boot  

Spring Boot는 Command Line Tool이나 같은 전통적인 자발 개발 도구를 사용 할 수 있습니다. 어느 쪽이던 Java SDK v1.8 이상을 필요로 합니다. 시작하기 전에 다음 명령어를 통해 현재 설치된 Java버전을 확인 해 보세요.  

> $ java -version  

자바 개발을 처음 하시는 분이거나 Spring Boot를 실험 해보고 싶으시다면, Spring Boot CLI를 해보세요. 기존의 설치 지침을 읽어 사용하셔도 됩니다.  

### Installation Instructions for the Java Developer  

Spring Boot는 표준 Java 라이브러리처럼 사용할 수 있습니다. 그렇게 하기 위해서 `spring-boot-*.jar`파일을 classpath에 포함시키세요. Spring Boot는 별도의 통합 툴을 필요로 하지 않습니다. 그렇기 때문에 어떤한 IDE나 Text editor를 사용해도 무방합니다. Spring Boot를 위한 특별한 장치가 없더라도 Java프로그램을 실행하거나 debug할 수 있습니다.

#### Maven Installation  

Spring Boot는 Maven 3.2이상과 호환됩니다. 만족되는 Maven이 설치되어있지 않다면 [maven.apache.org.](https://maven.apache.org/)의 소개에 따라 주세요.  

Tip  
    여러 운영체제에서는 패키지 매니져를 통한 Maven를 설치 할 수 있습니다.  
  * OSX에서의 Homebrew는 `brew install maven`
  * Ubuntu사에서는 `apt-get install maven`
  * Window의 (관리자 권한에서) Chocolatey에서는 `choco install maven`

Spring Boot 의존성은 `org.springframework.boot` group id를 사용합니다. 일반적으로, Maven POM 파일은 `spring-boot-starter-parent` 프로젝트와 의존성들이 작성되어 있는 다른 "starter"를 상속합니다. Spring Boot는 또한 실행가능한 jars를 생성하기 위한 Maven 플러그인을 제공합니다.  

다음은 기본적인 pom.xml파일 입니다.

```xml
<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
	xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
	<modelVersion>4.0.0</modelVersion>

	<groupId>com.example</groupId>
	<artifactId>myproject</artifactId>
	<version>0.0.1-SNAPSHOT</version>

	<!-- Inherit defaults from Spring Boot -->
	<parent>
		<groupId>org.springframework.boot</groupId>
		<artifactId>spring-boot-starter-parent</artifactId>
		<version>2.0.0.RELEASE</version>
	</parent>

	<!-- Add typical dependencies for a web application -->
	<dependencies>
		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-web</artifactId>
		</dependency>
	</dependencies>

	<!-- Package as an executable jar -->
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

Tip  
  `spring-boot-starter-parent`는 Spring Boot를 사용하기 위한 최고의 방법입니다. 하지만 이것이 항상 최적의 방법은 아닙니다. 가끔은 다른 parent POM를 상속하여 사용하거나 기본 설정과는 다른 것이 필요할 것입니다. 그럴경우에는 `import scope`를 사용하여 해결하는 "Using Spring Boot Without the Parent"의 섹션를 참고하면 됩니다.

#### Gradle Installation  

Spring Boot는 Gradle 4와 호환합니다. Gradle이 설치가 되어있지 않다면 [gradle.org/.](https://gradle.org/)의 소개에 따라 주세요.  

Spring Boot 의존성들은 `org.springframework.bootgroup.`를 통하여 작성될 수 있습니다. 일반적으로 당신의 프로젝트는 하나 이상의 "Starter" 통하여 작성 될수 있습니다. Spring Boot는 유용한 Gradle Plugin를 제공하여 간단하게 의종성들을 작성하고 실생가능한 jars를 생성할 수 있습니다.  

##### Gradle Wrapper  
Gradle Wrapper는 프로젝트를 빌드할 떄 Gradle를 획득할 수 있는 좋은 방식을 제공합니다. 이것은 당신의 코드를 빌드 프로레스와 부트스트랩를 커밋하기 위한 작은 스크립트와 라이브러리입니다. [docs.gradle.org4.2.1/userguide/gradle_wrapper.html](docs.gradle.org4.2.1/userguide/gradle_wrapper.html)를 참고하세요.  

The Gradle Wrapper provides a nice way of “obtaining” Gradle when you need to build a project. It is a small script and library that you commit alongside your code to bootstrap the build process. See docs.gradle.org/4.2.1/userguide/gradle_wrapper.html for details.

일반적인 `build.gradle`파일의 예제입니다.

```java
plugins {
	id 'org.springframework.boot' version '2.0.0.RELEASE'
	id 'java'
}


jar {
	baseName = 'myproject'
	version =  '0.0.1-SNAPSHOT'
}

repositories {
	jcenter()
}

dependencies {
	compile("org.springframework.boot:spring-boot-starter-web")
	testCompile("org.springframework.boot:spring-boot-starter-test")
}
```

### Installing the Spring Boot CLI
 Spring Boot CLI (Command Line Interface)는 스프링을 이용한 프로토타입을 빠르게 만들 수 있게 합니다.
이것은 당신의 [Groovy](http://groovy-lang.org/) Script를 사용할 수 있게합니다. 이 말은 즉슨, 상용구 코드(boilerplate code)가 없이도 친 Java적인 언어를 사용합니다.

 CLI는 Spring 어플리케이션을 처음부터 시작하기 위한 제일 빠른 방법이지만, Spring Boot를 이용하는데 있어서 CLI를 사용하지 않아도 됩니다.


#### Manual Installation
 Spring 소프트웨어 저장소에서 Spring CLI 배포판을 다운로드 할 수 있습니다. :

 [spring-boot-cli-2.1.0.BUILD-SNAPSHOT-bin.zip](https://repo.spring.io/snapshot/org/springframework/boot/spring-boot-cli/2.1.0.BUILD-SNAPSHOT/spring-boot-cli-2.1.0.BUILD-SNAPSHOT-bin.zip)
 [spring-boot-cli-2.1.0.BUILD-SNAPSHOT-bin.tar.gz](https://repo.spring.io/snapshot/org/springframework/boot/spring-boot-cli/2.1.0.BUILD-SNAPSHOT/spring-boot-cli-2.1.0.BUILD-SNAPSHOT-bin.tar.gz)

 최신 [스냅샷](https://repo.spring.io/snapshot/org/springframework/boot/spring-boot-cli/) 또한 사용 가능합니다.  

 처음 다운로드 후, 압축을 푼 후 [INSTALL.txt](https://raw.githubusercontent.com/spring-projects/spring-boot/master/spring-boot-project/spring-boot-cli/src/main/content/INSTALL.txt)의 내용을 읽고 따라 주세요. 요약하자면 `.zip` 파일 안에는 `/bin` 폴더에 `spring` script(windows에선 `spring.bat`)가 있습니다. `.jar`파일을 사용하신다면 `java -jar`를 사용 할 수 있습니다. (스크립트의 도움으로 classpath가 올바르게 되었는 지 알 수 있습니다.)

#### Installation with SDKMAN!

SDKMAN! (The Software Development Kit Manager)는 Groovy와 Sprint Boot CLI를 포함한 다양한 바이너리 SDK들의 여려 버전을 관리 할 수 있게 해줍니다. [sdkman.io](http://sdkman.io/)를 사용해 보세요! 아래 명령어를 따라 Spring Boot에 설치 할 수 있습니다. :  

```
$ sdk install springboot
$ spring --version
Spring Boot v2.1.0.BUILD-SNAPSHOT
```

만약 개발 버전를 위한 CLI와 당신의 설치를 위한 버전으로 쉽게 접근하고 싶으시다면, 다음을 따라주세요.:  

```
$ sdk install springboot dev /path/to/spring-boot/spring-boot-cli/target/spring-boot-cli-2.1.0.BUILD-SNAPSHOT-bin/spring-2.1.0.BUILD-SNAPSHOT/
$ sdk default springboot dev
$ spring --version
Spring CLI v2.1.0.BUILD-SNAPSHOT
```

앞서 알려드린 설치는 `dev`로 이름으로 `spring` 인스턴스를 설치합니다. Spring Boot를 다시 빌드 할 때 마다 타겟 빌드 위치에는 Spring이 업데이트하게 됩니다.  

다음을 따라 실행되는 걸 볼 수 있습니다.  

```
$ sdk ls springboot

================================================================================
Available Springboot Versions
================================================================================
> + dev
* 2.1.0.BUILD-SNAPSHOT

================================================================================
+ - local version
* - installed
> - currently in use
================================================================================
```

#### OSX Homebrew Installation  

Mac과 Homebrew를 사용하신다면, 다음 명령어를 따라 Spring Boot CLI를 설치 할 수 있습니다. :

```
$ brew tap pivotal/tap
$ brew install springboot
```

Homebrew는 `/usr/local/bin` 위치에 `spring`을 설치합니다.

#### OSX Homebrew Installation  

Mac과 Homebrew를 사용하신다면, 다음 명령어를 따라 Spring Boot CLI를 설치 할 수 있습니다. :

```
$ brew tap pivotal/tap
$ brew install springboot
```

Homebrew는 `/usr/local/bin` 위치에 `spring`을 설치합니다.

#### MacPorts Installation  

Mac과 MacPorts를 사용하신다면, 다음 명령어를 따라 Spring Boot CLI를 설치 할 수 있습니다. :  

```
$ sudo port install spring-boot-cli
```

#### Command-line Completion

Spring Boot CLI는 `BASH`와 `zsh`쉘을 통한 설치 완료를 위한 스크립트를 포함하고 있습니다. 스크립트(spring)를 모든 쉘로 사용하거나, 개인 프로젝트나 시스템 전체에 (your personal or system-wide) 초기화 완료에 사용 할 수 있습니다. 데비안 시스템에서는 시스템 전체의 스크립트가 `/shell-completion/bash`에 있고 이 곳에 있는 모든 스크립트는 새로운 쉘이 시작 할 떄 실행됩니다. 예를 들어 SDKMAN를 사용하여 설치했으면 직접 실행시키기 위해서 다음의 명령어를 사용하면 됩니다. :  

```
$ . ~/.sdkman/candidates/springboot/current/shell-completion/bash/spring
$ spring <HIT TAB HERE>
  grab  help  jar  run  test  version
```  

#### Quick-start Spring CLI Example  

다음을 간단한 웹 어플리케이션을 통해 설치가 됬을믈 확인 할 수 있습니다. 시작하기 위해 `app.groovy`의 이름으로 아래 내용을 따라 해보세요. :  

```
@RestController
class ThisWillActuallyRun {

	@RequestMapping("/")
	String home() {
		"Hello World!"
	}

}
```

쉘에서 다음을 따라 실행합니다. :

```
$ spring run app.groovy
```

Note

> 처음에는 dependencies 다운로드 때문에 실행이 느립니다. 이후부터는 훨씬 빠른 속도로 실행됩니다.  

[localhost:8080](localhost:8080)를 열면 다음과 같은 출력이 보일것 입니다.  

Hello World!  


### Upgrading from an Earlier Version of Spring Boot

이전 버전의 Spring Boot로부터 업드레이드를 한다면, ["migration guide" on the project wiki](https://github.com/spring-projects/spring-boot/wiki/Spring-Boot-2.0-Migration-Guide)에서 제공되는 업그레이드 소개를 확인하세요. ["release notes"](https://github.com/spring-projects/spring-boot/wiki)의 각 릴리즈들을 확인하여 새로운 핵심적인 정보들(new and notewrthy) 확인합니다.  
기존 CLI 설치를 업그레이드하려면 해당 패키지 관리자 명령 (예 : brew upgrade)을 사용하시거나, CLI를 수동으로 설치 한 경우, [standard instructions](https://docs.spring.io/spring-boot/docs/current-SNAPSHOT/reference/htmlsingle/#getting-started-manual-cli-installation)를 따라서 PATH 환경 변수를 업데이트하여 이전 참조 파일들을 제거합니다.  


## Chapter 11. Developing Your First Spring Boot Application  

 이 섹션에서는 Spring Boot의 중요 기능을 이용해 쉽게 "Hello Would!" 웹 어플리케이션을 만들어봅니다. 우리는 대부분의 IDE는 Maven을 지원하기 떄문에 Maven을 사용합니다.  

Tip  
  [spring.io](https://spring.io/) 웹사이트에는 Spring Boot를 이용한 많은 'Getting Started' guides 가 있습니다. 어떠한 문제가 발생하면 먼저 위의 사이트에서 확인을 하시기 바랍니다. [start.spring.io](https://start.spring.io/) 사이트에서 deplendencies 검색기에서 'Web' starter를 찾아 바로 시작 할 수 있습니다. 새로운 프로젝트 구조를 생성하고 난뒤 바로 코딩을 시작할 수 있습니다. [Spring Initalizr documentation](https://github.com/spring-io/initializr)를 확인해 자세히 알아보세요.  

 우리는 시작하기 전에 터미널을 열고 다음을 명령어를 따라 Java와 Maven의 설치된 버전을 확인 할 수 있습니다.

 ```
 $ java -version
java version "1.8.0_102"
Java(TM) SE Runtime Environment (build 1.8.0_102-b14)
Java HotSpot(TM) 64-Bit Server VM (build 25.102-b14, mixed mode)
 ```

 ```
 $ mvn -v
Apache Maven 3.3.9 (bb52d8502b132ec0a5a3f4c09453c07478323dc5; 2015-11-10T16:41:47+00:00)
Maven home: /usr/local/Cellar/maven/3.3.9/libexec
Java version: 1.8.0_102, vendor: Oracle Corporation
 ```

Note  
  위 코드는 소유한 폴터에 생성되어야 합니다. 다음의 절차주터는 당신의 현제 디렉토리나 알맞는 폴터에서 진행됩니다. ?

### 11.1 Creating the POM

Maven에서의 pom.xml를 생성함으로서 시작합니다. pom.xml는 프로젝트를 만드는데 있어서 필요한 목록입니다. 당신의 Text editor를 이용해 다음을 따라하세요.

```
<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
	xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
	<modelVersion>4.0.0</modelVersion>

	<groupId>com.example</groupId>
	<artifactId>myproject</artifactId>
	<version>0.0.1-SNAPSHOT</version>

	<parent>
		<groupId>org.springframework.boot</groupId>
		<artifactId>spring-boot-starter-parent</artifactId>
		<version>2.0.0.RELEASE</version>
	</parent>

	<!-- Additional lines to be added here... -->

</project>

```

앞의 목록은 당신에게 빌드를 제공합니다. `mvn package` 명령어를 통해 테스트 해볼 수 있습니다. (현제 상태에서 발생하는 `“jar will be empty - no content was marked for inclusion!”` 워닝은 무시할 수 있습니다.)  

Note
  요점은, 이를 통해 IDE(maven을 지원하는 가장 현대적인 java IDE)으로 프로젝트를 설정 할 수 있다는 것입니다. 간단히 말해, 우리는 위의 예제를 위해 text editor를 사용하게 될것 입니다.  

#### 11.2 Adding Classpath dependencies

 Spring Boot는 당신의 classpath에 jars를 추가 할 수 있도록 몇몇개의 "Starter"를 제공해 줍니다. 우리의 셈플 어플리케이션에서의 POM의 `parent`부분에 `spring-boot-starter-parent`가 이미 추가되어 있습니다. `spring-boot-starter-parent`는 유용한 Maven의 기본적인 것들을 제공해주는 특별한 starter입니다. 이는 또한 `dependency-management`에서 "blessed" dependencies에서 version 테그를 생략할 수 있게 해줍니다.  

  다른 "Starters"들은 특정한 타입의 어플리케이션을 만들 때 필요한 것들을 제공해 줍니다. 웹 어플리케이션을 만든다면, `spring-boot-starter-web` 의존선을 추가하면됩니다. 그 전에는 다음 명령어를 실행하여 현재의 의존성들을 확인할수 있습니다.

```
$ mvn dependency:tree

[INFO] com.example:myproject:jar:0.0.1-SNAPSHOT
```

`mvn dependency:tree` 명령어는 당신의 프로젝트의 의존성을 트리 모양으로 출력해줍니다. 당신은 `spring-boot-starter-parent`이 의존성들을 제공해주지 않는다는 것을 볼 수 있을 것 입니다. 필요한 의존성들을 `pom.xml`에서 `spring-boot-starter-web` 의존성의 `parent`부분 바로 아래에 바로 추가하면 됩니다.

```
<dependencies>
	<dependency>
		<groupId>org.springframework.boot</groupId>
		<artifactId>spring-boot-starter-web</artifactId>
	</dependency>
</dependencies>
```

`mvn dependency:tree`를 다시 실행해본다면, 추가된 의존성들을 spring boot, tomcat web server와 함깨 볼 수 있습니다.

#### 11.3 Writing the code``

 이 예제 어플리케이션을 완성하기 위해서는 하나의 자바 파일이 필요합니다. 기본적으로 maven 컴파일러는 `src/main/java` 아래의 파일들을 사용합니다. 그러므로 그 구조에 따라서 `src/main/java/Example.java`으로 아래 내용을 작성합니다.   

 ```
 import org.springframework.boot.*;
import org.springframework.boot.autoconfigure.*;
import org.springframework.web.bind.annotation.*;

@RestController
@EnableAutoConfiguration
public class Example {

	@RequestMapping("/")
	String home() {
		return "Hello World!";
	}

	public static void main(String[] args) throws Exception {
		SpringApplication.run(Example.class, args);
	}

}
 ```

 긴 코드는 아니지만 꽤 많은 일들이 일어나고 있습니다. 다음 섹션들을 통해 중요한 부분들을 단계별로 설명합니다.  

#### 11.3.1  The @RestController and @RequestMapping Annotation

`Example` class의 처음으로 보게 되는 annotation `@RestController`입니다. 이것은 *stereotype* annotation으로 알려져 있습니다. 이것은 코드를 읽는 사람에게 힌트를 주고 Spring에게 이 class가 특정 역활을 한다고 알려줍니다. 이번 경우에서는 이 클래스는 web @Controller이기 때문에 Spring은 들어오는 웹 요청을 처할 떄 고려하게 됩니다.  

@RequestMapping annotation는 "Routing" 정보를 제공합니다. 위의 경우 `/`경로의 HTTP요청이 들어오는 것들에 대해서 `home` 메서드에 맵핑해줍니다. `@RestController` annotation은 Spring에게 요청자에게 문자열로서 결과값을 랜더링 하라고 알려줍니다.  

Tip.
    `@RestController`와 `@RequestMapping` annotation들은 Spring MVC annotation들입니다. (이것들은 Spring Boot에 속해있지 않습니다.) Spring 레퍼런스 문서의 [MVC section](https://docs.spring.io/spring/docs/5.0.4.RELEASE/spring-framework-reference/web.html#mvc)를 참고하여 더 알아보세요.  
