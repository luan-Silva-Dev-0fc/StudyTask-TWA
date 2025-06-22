
# StudyTask-TWA

Este repositório contém o código e as configurações do projeto **StudyTask** transformado em um **Aplicativo Android Nativo** através do **Bubblewrap**, partindo de um **Progressive Web App (PWA)**.

## Passos Realizados

### 1. **Criação do PWA**
O projeto foi inicialmente desenvolvido como um **Progressive Web App (PWA)**. A ideia foi criar uma versão da aplicação que funcionasse de forma responsiva tanto em dispositivos móveis quanto em desktop, aproveitando os recursos de um PWA.

- A aplicação foi hospedada em:  
  [https://luan-silva-dev-0fc.github.io/StudyTask-PWA](https://luan-silva-dev-0fc.github.io/StudyTask-PWA)
  
- O **manifest.json** e outros recursos do PWA estão configurados para permitir a instalação e uso no navegador.

### 2. **Transformação do PWA em Aplicativo Android com Bubblewrap**
A partir do **PWA**, utilizamos o **Bubblewrap** para gerar um **APK** nativo para Android, seguindo os passos:

- **Instalação do Bubblewrap**:  
  Usamos o comando `npm install -g @bubblewrap/cli` para instalar o **Bubblewrap** e configurá-lo.
  
- **Iniciação do Projeto com Bubblewrap**:  
  O comando `bubblewrap init --manifest [URL do Manifesto]` foi usado para iniciar a criação do APK. Durante o processo, fornecemos as configurações do projeto, como nome do aplicativo, ID do pacote e modo de exibição.
  
- **Geração de APK**:  
  Após a configuração do Bubblewrap, geramos um **APK** para o projeto Android.

### 3. **Compilação e Ajustes no Android Studio**
O código foi então importado para o **Android Studio**, onde realizamos ajustes e compilamos o APK:

- **Importação do Projeto no Android Studio**:  
  Abrimos o projeto existente no **Android Studio** para realizar qualquer ajuste e verificar se tudo estava configurado corretamente.
  
- **Compilação do APK**:  
  Utilizamos o Android Studio para compilar o **APK** e gerá-lo para teste. O processo de compilação foi bem-sucedido e o APK foi gerado.

### 4. **Subida do Código para o GitHub**
O projeto foi versionado com **Git** e o código foi enviado para o GitHub para futuras alterações e controle de versão.

- O repositório do GitHub é:  
  [https://github.com/luan-Silva-Dev-0fc/StudyTask-TWA](https://github.com/luan-Silva-Dev-0fc/StudyTask-TWA)

### 5. **Criação de um Keystore e Assinatura do APK (Opcional)**
Caso necessário, seria possível criar uma chave de assinatura **(keystore)** para assinar o APK. Contudo, como o objetivo não é publicar o aplicativo na Play Store, essa etapa foi ignorada.

---

## Como Rodar o Projeto

Para rodar o projeto localmente, basta seguir os seguintes passos:

### 1. **Instalar Dependências**
Certifique-se de ter o **Node.js** e o **npm** instalados.

```bash
npm install
```

### 2. **Iniciar o Projeto**
Caso deseje rodar o PWA no navegador:

```bash
npm start
```

### 3. **Gerar o APK (Caso Deseje Compilar para Android)**
Para gerar o **APK** do aplicativo, siga os seguintes passos:

1. **Instale o **Bubblewrap**:
   ```bash
   npm install -g @bubblewrap/cli
   ```

2. **Inicie o processo de criação do APK** com o **Bubblewrap**:
   ```bash
   bubblewrap init --manifest https://luan-silva-dev-0fc.github.io/StudyTask-PWA/manifest.json
   ```

3. **Compile o APK** no **Android Studio**.

---

## Tecnologias Utilizadas

- **React** (para o desenvolvimento do PWA)
- **Bubblewrap** (para transformar o PWA em um aplicativo Android nativo)
- **Android Studio** (para compilar e gerar o APK)
- **Node.js e npm** (para gerenciamento de dependências)
- **Git** e **GitHub** (para controle de versão)

