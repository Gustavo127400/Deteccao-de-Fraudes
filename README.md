# 🔍 Online Payment Fraud Detection Dataset | Real-World Transactions 💳

## 📝 Descrição do Dataset

As transações fraudulentas são um desafio crescente para empresas de fintech. Este dataset contém mais de **51.000 transações**, cada uma rotulada como **fraudulenta** ou **legítima**, com base em padrões do mundo real.

---

## 📊 Visão Geral das Colunas

### Detalhes da Transação:
- **Transaction_Amount**: Valor da transação (float)
- **Transaction_Type**: Tipo de transação (categórico)
- **Time_of_Transaction**: Horário da transação (float)
- **Payment_Method**: Método de pagamento utilizado (categórico)

### Comportamento do Usuário:
- **User_ID**: Identificação do usuário (int)
- **Previous_Fraudulent_Transactions**: Número de transações fraudulentas anteriores (int)
- **Account_Age**: Idade da conta em dias (int)
- **Number_of_Transactions_Last_24H**: Número de transações nas últimas 24 horas (int)

### Dispositivo e Localização:
- **Device_Used**: Dispositivo utilizado para a transação (categórico)
- **Location**: Localização da transação (categórico)

## 🔧 Pré-processamento Realizado

Para garantir a qualidade dos dados, foram realizadas as seguintes etapas de pré-processamento:

1. **Valores Ausentes**:
   - `Transaction_Amount`: Preenchido com a **mediana** (robusto contra outliers).
   - `Time_of_Transaction`: Preenchido com a **média** (consistência do tempo médio).
   - `Device_Used` e `Location`: Preenchidos com **'Unknown'** (valores categóricos ausentes).
   - `Payment_Method`: Preenchido com a **moda** (valor mais frequente).

---

## 📂 Como Usar

1. **Clone o repositório**:
   ```bash
   git clone https://github.com/Gustavo127400/Deteccao-de-Fraudes.git
