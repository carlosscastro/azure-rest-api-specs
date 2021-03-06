# StorageImportExport

> see https://aka.ms/autorest

This is the AutoRest configuration file for StorageImportExport.



---
## Getting Started
To build the SDK for StorageImportExport, simply [Install AutoRest](https://aka.ms/autorest/install) and in this folder, run:

> `autorest`

To see additional help and options, run:

> `autorest --help`
---

## Configuration



### Basic Information
These are the global settings for the StorageImportExport API.

``` yaml
openapi-type: arm
tag: package-2016-11
```


### Tag: package-2016-11

These settings apply only when `--tag=package-2016-11` is specified on the command line.

``` yaml $(tag) == 'package-2016-11'
input-file:
- Microsoft.ImportExport/stable/2016-11-01/storageimportexport.json
```


---
# Code Generation

## Swagger to SDK

This section describes what SDK should be generated by the automatic system.
This is not used by Autorest itself.

``` yaml $(swagger-to-sdk)
swagger-to-sdk:
  - repo: azure-sdk-for-go
  - repo: azure-sdk-for-go
```

## Go

These settings apply only when `--go` is specified on the command line.

``` yaml $(go)
go:
  license-header: MICROSOFT_APACHE_NO_VERSION
  namespace: storageimportexport
  clear-output-folder: true
```

### Go multi-api

``` yaml $(go) && $(multiapi)
batch:
  - tag: package-2016-11
```

### Tag: package-2016-11 and go

These settings apply only when `--tag=package-2016-11 --go` is specified on the command line.
Please also specify `--go-sdk-folder=<path to the root directory of your azure-sdk-for-go clone>`.

``` yaml $(tag) == 'package-2016-11' && $(go)
output-folder: $(go-sdk-folder)/services/storageimportexport/mgmt/2016-11-01/storageimportexport
```


## Java

These settings apply only when `--java` is specified on the command line.
Please also specify `--azure-libraries-for-java-folder=<path to the root directory of your azure-libraries-for-java clone>`.

``` yaml $(java)
azure-arm: true
fluent: true
namespace: com.microsoft.azure.management.storageimportexport
license-header: MICROSOFT_MIT_NO_CODEGEN
payload-flattening-threshold: 1
output-folder: $(azure-libraries-for-java-folder)/azure-mgmt-storageimportexport
```

### Java multi-api

``` yaml $(java) && $(multiapi)
batch:
  - tag: package-2016-11
```

### Tag: package-2016-11 and java

These settings apply only when `--tag=package-2016-11 --java` is specified on the command line.
Please also specify `--azure-libraries-for-java=<path to the root directory of your azure-sdk-for-java clone>`.

``` yaml $(tag) == 'package-2016-11' && $(java) && $(multiapi)
java:
  namespace: com.microsoft.azure.management.storageimportexport.v2016_11_01
  output-folder: $(azure-libraries-for-java-folder)/storageimportexport/resource-manager/v2016_11_01
regenerate-manager: true
generate-interface: true
```


