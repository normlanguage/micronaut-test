# Micronaut Test samples

[English](README.md) | [简体中文](README.zh-CN.md)

[Bean replacement](sample/test/DiscountTest.norm) runs one JUnit test through `@MicronautTest`. `@MockBean` replaces the application discount service, so the assertion observes a discount of 12 instead of the production value 0. The [consumer module](sample/test/module.norm) depends on `micronaut.test` and the injection processor.

From the repository root, run:

```sh
norm test samples/sample/test --format json
```

The result must report one test found, one passed, and no failures.
