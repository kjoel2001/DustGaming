<template>
  <div class="about-us">
    <h1 class="cart__title">Sobre nosotros</h1>
    <p>¡Bienvenido a nuestra tienda en línea de videojuegos y periféricos gaming! En {{ storeName }}, nos apasiona ofrecerte la mejor experiencia de juego y sumergirte en el emocionante mundo de los videojuegos.</p>
    
    <h1 class="cart__title">Nuestra misión</h1>
    <p>Nuestra misión es proporcionarte una amplia selección de videojuegos de calidad y periféricos gaming de última generación. Nos esforzamos por ser el destino número uno para todos los amantes de los videojuegos, brindando un catálogo diverso, atención al cliente excepcional y entregas rápidas y seguras.</p>
    
    <h1 class="cart__title">Nuestra selección de productos</h1>
    <p>En {{ storeName }}, ofrecemos una extensa gama de productos que incluyen videojuegos para todas las plataformas populares, como PlayStation, Xbox, Nintendo Switch y PC. También disponemos de una variedad de periféricos gaming de marcas reconocidas, como teclados, ratones, auriculares, controladores y mucho más.</p>
    
    <h1 class="cart__title">Nuestro compromiso con la satisfacción del cliente</h1>
    <p>En {{ storeName }}, tu satisfacción es nuestra máxima prioridad. Nos esforzamos por brindarte un servicio al cliente excepcional en cada paso del camino. Nuestro equipo dedicado está aquí para ayudarte con cualquier pregunta, consulta o problema que puedas tener. Valoramos tu confianza en nosotros y nos comprometemos a brindarte una experiencia de compra agradable y sin complicaciones.</p>
    
    <h1 class="cart__title">Envío rápido y seguros</h1>
    <p>Sabemos que deseas disfrutar de tus videojuegos lo antes posible, por eso nos esforzamos por realizar envíos rápidos y seguros. Trabajamos con socios logísticos confiables para garantizar que tus pedidos lleguen a tu puerta de manera rápida y segura.</p>
    
    <h1 class="cart__title">Únete a nuestra comunidad</h1>
    <p>En {{ storeName }}, no solo nos enfocamos en vender productos, sino también en construir una comunidad de amantes de los videojuegos. Síguenos en nuestras redes sociales y participa en nuestras actividades para estar al tanto de las últimas noticias, promociones especiales, eventos y reseñas de videojuegos.</p>
    
    <h1 class="cart__title">Contacto</h1>
    <p>Si tienes alguna pregunta, sugerencia o simplemente deseas obtener más información, no dudes en ponerte en contacto con nosotros. Puedes comunicarte con nuestro equipo de atención al cliente a través de nuestro formulario de contacto en línea, por correo electrónico o por teléfono. Estamos aquí para ayudarte en cualquier momento.</p>
    
    <p class="thanks">¡Gracias por visitar {{ storeName }}! Esperamos que disfrutes explorando nuestra amplia selección de videojuegos y periféricos gaming. ¡Diviértete y juega como nunca antes lo has hecho!</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      storeName: "Dust Gaming",
    };
  },
};
</script>

<style scoped>
.about-us {
  max-width: 800px;
  margin: 0 auto;
  padding: 20px;
  text-align: justify;
}

h1 {
  font-size: 32px;
  font-weight: bold;
  margin-bottom: 20px;
}

h2 {
  font-size: 24px;
  font-weight: bold;
  margin-top: 30px;
  margin-bottom: 15px;
}

p {
  font-size: 18px;
  line-height: 1.5;
  margin-bottom: 15px;
}

.thanks {
  font-size: 20px;
  font-style: italic;
  text-align: center;
  margin-top: 40px;
}
</style>
