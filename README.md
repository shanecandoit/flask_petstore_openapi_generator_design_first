

shane@r15 ~/code/flask_petstore
$ java -jar ~/downloads/openapi-generator-cli-6.6.0.jar help
usage: openapi-generator-cli <command> [<args>]

The most commonly used openapi-generator-cli commands are:
    author        Utilities for authoring generators or customizing templates.
    batch         Generate code in batch via external configs.
    config-help   Config help for chosen lang
    generate      Generate code with the specified generator.
    help          Display help information about openapi-generator
    list          Lists the available generators
    meta          MetaGenerator. Generator for creating a new template set and configuration for Codegen.  The output will be base
d on the language you specify, and includes default templates to include.
    validate      Validate specification
    version       Show version information used in tooling

See 'openapi-generator-cli help <command>' for more information on a specific
command.

$ java -jar /d/downloads/openapi-generator-cli-6.6.0.jar list

    ...
SERVER generators:
    ...
    - go-echo-server (beta)
    - go-gin-server
    - go-server
    ...
    - nodejs-express-server (beta)
    ...
    - python-aiohttp
    - python-blueplanet
    - python-fastapi (beta)
    - python-flask
    ...
    - rust-server
    ...
    - spring
    ...



(if you're on Windows, replace the last command with java -jar modules\openapi-generator-cli\target\openapi-generator-cli.jar generate -i https://raw.githubusercontent.com/openapitools/openapi-generator/master/modules/openapi-generator/src/test/resources/3_0/petstore.yaml -g php -o c:\temp\php_api_client)



$ java -jar ~/downloads/openapi-generator-cli-6.6.0.jar generate -i petstore.yaml -g python-flask -o python_server

to run it:
1. cd python_server
2. pip install -r requirements.txt
3. export FLASK_APP=run.py
4. flask run

$ java -jar ~/downloads/openapi-generator-cli-6.6.0.jar generate -i petstore


OpenAPI_Petstore.postman_collection.json
was generated with postman from petstore.yaml
