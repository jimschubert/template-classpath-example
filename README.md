# OpenAPI Generator Template via Classpath

A somewhat silly example to demonstrate loading template files via classpath.

It's silly because nobody will want [Bangers](https://fonts.google.com/specimen/Bangers?selection.family=Bangers) as their documentation font!

## Use it

### Compile

```
gradle build publishToMavenLocal
```

### Consume

You can target this custom artifact and generate ike this:

```sh
java -cp ~/.m2/repository/org/openapitools/samples/template-classpath-example/1.0-SNAPSHOT/template-classpath-example-1.0-SNAPSHOT.jar:modules/openapi-generator-cli/target/openapi-generator-cli.jar org.openapitools.codegen.OpenAPIGenerator generate -i https://raw.githubusercontent.com/OAI/OpenAPI-Specification/master/examples/v3.0/petstore.yaml  -g html -o template-example -t templates/htmlDocs
```

Open `template-example/index.html` in your browser and take a look.
