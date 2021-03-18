## For run application

Install addon (now, it is not installed)

From root package of application:

1. gradle buildUberJar
2. gradle moveJars
3. cd docker-image
4. docker build -t javamelody ./javamelody
5. docker build -t cuba-sample-sales-core ./core
6. docker build -t cuba-sample-sales-web ./web

**Pay attention!** In the docker-compose.yml file, first start postgres, then javamelody, and only then the core and web modules! 