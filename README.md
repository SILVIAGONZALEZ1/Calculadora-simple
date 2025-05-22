# Calculadora-simple
Este es un proyecto de calculadora simple, creado en el curso trilogia web

````markdown
# 📱 Calculadora Web Simple

Una calculadora básica hecha con HTML, CSS y JavaScript puro. Permite realizar operaciones matemáticas simples como suma, resta, multiplicación y división, además de borrar un solo carácter o reiniciar el cálculo.

## 🚀 Funcionalidades

- ✅ Operaciones matemáticas básicas (`+`, `-`, `*`, `/`)
- 🔄 Botón "AC" para borrar todo
- ⬅️ Botón "DE" para borrar un solo carácter
- 🟰 Botón "=" para calcular el resultado

## 🧠 Lógica Principal (JavaScript)

```js
buttons.forEach((btn) => {
  btn.addEventListener("click", () => {
    if (btn.id === "=") {
      display.value = eval(display.value);
    } else if (btn.id === "ac") {
      display.value = "";
    } else if (btn.id == "de") {
      display.value = display.value.slice(0, -1);
    } else {
      display.value += btn.id;
    }
  });
});
````

## 📂 Estructura de Archivos

```
/calculadora
│
├── index.html     # Interfaz principal
├── style.css      # Estilos de la calculadora
└── script.js      # Lógica de la calculadora
```

## 🛠️ Requisitos

Solo necesitas un navegador moderno. No se requieren dependencias externas.

## ▶️ Cómo usar

1. Clona el repositorio o descarga los archivos.
2. Abre `index.html` en tu navegador.
3. ¡Empieza a calcular!

## ⚠️ Advertencia

Este proyecto utiliza `eval()` para calcular la expresión matemática. En aplicaciones reales se recomienda evitar `eval()` por razones de seguridad.

## 📄 Licencia

Este proyecto es de uso libre para fines educativos y personales.

![Calculadora](https://github.com/user-attachments/assets/55253bd1-f15c-468b-8b52-ad1f6afaf8d6)

