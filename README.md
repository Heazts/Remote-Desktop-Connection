[![Windows 11 • 10](https://img.shields.io/badge/Windows-11%20%E2%80%A2%2010-0078D4?style=for-the-badge&logo=windows&logoColor=white)](https://www.microsoft.com/pt-br/windows)
[![Arquitetura 64 bits (x64)](https://img.shields.io/badge/Arquitetura%2064%20bits-x64-6354CC?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/Heazts/Remote-Desktop-Connection/releases)
[![Tamanho](https://img.shields.io/badge/Tamanho-266%20KB-00D26A?style=for-the-badge)](https://github.com/Heazts/Remote-Desktop-Connection/releases)
[![Licença Microsoft Original](https://img.shields.io/badge/Licen%C3%A7a-Microsoft%20Original-8C8C8C?style=for-the-badge&logo=microsoft&logoColor=white)](https://www.microsoft.com)

# MSTSC – Cliente de Área de Trabalho Remota (mstsc.exe) para Windows 11/10

Algumas instalações do Windows 11 (e também do Windows 10) simplesmente não possuem mais o executável clássico **mstsc.exe**, localizado em `C:\Windows\System32`.  
Mesmo com o recurso “Cliente de Área de Trabalho Remota” marcado como instalado, o binário pode desaparecer sem explicação clara.

Em meu caso, o mstsc havia sumido completamente. Tentei tudo:
- Recursos opcionais
- SFC /scannow
- DISM
- Até IAs

Nada funcionou. A solução definitiva veio com um instalador oficial da Microsoft preservado pelo site **IT Trip** e arquivado na Wayback Machine.

---

## O que contém este repositório

- `Remote-Desktop-Connection-Installer.exe` → instalador oficial 64-bit da Microsoft (versão 10.0.25989.1000)  
- Restaura automaticamente `mstsc.exe`, `mstscax.dll` e todas as dependências  
- Funciona no Windows 11 (todas as builds), Windows 10 e Insider  
- Instalação offline e silenciosa  

---

## Download

[![Download](https://img.shields.io/badge/DOWNLOAD%20MSTSC%2064--bit-0066CC?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/Heazts/Remote-Desktop-Connection/blob/6baaab6744fea979c88d3e1c94d1efb9bfb71346/Remote-Desktop-Connection-Installer.exe)

---

## Verificação de segurança

**SHA-256 oficial:**

`5F8D6C736CAAB6BFBB9A1AE3897781B8694EA8607750AA192AADA8DADBF7931`

**Como verificar no PowerShell:**
```powershell
Get-FileHash .\Remote-Desktop-Connection-Installer.exe -Algorithm SHA256
```

**Assinado digitalmente por Microsoft Corporation (válido)**

### Fontes oficiais

- 🇧🇷 **Guia completo em português** → [pt.ittrip.xyz → Reinstalar RDP no Windows 11](https://pt.ittrip.xyz/windows/rdp/reinstalar-rdc-win11)
- 🇺🇸 **Guia em inglês** → [en.ittrip.xyz → Reinstall RDC on Windows 11](https://en.ittrip.xyz/windows/rdp/rdc-reinstall-win11)
- 🏛️ **Arquivo original arquivado** → [Wayback Machine – Microsoft (2025)](https://web.archive.org/web/20250319121744/https://go.microsoft.com/fwlink/?linkid=2247659)
## Como instalar (2 minutos)

1. Baixe o arquivo da Release acima
2. Clique com botão direito → **Executar como administrador**
3. Aguarde a instalação silenciosa
4. Reinicie o PC (ou mate o `explorer.exe`)
5. `Win + R` → digite `mstsc` → **pronto!**


## Aviso importante
- Arquivo **100 % original** da Microsoft.
- Sempre verifique o hash antes de executar.
- Evite fontes não confiáveis.

## Créditos

- Microsoft (binário original)
- IT Trip (guia incrível que salvou milhares de pessoas)
- Internet Archive / Wayback Machine

Se te ajudou, deixa uma ⭐ – ajuda quem está na mesma situação a encontrar rápido!
