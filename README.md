# Kuali Muebles — Sitio Web

## Estructura
```
/
├── index.html          Página principal (catálogo)
├── producto.html       Página de producto individual
├── productos.json      Base de datos de productos
├── vercel.json         Configuración de Vercel
├── imgs/               Imágenes de productos
│   ├── logo-kuali.png
│   ├── ropero-amigo.png
│   ├── placeholder.jpg
│   └── [id-producto]-[n].jpg
└── README.md
```

## Cómo agregar un producto
1. Agregar la entrada en `productos.json`
2. Subir la imagen a `/imgs/` con el nombre `[id]-1.jpg`, `[id]-2.jpg`, etc.
3. Hacer deploy en Vercel

## Conectar al ERP (cuando esté listo)
En `index.html` y `producto.html` busca el comentario:
```
// Para conectar al ERP, cambiar la URL a:
//   const DATA_URL = 'https://api.kualimuebles.com/api/productos';
```
Descomenta esa línea y comenta `const DATA_URL = 'productos.json';`

## Deploy en Vercel
1. Subir esta carpeta a un repositorio GitHub
2. Conectar el repo en vercel.com
3. Apuntar el dominio kualimuebles.com a Vercel
