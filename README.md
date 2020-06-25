# GSON fully OSGi compatible

The intention of the repository is to provide an OSGi compatible version of the
GSON library. Unlike the original, all packages in the library are made
available for public access.

> GSON is fully OSGi compatible

GSON has all OSGi relevant metadata in the version rolled out by the vendor. The
execution in an OSGi-based runtime environment is possible without difficulty.

> Extension of the OSGI metadata set

In some projects, including the JClouds project, access is made to GSON-internal
package layers, which are excluded from public access.

The intention of such access is to implement features and capabilities that are
not provided by the GSON library.

## Use of the repository

This repository integrates the source code of the software project GSON as a Git
submodule. A direct use of the repository requires a manual execution of the
build process to generate the artifact.

## Using the artifact

The GSON artifact can also be used without the direct usage of the repository.

Besides the **_Github as a software repository_**, **_Gitlab is used as a common
delivery platform_**. The artifact is **_automatically build and deployed_** in
the package repository of the assigned Gitlab project.

> To provide a stable version of the artifact, the most recent release tag
> provided by the GSON project is used.

### Repository and dependency coordinates

```xml
<repository>
  <id>gitlab-maven</id>
  <url>https://gitlab.com/api/v4/projects/19575612/packages/maven</url>
</repository>
```

```xml
<dependency>
  <groupId>com.google.code.gson</groupId>
  <artifactId>gson</artifactId>

  <!--
    set latest version -
    initial version when the repository was made available - 2.8.6
  -->

  <version>2.8.6</version>
</dependency>
```
