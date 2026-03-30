# Tutorial para enviar e atualizar códigos no GitHub

Cada grupo deverá utilizar **apenas o seu próprio repositório no GitHub**.  
O projeto deve ser atualizado **ao longo do semestre**, e não apenas no final.

Os códigos podem ser enviados de **duas formas**:

- pelo **navegador (GitHub Web)**;
- pelo **VS Code ou outro editor com Git**.

---

## Opção 1 — Enviar e atualizar código pela versão Web do GitHub

### 1. Abrir o repositório do grupo

Entrar no GitHub e abrir o repositório correspondente ao grupo, por exemplo:

- `G1`
- `G7`
- `G12`



### 2. Fazer o primeiro envio dos arquivos

Na página principal do repositório:

1. clicar em **Add file**;
2. clicar em **Upload files**;
3. arrastar os arquivos para a página ou selecionar manualmente no computador.



### 3. Confirmar o envio

Depois de adicionar os arquivos:

1. descer até o final da página;
2. preencher a mensagem de commit, por exemplo:

```bash
Entrega parcial do projeto
```
Esse cuidado evita trabalhar em uma versão desatualizada do projeto. O VS Code oferece operações de fetch, pull e push na integração de controle de versão.

---

## Opção 2 — Enviar e atualizar código pelo VS Code ou outro editor

Indicada para quem vai programar com frequência. O VS Code possui integração nativa com Git e permite revisar alterações, preparar arquivos para commit, registrar commits e fazer push/pull sem depender apenas do terminal.

### 1. Clonar o repositório do grupo no computador

No repositório do GitHub, clicar em **Code** e copiar a URL do repositório.

No terminal, executar:

```bash
git clone https://github.com/poo-ee-2026-1/NOME-DO-REPOSITORIO.git
```
Depois entrar na pasta:

cd NOME-DO-REPOSITORIO

A lógica do GitHub é que o trabalho local seja publicado no repositório remoto por meio de commits e push.

2. Abrir a pasta no VS Code

Abrir a pasta clonada no VS Code. Quando o VS Code detecta que a pasta é um repositório Git, ele ativa automaticamente os recursos de controle de versão.

3. Criar ou alterar os arquivos do projeto

O grupo pode então criar e editar normalmente os arquivos do sistema, por exemplo:
```bash
main.cpp
Aluno.cpp
Aluno.h
Sistema.cpp
Sistema.h
README.md
```
4. Preparar e registrar as alterações

No VS Code, abrir a aba Source Control. O editor mostra os arquivos alterados. Depois:

```bash
revisar as mudanças;
clicar no + para preparar os arquivos;
escrever a mensagem de commit;
confirmar o commit.
```
O VS Code documenta exatamente esse fluxo de stage e commit pela interface.

5. Enviar as alterações para o GitHub

Após o commit, fazer o push. No VS Code, isso pode ser feito pela opção Push, pelo menu de ações, ou pelo ícone de sincronização. A documentação do VS Code informa que o push envia os commits locais para o repositório remoto.

Se o grupo preferir usar terminal dentro do VS Code ou em outro editor, o fluxo básico é:
```bash
git add .
git commit -m "Mensagem clara da alteração"
git push origin main
```
O GitHub documenta que o git push normalmente é feito com o remoto e a branch, como em git push origin main.

6. Atualizar o código antes de continuar trabalhando

Antes de começar novas alterações, o grupo deve baixar a versão mais recente do repositório. No VS Code isso pode ser feito por pull ou pela sincronização; no terminal:
```bash
git pull origin main
```
Esse cuidado evita trabalhar em uma versão desatualizada do projeto. O VS Code oferece operações de fetch, pull e push na integração de controle de versão.
