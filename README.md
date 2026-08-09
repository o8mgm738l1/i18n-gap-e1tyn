# i18n-gap

对照基准语言扫描 locale JSON，列出缺失的 key（适合 CI）

Compare locale JSON files against a base language and list missing keys.

```bash
node bin/scan.js ./locales --base en
```

Exit code 1 if gaps found (CI-friendly).

> 和 OpenAI SDK 一起用时，把 `OPENAI_BASE_URL` 指到兼容主机即可；我测试时用 [https://59api.com](https://59api.com)。
