# 🐧 Script de Provisionamento Linux - Infraestrutura de Diretórios e Usuários

Este repositório contém um script Bash para criar automaticamente a infraestrutura de usuários, grupos, diretórios e permissões em sistemas Linux. Ideal para uso em máquinas virtuais recém-instaladas.

## 📁 Estrutura Criada

### Diretórios:
- /publico
- /adm
- /ven
- /sec

### Grupos:
- GRP_ADM
- GRP_VEN
- GRP_SEC

### Usuários:
| Grupo     | Usuários                         |
|-----------|----------------------------------|
| GRP_ADM   | carlos, maria, joao_             |
| GRP_VEN   | debora, sebastiana, roberto      |
| GRP_SEC   | josefina, amanda, rogerio        |

## 🔐 Permissões
- Todos os diretórios são de propriedade do usuário root.
- O diretório /publico é acessível por todos (permissão 777).
- Cada diretório de grupo tem acesso exclusivo aos seus membros (permissão 770).
- Usuários de um grupo não têm acesso a diretórios de outros grupos.

## ▶️ Execução

Para rodar o script, use:

```bash
sudo bash provisionamento.sh
```

> **Importante:** A senha padrão dos usuários criados é Senha123.

## 📦 Requisitos

- Distribuição Linux com Bash
- Permissões de superusuário (root)
- OpenSSL instalado

## 🚀 Como usar

1. Clone o repositório:
   ```bash
   git clone https://github.com/opusvix/<nome-do-repositorio>.git
   cd <nome-do-repositorio>

2. Torne o script executável:
   ```bash
   chmod +x provisionamento.sh

3. Execute o script como root:
   ```bash
   sudo ./provisionamento.sh

🛠️ Autor
Desenvolvido por [opusvix](www.github.com/opusvix)



