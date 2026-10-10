<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=220&section=header&text=M8%204G&fontSize=80&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=MediaTek%20%E2%80%A2%20Tablet%20%E2%80%A2%20Hack%20%E2%80%A2%20Root%20%E2%80%A2%20Linux&descAlignY=60&descSize=18" width="100%" alt="banner M8 4G"/>

<a href="https://github.com/">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=00E5FF&center=true&vCenter=true&width=700&lines=Tablet+MediaTek+M8+4G+%F0%9F%93%B1;Flash+%7C+Unbrick+%7C+Root+%7C+Linux+%F0%9F%90%A7;Tudo+documentado+e+open+source+%F0%9F%9A%80" alt="Typing SVG" />
</a>

<br/>

![Plataforma](https://img.shields.io/badge/Plataforma-MediaTek-FF6F00?style=for-the-badge&logo=mediatek&logoColor=white)
![Android](https://img.shields.io/badge/Android-Root-3DDC84?style=for-the-badge&logo=android&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-Alpine%20chroot-0D597F?style=for-the-badge&logo=alpinelinux&logoColor=white)
![Termux](https://img.shields.io/badge/Termux-Ready-000000?style=for-the-badge&logo=termux&logoColor=white)

![Stars](https://img.shields.io/github/stars/SEU_USUARIO/m8_4g?style=for-the-badge&color=ffd700&logo=github)
![Forks](https://img.shields.io/github/forks/SEU_USUARIO/m8_4g?style=for-the-badge&color=00c7ff&logo=github)
![Issues](https://img.shields.io/github/issues/SEU_USUARIO/m8_4g?style=for-the-badge&color=ff4d6d&logo=github)
![License](https://img.shields.io/github/license/SEU_USUARIO/m8_4g?style=for-the-badge&color=8a2be2)

<br/>

**[📖 Sobre](#-sobre) • [📱 Aparelho](#-sobre-o-aparelho) • [🛠️ Ferramentas](#️-ferramentas) • [⚡ Guia rápido](#-guia-rápido) • [🐧 Linux](#-linux-no-m8-4g) • [🖼️ Screenshots](#️-screenshots) • [🤝 Contribuir](#-contribuindo)**

</div>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:00e5ff,100:8a2be2&height=3" width="100%" alt="divisor"/>

## ✨ Sobre

> **M8 4G** é um tablet baseado em **MediaTek**. Este repositório reúne tudo o que é necessário para **entender, restaurar, modificar e dar uma segunda vida** ao aparelho — de forma simples e direta.

<table>
<tr>
<td width="33%" align="center">

### 🔧 Restaurar
Formatar partições e recuperar o aparelho quando ele travar.

</td>
<td width="33%" align="center">

### 🔓 Customizar
Root, ajustes de sistema e kernel.

</td>
<td width="33%" align="center">

### 🐧 Linux
Rodar **Alpine Linux** em chroot direto no Android.

</td>
</tr>
</table>

## 📱 Sobre o aparelho

<div align="center">

<img src="https://placehold.co/700x380/0f2027/00e5ff?text=Foto+do+M8+4G&font=montserrat" width="70%" alt="Foto do M8 4G"/>

</div>

| 🧩 Item | 📋 Detalhe |
|:--|:--|
| **Modelo** | M8 4G |
| **Chipset** | MediaTek |
| **Conectividade** | 4G LTE + Wi-Fi |
| **Arquitetura** | aarch64 (ARM64) |
| **RAM / Armazenamento** | _preencher_ |
| **Versão do Android** | _preencher_ |

> 💡 Edite a tabela acima com as especificações reais do seu aparelho.

## 🛠️ Ferramentas

<div align="center">

| Ferramenta | Para que serve |
|:--:|:--|
| ![mtkclient](https://img.shields.io/badge/mtkclient-00E5FF?style=flat-square&logo=python&logoColor=black) | Ler, apagar e gravar partições em chips MediaTek |
| ![Termux](https://img.shields.io/badge/Termux-000000?style=flat-square&logo=termux&logoColor=white) | Terminal no próprio Android |
| ![Magisk](https://img.shields.io/badge/Magisk%20%2F%20KernelSU-00AF9C?style=flat-square&logo=magisk&logoColor=white) | Acesso root |
| ![Alpine](https://img.shields.io/badge/Alpine%20Linux-0D597F?style=flat-square&logo=alpinelinux&logoColor=white) | Linux leve rodando em chroot |

</div>

## ⚡ Guia rápido

### 1️⃣ Clonar o repositório

```bash
git clone https://github.com/SEU_USUARIO/m8_4g.git
cd m8_4g
```

### 2️⃣ Instalar o mtkclient

```bash
git clone https://github.com/bkerler/mtkclient.git
cd mtkclient
pip install -r requirements.txt
```

### 3️⃣ Limpar partições de usuário

> [!WARNING]
> Esta etapa **apaga todos os seus dados**. Faça backup antes de continuar.

```bash
python mtk.py e userdata
python mtk.py e cache
python mtk.py e metadata
python mtk.py e frp
```

Com o aparelho **desligado**, conecte o cabo USB quando o `mtkclient` pedir.

> [!TIP]
> Sem PC por perto? Dá para rodar o `mtkclient` pelo **Termux** com root.

## 🐧 Linux no M8 4G

Rode **Alpine Linux** em chroot, com acesso root via Magisk ou KernelSU:

```bash
# Exemplo de estrutura
/data/local/alpine
```

- 🪶 Leve e rápido
- 🔗 Bind-mount dos diretórios do Android (`/sdcard`, `/data` etc.)
- 🖥️ Ideal para ferramentas de linha de comando e desenvolvimento

## 🖼️ Screenshots

<div align="center">

<img src="https://placehold.co/260x420/0f2027/00e5ff?text=Tela+1&font=montserrat" width="24%" alt="Screenshot 1"/>
<img src="https://placehold.co/260x420/203a43/8a2be2?text=Tela+2&font=montserrat" width="24%" alt="Screenshot 2"/>
<img src="https://placehold.co/260x420/2c5364/ff6f00?text=Tela+3&font=montserrat" width="24%" alt="Screenshot 3"/>

</div>

> 📸 Troque os placeholders por prints reais salvos em uma pasta `assets/` do repositório.

## 🗂️ Estrutura do projeto

```text
m8_4g/
├── 📄 README.md
├── 📁 assets/        # imagens e screenshots
├── 📁 scripts/       # scripts de apoio
├── 📁 docs/          # guias e anotações
└── 📜 LICENSE
```

## 🤝 Contribuindo

Contribuições são muito bem-vindas!

1. 🍴 Faça um **fork**
2. 🌿 Crie uma branch: `git checkout -b minha-melhoria`
3. 💾 Commit: `git commit -m "Minha melhoria"`
4. 📤 Push: `git push origin minha-melhoria`
5. 🔁 Abra um **Pull Request**

## ⚠️ Aviso

> Modificar o aparelho pode **anular a garantia** e, se feito de forma errada, causar **brick**. Tudo aqui é fornecido **sem garantia** — use por sua conta e risco.

## 📜 Licença

Distribuído sob a licença **MIT**. Veja o arquivo `LICENSE` para mais detalhes.

<div align="center">

<br/>

### ⭐ Gostou? Deixe uma estrela!

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,50:203a43,100:0f2027&height=120&section=footer" width="100%" alt="rodapé"/>

</div>
