# backup-config_starship

Este repositório contém backups de arquivos de configuração para o [Starship](https://starship.rs/), um prompt de terminal rápido e customizável.

## 🧑‍💻 Minha Configuração (Álvaro)

A configuração principal e mantida por mim para o meu uso diário e fluxo de trabalho:
* **`starship-alvaro.toml`**: Configuração pessoal e atual do Álvaro, com estilo Powerline e módulos organizados.
* **`starship-legacy.toml`**: Versão antiga/legada da minha configuração para histórico.

## 🌐 Configurações da Comunidade (Encontradas no Git)

Coleção de configurações de outros desenvolvedores que encontrei navegando pelo GitHub e outras plataformas. Excelentes para referência, estudo e inspiração:

* **`starship-theme-arch-os.toml`**: Baseado no repositório murkl/starship-theme-arch-os. Um tema estilo Powerline em linha única usando as cores do Nord Theme, focado no Arch Linux.
* **`starship-profile.toml`**: Baseado no repositório Firi0n/starship-profile. Um prompt de múltiplas linhas muito completo (layout em grade), que exibe desde a bateria do sistema até ícones bem específicos de várias linguagens de programação.

## 🧠 Entendendo as Configurações

Os arquivos `.toml` do Starship são bastante legíveis e modulares. Ao abrir qualquer uma das configurações deste repositório, você geralmente encontrará os seguintes blocos:

* **`format` / `right_format`**: Define a estrutura e o layout do prompt. É aqui que você controla a ordem exata em que as informações aparecem.
* **Módulos (ex: `[directory]`, `[git_status]`)**: Cada bloco entre colchetes personaliza uma informação específica. Dentro deles, você altera ícones (`symbol`), cores (`style`) e regras de quando aquele módulo deve aparecer.
* **`[character]`**: Configura o símbolo do cursor de digitação (geralmente `❯`, `$` ou `➜`). Ele pode mudar de cor dependendo se o último comando teve sucesso ou falhou.
* **Paletas de Cores (`[palettes]`)**: Alguns arquivos mais avançados definem esquemas de cores próprios. Isso facilita a criação de temas (como Dracula, Catppuccin, etc.) mapeando nomes de cores para códigos HEX.

## 🚀 Como Usar

Para testar ou usar qualquer uma das configurações listadas acima, copie o arquivo desejado para a pasta de configuração do seu usuário, renomeando-o para `starship.toml`:

```bash
# Exemplo copiando a minha configuração
cp starship-alvaro.toml ~/.config/starship.toml
```
