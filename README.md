# osv-scanner-test

## Preparation

```shell
go install github.com/google/osv-scanner/v2/cmd/osv-scanner@v2.2                                                                                                                                                                                                           ‹git:main ✘› 12:24.06 Mon Aug 11 2025 >>> 
```

## Failure

```shell
osv-scanner scan source -r .
```

## Success

1. Uncomment in pom.xml:

```xml

<dependency>
  <groupId>io.quarkus</groupId>
  <artifactId>quarkus-vertx</artifactId>
  <version>3.24.0</version>
</dependency>
```

2. Run:

```shell
osv-scanner scan source -r .
```

