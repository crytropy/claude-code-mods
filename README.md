# claude-code-mods

我的 Claude Code mod，全部放在這個 marketplace。每個 mod 一個資料夾。

| 名稱 | 功能 | 說明 |
|---|---|---|
| `windsock` | 輸入框上方的資訊列：用量、PR 狀態、快取倒數（Pro、Max） | [windsock/README.md](windsock/README.md) |
| `windsock-ultra` | 同上，Ultra 方案用（不顯示 5 小時） | [windsock/README.md](windsock/README.md#兩個版本) |
| `output-style` | 輸入框下方顯示目前的 output style，`/style` 切換 | [output-style/README.md](output-style/README.md) |
| `one-click-handoff` | Context 用到 70% 時，一鍵寫交接文件並開新對話 | [one-click-handoff/README.md](one-click-handoff/README.md) |

`windsock` 和 `windsock-ultra` 只能裝一個。

## 安裝

```
/plugin marketplace add crytropy/claude-code-mods
/plugin install windsock@claude-code-mods
/plugin install output-style@claude-code-mods
/plugin install one-click-handoff@claude-code-mods
```

也可以開 `/plugin`，到 `claude-code-mods` marketplace 裡挑。

## 從舊的 repo 換過來

以前從 `crytropy/windsock-mod`、`crytropy/output-style-mod`、`crytropy/one-click-handoff` 裝的，先移除舊的，再照上面裝一次。不然會畫出兩份。

```
/plugin uninstall windsock-mod@windsock-mod
/plugin uninstall windsock-mod-ultra@windsock-mod
/plugin uninstall style@output-style-mod
/plugin uninstall one-click-handoff@one-click-handoff
/plugin marketplace remove windsock-mod
/plugin marketplace remove output-style-mod
/plugin marketplace remove one-click-handoff
```

改名的有：`windsock-mod` → `windsock`、`windsock-mod-ultra` → `windsock-ultra`、`style` → `output-style`。`/style` 指令沒變。

## 開發

```
claude plugin validate .
claude plugin validate <資料夾>
claude plugin test <資料夾>
```
