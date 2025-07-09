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

- 🪙 **TokenA**: [`0x436Dee1cb61c53739cf64717508f97E512a0608A https://sepolia.etherscan.io/token/0x436dee1cb61c53739cf64717508f97e512a0608a#code`  ]
- 🪙 **TokenB**: [`0x9FAfB9DeD27ccAe20F4C7d55A6a6158C41eE74AF  https://sepolia.etherscan.io/address/0x9FAfB9DeD27ccAe20F4C7d55A6a6158C41eE74AF#code` ]
- 🔁 **SimpleDEX**: [`0xEd152fC19C23DD94f029AbEC4f4Fb3ffA53B41cb https://sepolia.etherscan.io/address/0xEd152fC19C23DD94f029AbEC4f4Fb3ffA53B41cb#code`]

---

### 🛠️ Tecnologías

- Solidity `^0.8.22`
- Remix + MetaMask + Scroll Sepolia testnet



---

### 📄 Licencia

MIT
