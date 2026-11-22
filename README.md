# 01_Setup_Entorno

1. Instala Node y NPM
2. Inicializa un nuevo proyecto de node e instala jest
```bash
npm init -y
npm install --save-dev jest
```
3. Modifica `package.json` para que incluya este comando `test`:
```json
"scripts": {
  "test": "jest"
}
```
4. Crea un archivo `sumar.test.ts` y agrega este contenido
```typescript
test('prueba falsa', () => {
  expect(true).toBe(true);
});
```
5. Ejecuta la prueba con teste comando
```bash
npm test
```

La prueba usa TypeScript, por lo que también se instalaron `typescript`,
`ts-jest` y `@types/jest`. La configuración está en `jest.config.js` y
`tsconfig.json`. Las dependencias se guardan en `node_modules`, una carpeta
local que no se sube a GitHub.

Al finalizar, toma una captura de la terminal donde se vea el resultado y
entrega esa captura según las instrucciones de la actividad.
