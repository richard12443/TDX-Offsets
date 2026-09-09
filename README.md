# TDX-Offsets

Offsets do Roblox para o auto-update do TDX External.

## Como atualizar quando o Roblox atualiza

1. Rode o `roblox-dumper.exe` com o Roblox aberto (de preferência dentro de um jogo)
2. Pegue o `offsets.json` gerado
3. Substitua o `offsets.json` deste repositório pelo novo (confira que `metadata.roblox_version` bate com a versão nova do client)
4. Commit + push — o cheat baixa sozinho na próxima abertura, sem precisar recompilar

```powershell
Copy-Item "D:\TDX ROBLOX\TDX ROBLOX\offsets.json" ".\offsets.json" -Force
git add offsets.json
git commit -m "offsets version-XXXX"
git push
```

O painel só aceita o JSON se `metadata.roblox_version` for igual à versão do Roblox instalado.
