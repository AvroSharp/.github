# AvroSharp

**A high-performance .NET implementation of the [Apache Avro™](https://avro.apache.org/) specification**, with source-generated serializers, schema evolution, container files with every codec, and schema-registry framing. It is faster than Apache.Avro on every benchmark it is measured on, allocates no more, and works with Native AOT and trimming.

**[Documentation](https://avrosharp.github.io/AvroSharp/)** · [Getting started](https://avrosharp.github.io/AvroSharp/docs/getting-started/index.html) · [API reference](https://avrosharp.github.io/AvroSharp/docs/api/index.html) · [Benchmarks](https://avrosharp.github.io/AvroSharp/docs/benchmarks.html) · [Compared with Apache.Avro](https://avrosharp.github.io/AvroSharp/docs/apache-avro.html) · [Samples](https://github.com/AvroSharp/AvroSharp/tree/main/samples) · [Migrating from Apache.Avro](https://avrosharp.github.io/AvroSharp/docs/migrating-from-apache-avro.html)

## Packages

From the [AvroSharp](https://github.com/AvroSharp/AvroSharp) repository, for .NET 8, 9 and 10, .NET Standard 2.0 and 2.1, and .NET Framework:

| Package | What it is |
|---|---|
| [AvroSharp](https://www.nuget.org/packages/AvroSharp) | The runtime: schemas, binary and JSON encoding, the generic model, schema resolution, container files, single-object and schema-registry messages, streams |
| [AvroSharp.Generators](https://www.nuget.org/packages/AvroSharp.Generators) | The source generator: C# types and serializers from `.avsc` files as the project builds |
| [AvroSharp.Tool](https://www.nuget.org/packages/AvroSharp.Tool) | `avrosharp`, the `dotnet tool`: code generation, canonical forms and fingerprints |
| [AvroSharp.Codecs](https://www.nuget.org/packages/AvroSharp.Codecs) | The snappy, zstandard, bzip2 and xz codecs, fully managed |
| [AvroSharp.CodeGen](https://www.nuget.org/packages/AvroSharp.CodeGen) | The code generation engine, for your own tools |
| [AvroSharp.Confluent](https://github.com/AvroSharp/AvroSharp/tree/main/src/AvroSharp.Confluent) | Confluent Schema Registry serializers for Confluent.Kafka, without Apache.Avro (new in the 1.0.0 release candidates) |

## Integrations

Add-on packages plug AvroSharp into the clients and frameworks applications already use. They live in the AvroSharp repository too, and are released with it at the same version:
- [AvroSharp.Confluent](https://github.com/AvroSharp/AvroSharp/tree/main/src/AvroSharp.Confluent), for Confluent.Kafka with Confluent Schema Registry and registries with its API, is in the release candidates.
- Planned: KafkaFlow ([#154](https://github.com/AvroSharp/AvroSharp/issues/154)), Azure Schema Registry ([#155](https://github.com/AvroSharp/AvroSharp/issues/155)) and AWS Glue Schema Registry ([#156](https://github.com/AvroSharp/AvroSharp/issues/156)).

The [integrations page](https://avrosharp.github.io/AvroSharp/docs/integrations.html) has the plan, and what works today. Feature requests and questions are welcome in [the issues](https://github.com/AvroSharp/AvroSharp/issues).

<sub>Apache Avro, Avro and Apache are trademarks of The Apache Software Foundation. AvroSharp is an independent project and is not endorsed by or affiliated with the Apache Software Foundation.</sub>
