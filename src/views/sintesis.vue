<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(icono="fas fa-sitemap" titulo="Síntesis")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    p.mb-4 El componente formativo Formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico aborda la metodología que facilita la formulación, planificación, ejecución, seguimiento y evaluación de proyectos mediante un proceso lógico y sistemático. Su principal herramienta es la Matriz de Marco Lógico (MML), la cual organiza los objetivos, resultados, actividades, indicadores, medios de verificación y supuestos para orientar la gestión y la toma de decisiones.

  

    .bloque-texto-g.bloque-texto-g--inverso.bg-color-99.p-3.p-sm-4.p-md-5.mb-5
      .bloque-texto-g__img(
        :style="{'background-image': `url(${require('@/assets/curso/img1.png')})`}"
      )
      .bloque-texto-g__texto.p-4
        p.mb-0 La construcción de la MML comprende dos etapas. La etapa de análisis incluye el estudio del contexto, el análisis de actores, problemas y objetivos, utilizando herramientas como la matriz de Vester, el Diagnóstico Rural Participativo (DRP) y el mapa de involucrados, con el fin de identificar necesidades y formular soluciones pertinentes y sostenibles. Por su parte, la etapa de planificación contempla el análisis de alternativas, la elaboración de la matriz, la definición de indicadores y medios de verificación, así como el análisis de riesgos y supuestos, garantizando una adecuada organización, seguimiento y evaluación del proyecto para el logro de los resultados esperados.


    .row.justify-content-center
      .col-lg-10.mb-5
        figure
          img(src="@/assets/curso/temas/sintesis.svg", alt="Se detalla aspectos importantes de la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico, generalidades del enfoque de marco lógico, etapa de análisis, etapa de planificación.")
      .col-auto
        a.anexo.mb-5(:href="obtenerLink('/downloads/Sintesis.pdf')" target="_blank")
          .anexo__icono
            img(src="@/assets/template/icono-pdf.svg")
          .anexo__texto
            p Anexo. Síntesis

</template>

<script>
export default {
  name: 'Sintesis',
  data: () => ({
    // variables de vue
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>
