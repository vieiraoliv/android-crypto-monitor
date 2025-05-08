# 📱 Crypto Monitor

Aplicativo Android desenvolvido em Kotlin para exibir informações atualizadas sobre a cotação do **Bitcoin**, utilizando a API pública do [Mercado Bitcoin]. O app apresenta de forma simples e funcional o valor mais recente da criptomoeda.

---

## 🧪 Tecnologias Utilizadas

- **Kotlin**
- **Retrofit** (consumo de API REST)
- **Kotlin Coroutines** (requisições assíncronas)
- **Material Design**
- **Android SDK**
- **View System Tradicional** (TextView, Button, Toolbar)


## 🎯 Funcionalidades

- Consulta da cotação atual do Bitcoin.
- Exibição do valor atualizado na tela principal.
- Botão de atualização manual (Refresh).
- Exibição do horário da última atualização.
- Interface simples e objetiva.


Tela antes da atualização do valor através do botão "atualizar".


![image](https://github.com/user-attachments/assets/73d27353-f84e-4623-b085-19d93936925b)

Tela depois da atualização do valor.


![image](https://github.com/user-attachments/assets/83c69662-bc27-4fe5-955f-73607195c563)



## 🔗 API Utilizada

O app consome dados da seguinte URL:
https://www.mercadobitcoin.net/api/BTC/ticker/


A resposta da API é tratada pelo modelo `TicketResponse.kt`, exibindo os dados diretamente ao usuário.
```
class TickerResponse(
    val ticker: Ticker
)

class Ticker(
    val high: String,
    val low: String,
    val vol: String,
    val last: String,
    val buy: String,
    val sell: String,
    val date: Long
)
```
## 🛠 Como Executar o Projeto

1. Clone ou baixe este repositório:

    ```bash
   git clone https://github.com/seuusuario/android-crypto-monitor.git

   ```
2. Abra o projeto no Android Studio.

3. Aguarde o carregamento do Gradle e as dependências.

4. Execute em um emulador ou dispositivo físico com Android 5.0+.


