# SimpleDEX - Exchange Descentralizado con Fórmula del Producto Constante

Este proyecto implementa un **Exchange Descentralizado Simple (DEX)** que permite el intercambio entre dos tokens ERC-20 utilizando un contrato inteligente en Solidity.

### ✨ Características principales

- **Tokens ERC-20 personalizados**:  
  - `TokenA`: nombre `TokenA`, símbolo `TKA`  
  - `TokenB`: nombre `TokenB`, símbolo `TKB`

- **Contrato de intercambio** (`SimpleDEX`) que:
  - Permite añadir y retirar liquidez (solo el owner)
  - Permite intercambiar `TokenA` por `TokenB` y viceversa
  - Calcula precios automáticamente usando la **fórmula del producto constante**

---

### 📐 Fórmula del Producto Constante

La lógica del DEX está basada en la fórmula de mercado automatizado (AMM) utilizada por Uniswap v1:

\[
(x + dx) \cdot (y - dy) = x \cdot y
\]

Donde:
- `x`, `y` son las reservas de TokenA y TokenB
- `dx` es el monto de entrada
- `dy` es el monto de salida

---

### 📦 Contratos desplegados en Scroll Sepolia

- 🪙 **TokenA**: [`0x1236D8A9CEC13c4ba13464574297bbb1958cB033`]
- 🪙 **TokenB**: [`0x212fce43221e35b6FA4302f5C1a262850B34f105`]
- 🔁 **SimpleDEX**: [`0xA83eA4B94a93B68D33BF52c308cd64cACfec3758`]

---

### 🛠️ Tecnologías

- Solidity `^0.8.22`
- OpenZeppelin Contracts `^5.0.0`
- Remix + MetaMask + Scroll Sepolia testnet

---

### ✅ Objetivos académicos

Este proyecto fue desarrollado como parte de una práctica final para comprender:
- El funcionamiento básico de los exchanges descentralizados
- El modelo AMM con producto constante
- La interacción entre múltiples contratos inteligentes ERC-20

---

### 📄 Licencia

MIT
