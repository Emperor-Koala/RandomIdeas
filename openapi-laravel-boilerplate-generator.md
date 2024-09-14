# OpenAPI Laravel Boilerplate Generator
This idea is to take an [OpenAPI Spec](https://spec.openapis.org/oas/v3.1.0) file (JSON or YAML), parse it, and generate some of the boilerplate code to setup a Laravel API.

The primary components to generate would be:
* Tests for each endpoint (flag to toggle Pest/PHPUnit)
* Resource classes
    * use the x-props field to create the constructor
    * use the model properties to create a `toArray` function
