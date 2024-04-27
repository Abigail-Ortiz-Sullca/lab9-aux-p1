# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Install & Run
- yarn 
- yarn dev

# Adaptación al uso de TypeScript

Este proyecto está configurado para utilizar TypeScript (`.tsx`) en lugar de JavaScript (`.jsx`). Esto permite explotar las ventajas que ofrece TypeScript, como la definición de tipos y la seguridad de tipo en tiempo de compilación.

## Definición de tipos para Product

En TypeScript, se establece un tipo para `Product` que define sus propiedades y los tipos de datos que estas pueden tener. Aquí tienes un ejemplo de esta definición:

```typescript
type Product = {
  id: number;
  title: string;
  description: string;
  price: number;
  brand: string;
};
# **Uso de TypeScript en el Proyecto**

Este proyecto utiliza TypeScript para facilitar la manipulación de objetos, en particular, los objetos `Product`. Esto asegura que siempre se esté trabajando con las propiedades correctas y proporciona funcionalidades de autocompletado y sugerencias de código en el editor, lo que puede simplificar la escritura del código y reducir la probabilidad de errores.

## **Implementación de useState y useEffect**

En este proyecto, se utilizan `useState` y `useEffect` de React en conjunto con TypeScript. Se pueden proporcionar anotaciones de tipo para los valores de estado y los parámetros de las funciones de efecto. Por ejemplo, en el componente `Card`, se anota el estado del producto de la siguiente manera:

```typescript
const [product, setProduct] = useState<Product | null>(null);


