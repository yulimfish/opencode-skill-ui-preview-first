# opencode-skill-ui-preview-first

> opencode 技能：**任何**会移动 DOM 节点的 UI 改动之前，先输出 ASCII wireframe（改前 → 改后）拿到一句确认，再动手。

隶属 [`opencode-codex-kit`](https://github.com/Yulimfish/opencode-codex-kit)。搭配 [`opencode-codex-guardrails`](https://github.com/Yulimfish/opencode-codex-guardrails) 效果最好 —— 后者会在 UI 文件路径上自动注入系统提示。

## 生效范围

- `.tsx / .jsx / .vue / .svelte / .astro / .html / .css / .scss / .sass / .less`
- `components/`、`ui/`、`views/`、`pages/`、`screens/`、`layouts/` 下的任何东西

**跳过**纯逻辑改动（handler 内部、hook 内部、值的调整）—— 只要不移动 DOM 节点就不管。

## 示例

```
改前                            改后
┌───────────────┐              ┌───────────────┐
│ [Logo]  Menu  │              │ [Logo]        │
├───────────────┤              │  ── Menu ──   │
│  Hero image   │              ├───────────────┤
│               │              │  Hero image   │
└───────────────┘              └───────────────┘
```

然后一句"go"从你这来，才开始改文件。

## 安装

```bash
mkdir -p ~/.config/opencode/skills
git clone https://github.com/Yulimfish/opencode-skill-ui-preview-first.git \
  ~/.config/opencode/skills/ui-preview-first
```

## 许可

MIT © Yulimfish
