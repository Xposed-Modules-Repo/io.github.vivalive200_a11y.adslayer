# AdSlayer

No-op initialization of third-party ad SDKs (Pangle/CSJ, YLH/GDT, Kuaishou Union, Baidu BES, TopOn) in scoped apps.

- Works on LSPosed / Vector (legacy Xposed API + libxposed-ready)
- Apps are NOT hardcoded: injects into whatever apps you put in this module's scope
- Does not modify target APKs, no re-signing, no signature/integrity breakage — Taobao/Alipay logins unaffected
- Survives host app OTA (hooks public/stable ad-SDK shell APIs)
- Built-in anti-tamper: defeats SecNeo-class packers' fake Xposed-API canary via early warm-up binding
- Open source: https://github.com/vivalive200-a11y/AdSlayer

⚠️ Not recommended to scope: ByteDance/Tencent consumer apps (ads are their own monetization + coin tasks), video players (self-served pre-roll).
