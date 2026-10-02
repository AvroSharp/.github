<h1 align="center"><picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/AvroSharp/AvroSharp/main/docs/images/logo-dark.png"><img src="https://raw.githubusercontent.com/AvroSharp/AvroSharp/main/docs/images/logo.png" alt="AvroSharp"></picture></h1>

**A high-performance .NET implementation of the [Apache Avro™](https://avro.apache.org/) specification**, with source-generated serializers, schema evolution, container files with every codec, and schema-registry framing. It is faster than Apache.Avro on every benchmark it is measured on, allocates no more, and works with Native AOT and trimming.

**[Documentation](https://avrosharp.github.io/AvroSharp/)** · [Getting started](https://avrosharp.github.io/AvroSharp/docs/getting-started/index.html) · [API reference](https://avrosharp.github.io/AvroSharp/docs/api/index.html) · [Benchmarks](https://avrosharp.github.io/AvroSharp/docs/benchmarks.html) · [Compared with Apache.Avro](https://avrosharp.github.io/AvroSharp/docs/apache-avro.html) · [Samples](https://github.com/AvroSharp/AvroSharp/tree/main/samples) · [Migrating from Apache.Avro](https://avrosharp.github.io/AvroSharp/docs/migrating-from-apache-avro.html)

## Packages

From the [AvroSharp](https://github.com/AvroSharp/AvroSharp) repository, for .NET 8, 9 and 10, .NET Standard 2.0 and 2.1, and .NET Framework:

| Package | What it is |
|---|---|
| [AvroSharp](https://www.nuget.org/packages/AvroSharp) | The runtime: schemas, binary and JSON encoding, the generic model, schema resolution, container files, single-object and schema-registry messages, streams |
| [AvroSharp.Generators](https://www.nuget.org/packages/AvroSharp.Generators) | The source generator: C# types and serializers from `.avsc` files, and from your own types marked `[AvroSerializable]`, as the project builds |
| [AvroSharp.Tool](https://www.nuget.org/packages/AvroSharp.Tool) | `avrosharp`, the `dotnet tool`: code generation, canonical forms, fingerprints and compatibility checks |
| [AvroSharp.Codecs](https://www.nuget.org/packages/AvroSharp.Codecs) | The snappy, zstandard, bzip2 and xz codecs, fully managed |
| [AvroSharp.CodeGen](https://www.nuget.org/packages/AvroSharp.CodeGen) | The code generation engine, for your own tools |

## Integrations

Add-on packages plug AvroSharp into the clients and frameworks applications already use, without Apache.Avro. They live in the AvroSharp repository too, are new in 1.0.0, and are released with AvroSharp at the same version:

| Package | For |
|---|---|
| [AvroSharp.Confluent](https://github.com/AvroSharp/AvroSharp/tree/main/src/AvroSharp.Confluent) | Kafka with Confluent Schema Registry, and registries with its API: serializers for Confluent.Kafka, with the same bytes and settings as Confluent's Avro serializer ([guide](https://avrosharp.github.io/AvroSharp/docs/confluent.html)) |
| [AvroSharp.KafkaFlow](https://github.com/AvroSharp/AvroSharp/tree/main/src/AvroSharp.KafkaFlow) | KafkaFlow producers and consumers, on AvroSharp.Confluent ([guide](https://avrosharp.github.io/AvroSharp/docs/kafkaflow.html)) |
| [AvroSharp.Azure.SchemaRegistry](https://github.com/AvroSharp/AvroSharp/tree/main/src/AvroSharp.Azure.SchemaRegistry) | Azure Schema Registry with Event Hubs and Service Bus ([guide](https://avrosharp.github.io/AvroSharp/docs/azure-schema-registry.html)) |
| [AvroSharp.Aws.Glue](https://github.com/AvroSharp/AvroSharp/tree/main/src/AvroSharp.Aws.Glue) | AWS Glue Schema Registry, fully managed, on every platform ([guide](https://avrosharp.github.io/AvroSharp/docs/aws-glue.html)) |
| [AvroSharp.Aws.Glue.Kafka](https://github.com/AvroSharp/AvroSharp/tree/main/src/AvroSharp.Aws.Glue.Kafka) | Confluent.Kafka serializers for AWS Glue Schema Registry, on AvroSharp.Aws.Glue ([guide](https://avrosharp.github.io/AvroSharp/docs/aws-glue.html)) |

The [integrations page](https://avrosharp.github.io/AvroSharp/docs/integrations.html) covers what each one does, and how to use AvroSharp with a registry without them. Feature requests and questions are welcome in [the issues](https://github.com/AvroSharp/AvroSharp/issues).

<sub>Apache Avro, Avro and Apache are trademarks of The Apache Software Foundation. AvroSharp is an independent project and is not endorsed by or affiliated with the Apache Software Foundation.</sub>
