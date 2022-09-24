# StellarEasyLaboratory Boilerplate

Esta aplicación StellarEasyLaboratory es una colección repetitiva de funciones básicas de Stellar. Puede piratear este proyecto [Stencil](https://stenciljs.com) en lo que sea que esté tratando de construir o simplemente cortar y pegar las funciones desde aquí en su propio proyecto.

This StellarEasyLaboratory app is a boilerplate collection of basic Stellar functions. You can either hack this [Stencil](https://stenciljs.com) project into whatever you're trying to build or just cut and paste out the functions from here into your own project.


## Getting Started

To start building with this project clone this repo and install the deps:

```bash
npm i
```

and run:

```bash
npm start
```

To build the app for production, run:

```bash
npm run build
```

## [Stellar Functions](https://github.com/tyvdh/hack-stellar/blob/master/src/components/app-home/app-home.tsx#L48-L176) Featured in this Boilerplate

```ts
keypairGenerate() {}
```
Método de generador de par de claves Stellar muy simple. Hay muchas maneras de generar pares de llaves Stellar válidos, pero si todo lo que está buscando es un par de llaves rápido y aleatorio, este es el método para usted.
Dead simple Stellar keypair generator method. There are lots of ways to generate valid Stellar keypairs but if all you're looking for is a quick random keypair this is the method for you.

```ts
async accountFund() {}
```
Mientras que en testnet tenemos un pequeño y elegante método de servidor friendbot al que podemos llamar para pagarnos 10,000 XLM. Una vez que esté en un entorno de producción, deberá usar un método `accountPay` para poder crear y financiar las cuentas. Esta es solo una forma rápida de iniciar su entorno de prueba.
While on testnet we have a fancy little friendbot server method we can call to pay ourselves 10,000 XLM. Once you're in a production environment you'll need to use an `accountPay` method in order to get accounts created and funded. This is just a quick way to boot up your testing environment.

```ts
async accountUpdate() {}
```
Una vez que tenemos una cuenta financiada activa en el libro mayor, podemos llamar a esa cuenta y OBTENER su estado actual. Comprensiblemente, hay muchos datos en un objeto de cuenta, por lo que es probable que desee [repasar estos campos] (https://www.stellar.org/developers/guides/concepts/accounts.html)
Once we have a funded account live on the ledger we can call that account and GET its current state. There's lots of data in an account object understandably so you'll likely want to [brush up on these fields](https://www.stellar.org/developers/guides/concepts/accounts.html).

```ts
async accountCreate() {}
```
Una operación de transacción central de Stellar es la creación de nuevas cuentas. Es como una operación de pago, excepto que siempre es XLM y siempre financia cuentas nuevas que no existen en el libro mayor.
A core Stellar transaction operation is creating new accounts. It's just like a payment operation except it's always XLM and always funding new accounts which don't exist on the ledger.


```ts
async accountPay() {}
```
Otra operación central de las transacciones de Stellar es realizar pagos. En este método estamos pagando 100 XLM a la cuenta que acabamos de crear con 10 XLM iniciales. El siguiente paso sería explorar [activos personalizados](https://www.stellar.org/developers/guides/concepts/assets.html) para que pueda realizar y recibir pagos en activos que no sean el XLM nativo.
Another central operation of Stellar transactions is making payments. In this method we're paying 100 XLM to the account we just created with an intial 10 XLM. The next step would be to explore [custom assets](https://www.stellar.org/developers/guides/concepts/assets.html) so you can make and receive payments in assets other than the native XLM.

---

### Help links:
#### Docs
- [https://www.stellar.org/developers](https://www.stellar.org/developers)
- [https://stellar.github.io/js-stellar-sdk](https://stellar.github.io/js-stellar-sdk/)
- [https://github.com/stellar/js-stellar-sdk](https://github.com/stellar/js-stellar-sdk)
#### Explore
- [https://stellar.expert](https://stellar.expert/)
- [https://stellarbeat.io](https://stellarbeat.io/)
- [https://www.stellar.org/laboratory](https://www.stellar.org/laboratory/)
#### Wallets
- [https://solarwallet.io](https://solarwallet.io/)
- [https://testnet.interstellar.exchange](https://testnet.interstellar.exchange/)
- [https://stellarterm.com/testnet](https://stellarterm.com/testnet)
