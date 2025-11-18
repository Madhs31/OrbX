# 🌍 OrbX --- Repositório Principal

Este é o repositório **raiz** do projeto **OrbX**, contendo toda a
estrutura principal da aplicação, organizada em dois submódulos Git:

-   **OrbX_Backend** → API e servidor\
-   **OrbX_Frontend** → Interface web em React

O OrbX tem como objetivo fornecer uma plataforma composta por dados
geográficos, mapas dinâmicos e visualização estruturada de países,
cidades e regiões.

## 📁 Estrutura do Repositório

Este repositório usa **Git Submodules** para separar as partes do
projeto:

    OrbX/
     ├─ OrbX_Backend/      # Submódulo → https://github.com/Madhs31/OrbX_Backend
     └─ OrbX_Frontend/     # Submódulo → https://github.com/Madhs31/OrbX_Frontend

## 🔧 Configurando o repositório após o clone

Como este projeto utiliza **submódulos**, após fazer o clone, você
precisa rodar:

``` bash
git submodule update --init --recursive
```

Ou clone já trazendo tudo junto:

``` bash
git clone --recursive https://github.com/Madhs31/OrbX.git
```

Se você esqueceu de usar `--recursive`, basta fazer:

``` bash
git submodule update --init
```

## 🚀 Subprojetos

### 🖥️ OrbX Frontend

Interface construída com **React + Vite**, consumindo dados por API e
exibindo mapas dinâmicos.\
Repositório: https://github.com/Madhs31/OrbX_Frontend

### 🛠️ OrbX Backend

API construída em **Node + TypeScript + Prisma**, responsável pelos
dados e lógica de negócio.\
Repositório: https://github.com/Madhs31/OrbX_Backend

## 📦 Como rodar localmente

### 1️⃣ Baixe o repositório principal

``` bash
git clone --recursive https://github.com/Madhs31/OrbX.git
cd OrbX
```

Se não usou `--recursive`, faça:

``` bash
git submodule update --init --recursive
```

## ▶️ Executando o Backend

``` bash
cd OrbX_Backend
npm install
npm run dev
```

## 🌐 Executando o Frontend

``` bash
cd OrbX_Frontend
npm install
npm run dev
```

## 🔄 Atualizando submódulos

``` bash
git submodule update --remote
```

Ou individualmente:

``` bash
cd OrbX_Backend
git pull origin master
```
