# `04.1` Conditional Rendering

Hagamos nuestro componente `<Alert />` un poco más inteligente.

Cuando usas JSX tienes todas las funcionalidades de JavaScript disponibles: Variables, Bucles, Condicionales, etc.

Por ejemplo, el siguiente código renderiza una alerta roja o naranja dependiendo de la propiedad `color`.

```jsx
const colorClasses = {
    'red': 'alert-danger',
    'orange': 'alert-warning'
}

<div className={`alert ${colorClasses[props.color]}`} role="alert">
  This is a primary alert-check it out!
</div>
```

Estamos declarando una variable `colorClasses` que contendrá todos los class names que se le aplicarán en la alerta.

##  📝 Instrucciones:

1. Crea un componente `<Alert />` que renderice una [bootstrap alert](https://getbootstrap.com/docs/4.0/components/alerts/#examples). 

## 💡 Pista: 

El componente debe ser capaz de recibir las siguientes dos propiedades:

+ Text (string): El texto mostrado en la alerta.

+ Color (string): Rojo o naranja.

```jsx
{/* Para el color rojo */}
<div className="alert alert-danger" role="alert">
  This is a danger alert - check it out!
</div>

{/* Para el color amarillo */}
<div className="alert alert-warning" role="alert">
  This is a warning alert - check it out!
</div>
```
