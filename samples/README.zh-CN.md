# Micronaut Test 示例

[English](README.md) | [简体中文](README.zh-CN.md)

[Bean 替换](sample/test/DiscountTest.norm)通过 `@MicronautTest` 执行一个 JUnit 测试。`@MockBean` 替换应用中的折扣服务，使断言观察到折扣 12，而不是生产实现的 0。[消费者模块](sample/test/module.norm)依赖 `micronaut.test@2` 和注入处理器。

在仓库根目录运行：

```sh
norm test samples/sample/test --format json
```

结果应为发现并通过一个测试，没有失败。
