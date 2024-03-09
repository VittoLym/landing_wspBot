<script setup>
import Bot from '/bot.svg'
</script>
<template>
  <section id="section">
    <div class="container-img">
      <img :src="Bot" alt="bot image">
    </div>
    <article>
      <p>En un mundo cada vez más conectado, la comunicación eficiente se ha vuelto esencial. Nuestro innovador bot de WhatsApp ofrece una solución única al transformar la experiencia de mensajería al permitir a los usuarios convertir fácilmente mensajes de voz en texto. Esta funcionalidad revolucionaria simplifica la interacción, permitiendo a los usuarios recibir y responder a mensajes de audio de manera rápida y eficiente.</p>
      <p>El bot de WhatsApp incorpora tecnología avanzada de procesamiento de lenguaje natural para ofrecer una transcripción precisa de los mensajes de voz recibidos. Al aprovechar algoritmos inteligentes, el bot identifica automáticamente la voz, convirtiéndola en un formato de texto comprensible. Esta característica no solo ahorra tiempo, sino que también mejora la accesibilidad al proporcionar una opción de lectura para aquellos con preferencias de comunicación específicas.</p>
    </article>
  </section>
</template>

<script lang="ts" setup>

</script>

<style scoped>
#section{
  height:85vh;
  width:100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-wrap: wrap;
}
#section .container-img{
  margin: 0 2rem;
  padding: 1rem;
  height: 60vh;
  background-color: var(--color-background-invertido);
  border-radius: 200%;
}
#section .container-img img{
  height: 50vh;
  width: 60vh;
  margin: 3vh 0;
}
article{
  width: 50%;
  height: max-content;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
article p{
  width: 80%;
  margin: .5rem 0;
  font-size: 1rem;
  color: var(--bg-t);
}
</style>