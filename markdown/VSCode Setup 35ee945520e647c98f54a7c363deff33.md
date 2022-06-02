# VSCode Setup

## Theme

Tên: Atom Background Modified

Link: [https://marketplace.visualstudio.com/items?itemName=NAPTheDevHcj.atom-background-modified](https://marketplace.visualstudio.com/items?itemName=NAPTheDevHcj.atom-background-modified)

## Icon Theme

Tên: Material Icon Theme

Link: [https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)

## Font

Tên: Jetbrains Mono

Link: [https://www.jetbrains.com/lp/mono/](https://www.jetbrains.com/lp/mono/)

Settings VSCode:

```json
{
	"editor.fontSize": 14,
  "editor.fontFamily": "Jetbrains Mono",
  "editor.fontLigatures": true,
}
```

## Extensions

- Auto Rename Tag
- Code Spell Checker
- Codesnap (copy ảnh màn hình code đẹp)
- ESLint (linting, gợi ý cho js, ts)
- Import Cost (hiển thị import size)
- Prettier
- sort-imports (format thứ tự import trong js, jsx, ts, tsx, hoạt động tốt với prettier)
- Tabout (dùng tab để next ra khỏi các cái ngoặc, để tránh phải di chuyển tay bấm vào nút mũi tên phải)
- Tailwind CSS Intellisense
- Thunder Client (test api và http request, giống hệt postman, nhưng là extension)
- HTML CSS Support (Gợi ý css class cho html, thích hợp nếu code bootstrap trong html)

## Settings

```json
{
	// wrap mấy tab file ở phía trên
	"workbench.editor.wrapTabs": true,

	// cực kì hữu ích khi dùng snippet, vẫn bật autocomplete
  "editor.suggest.snippetsPreventQuickSuggestions": false,

	// nên để tab size bằng 2 thay vì 4
  "editor.tabSize": 2,

	// cursor smooth hơn
  "editor.cursorSmoothCaretAnimation": true,
  "editor.cursorBlinking": "smooth",

	// đặt default formatter là prettier
  "editor.defaultFormatter": "esbenp.prettier-vscode",

	// tắt cái hỏi workspace trust mỗi khi mở folder mới
  "security.workspace.trust.enabled": false,

	// format khi save
  "editor.formatOnSave": true,

	// chỉnh title của vscode phía trên theo ý thích
  "window.title": "😎 ${rootPath} 😎",

	// tốt hơn autosave thường, vì nó sẽ chỉ save khi alt + tab chuyển sang cửa sổ khác
  "files.autoSave": "onWindowChange",

	// thay thế cho bracket pair colorizer
  "editor.bracketPairColorization.enabled": true,
  "editor.guides.bracketPairs": true,

	// linting cho javascript, cực kì hữu ích
	"js/ts.implicitProjectConfig.checkJs": true,
}
```