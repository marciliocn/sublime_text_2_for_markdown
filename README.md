# Dicas para Sublime Text 2 e MarkDown

Este é um conjunto de dicas para a instalação do Sublime Text 2 otimizado para a linguagem MarkDown

## Instalação no ubuntu

```bash
sudo add-apt-repository ppa:webupd8team/sublime-text-2
sudo apt-get update
sudo apt-get install sublime-text
```

## Instalar o corretor ortográfico em português com o melhor dicionário

- Clone deste projeto ou click em `Download ZIP`
- Copie o conteúdo da pasta `Languages` para `~/.config/sublime-text-2/Packages/` 
- No Sublime Text, acesse: `View > Dictionary > Languages > pt_br > Portuguese(Brazilian)`
- Use F6 para habilitar/desabilitar o spell check

## Instalar o Package Control

- Ele será necessário para instalar os demais packages
- Acesse https://packagecontrol.io/installation
- Escolha a aba de acordo com a versão do Sublime
- Copie o texto da instalação
- Volte ao Sublime Text, abra um terminal: `View > Show Console`
- Cole o texto e aguarde a instalação.
- Talvez seja necessário reiniciar o Sublime algumas vezes

## Instalar os pacotes

Instale os seguintes pacotes

- ctrl shif p, escolha Install Package, escolha:
- Markdown Editing
- Monokai Extended

Escolha o tema Markdown Extended através Set Syntax. 

Abra `Preferences > Package Settings > MrkDown Editing > Markdown GFM Settings - User`

E configure o color_scheme:

```json
{
    "color_scheme": "Packages/Monokai Extended/Monokai Extended.tmTheme",
    "draw_centered": true,
    "wrap_width": 40,
    "word_wrap": true,
    "line_numbers": true
}
```

## Outras operações úteis

Instale o tema Soda, e configure o seu Settings-User com a entrada: `"theme": "Soda Dark.sublime-theme"`. Assim que instalar e configurar, as abas estarão estranhas, basta reiniciar.

## Outros plugins essenciais

- git
- GitGutter
- EMMET
- JavaScriptNext (javascript com ECMAScript 6)
- Clipboard History  (CTRL+ALT+V pra ver a lista)

## Mais dicas

Identar o código com F12 (Preferences > Key bindings - User) :

```json
{
 "keys": ["f12"], "command": "reindent", "args": {"single_line": false} 
}  
```



