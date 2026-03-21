# 📱 Kotlin Navigation App

Aplicativo Android desenvolvido em **Kotlin** utilizando **Jetpack Compose** e navegação entre telas.

## 🚀 Sobre o Projeto

Este projeto demonstra a implementação de navegação entre múltiplas telas em um aplicativo Android moderno. Ele simula um fluxo básico de aplicativo com:

* Tela de login
* Menu principal
* Tela de pedidos
* Tela de perfil

O objetivo é servir como exemplo prático de uso de **Navigation** com **Jetpack Compose**, seguindo boas práticas de organização de código.

---

## 🛠️ Tecnologias Utilizadas

* **Kotlin**
* **Android Studio**
* **Jetpack Compose**
* **Navigation Compose**
* **Gradle (KTS)**

---

## 📂 Estrutura do Projeto

```
app/
 └── src/main/java/.../navigation/
      ├── MainActivity.kt
      ├── screens/
      │    ├── LoginScreen.kt
      │    ├── MenuScreen.kt
      │    ├── PedidosScreen.kt
      │    └── PerfilScreen.kt
      └── ui/theme/
           ├── Color.kt
           ├── Theme.kt
           └── Type.kt
```

### 🔹 Principais Arquivos

* **MainActivity.kt**
  Responsável por configurar a navegação entre as telas.

* **LoginScreen.kt**
  Tela inicial do app (login do usuário).

* **MenuScreen.kt**
  Tela principal com opções de navegação.

* **PedidosScreen.kt**
  Exibe informações relacionadas a pedidos.

* **PerfilScreen.kt**
  Mostra dados do perfil do usuário.

---

## ▶️ Como Executar o Projeto

1. Clone o repositório:

```bash
git clone <url-do-repositorio>
```

2. Abra no **Android Studio**

3. Aguarde o Gradle sincronizar

4. Execute o app em um emulador ou dispositivo físico

---

## 🔄 Fluxo de Navegação

O aplicativo segue o seguinte fluxo:

```
Login → Menu → (Pedidos | Perfil)
```

* Após o login, o usuário é direcionado ao menu
* A partir do menu, pode navegar entre as telas disponíveis

---

## 📚 Objetivo Educacional

Este projeto foi criado com foco em:

* Aprender navegação no Jetpack Compose
* Estruturar aplicações Android modernas
* Separar responsabilidades por telas (screens)

---
## Capturas de tela
<img width="225" height="509" alt="image" src="https://github.com/user-attachments/assets/cd4aaa6a-c8a1-4ca6-8213-f84c4efa88bd" />
<img width="219" height="511" alt="image" src="https://github.com/user-attachments/assets/0ba51033-f557-4c6b-9ba1-4ac0b2ed8590" />
<img width="226" height="506" alt="image" src="https://github.com/user-attachments/assets/4ad47c33-9fc0-4834-83a2-5875f5fb3c4b" />
<img width="227" height="509" alt="image" src="https://github.com/user-attachments/assets/7992e53e-ec15-4b1d-b6aa-6e21a73500c0" />

## 👩‍💻 Autora

Desenvolvido por **Carol Rocha França**
