# Número por extenso em React

Componente React que retorna número por extenso

## Como instalar

Abaixo as formas de como instalar essa biblioteca utilizando o npm ou yarn:

...
npm install number-extension-rogerlog
#ou
yarn add react-input-por-extenso

## Como usar

Uma forma básica de como utilizar o componente:

```jsx
import React, { useState } from "react";
import ReactDOM from "react-dom";
import ReactInputPorExtenso from "number-extension-rogerlog";

const App = () => {
  const [numero, setNumero] = useState("");
  return (
    <>
      <ReactInputPorExtenso
        tipoExtenso="monetario"
        onChange={numeroExtenso => setNumero(numeroExtenso)}
      />
      <p>
        <strong>Número por extenso</strong>: {numero}
      </p>
    </>
  );
};

ReactDOM.render(<App />, document.getElementById("root"));
```

## Propriedades

Esse componente é uma abstração de um componente input do tipo nmérico, 
todas as propriedades de um input estão disponíveis.

| Propriedade   | Valor Inicial |   Tipo    | Descrição                     |
| ------------- | ------------- | --------- | ----------------------------- |
| tipoExtenso   | normal        | string    | Formato de extensão do número |