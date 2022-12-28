# Next JS 13 

## Novedades

 En la carpeta `app` , puedes crear todas las carpetas que quieras. Antes, si creabas una carpeta, se convertia automáticamente en una ruta. Ahora, si creas una carpeta pero no creas un `page.tsx`, no sera una ruta.

**Todo lo que este dentro de la carpeta `app`, se ejecuta por defecto en el servidor**

Si lo que quieres es que algo se ejecute en el cliente, poner `'use client'` al principio del archivo. Lo lógico sería que intentes que el componente que se ejecute en el servidor, sea lo más pequeño posible. Ej: Solo el componente del boton de like.


## Importante

Si vas a usar esta versión (13) y vas a necesitar usar la api, tu directorio del proyecto debe tener tanto `app` como `pages/api`. Al menos esto es actualmente (28/12/22)

## Fetching

Estático:

```javascript
const fetchPosts = async () => {
	return fetch('http://jsonplaceholder.typicode.com/posts')                                        
	then(res => res.json())     
}
```

ServerSide:

```javascript
const fetchPosts = async () => {
	return fetch('http://jsonplaceholder.typicode.com/posts', { cache: 'no-store'})                                        
	then(res => res.json())     
}
```

Incremental Static Regeneration (Regenera la página cada minuto o los segundos que pongas):

```javascript
const fetchPosts = async () => {
	return fetch('http://jsonplaceholder.typicode.com/posts', { next: { revalidate: 60 } })                                        
	then(res => res.json())     
}
```