<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(icono="far fa-question-circle" titulo="Actividad didáctica")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5

    #Actividad                
      <Actividad :cuestionario="cuestionario"/>

</template>

<script>
import Actividad from 'ecored-pkg-fliz/plugin/components/actividad/Actividad.vue'
export default {
  name: 'ActividadDidactica',
  components: {
    Actividad,
  },
  data: () => ({
    cuestionario: {
      tema:
        'Evaluación de conocimientos sobre la formulación de proyectos agropecuarios mediante la metodología de marco lógico.',
      titulo: 'Cuestionario',
      introduccion:
        '<b>Objetivo:</b> evaluar la capacidad del aprendiz para reconocer y aplicar los elementos técnicos y metodológicos del enfoque de marco lógico en la formulación de proyectos agropecuarios, considerando el análisis de problemáticas, la planificación de alternativas de solución y la estructuración de proyectos orientados al desarrollo rural.',
      barajarPreguntas: true,
      titulo_aprobado: '¡BUEN TRABAJO!',
      titulo_reprobado: 'VUELVA A INTENTARLO',
      preguntas: [
        {
          id: 1,
          texto:
            '¿Cuál es el propósito principal de la metodología de marco lógico?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Elaborar únicamente presupuestos de proyectos.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Gestionar proyectos mediante un análisis estructurado de problemas y soluciones.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Realizar estudios financieros exclusivamente.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Determinar costos de producción agrícola.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los conceptos relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
        },
        {
          id: 2,
          texto:
            'El enfoque de marco lógico se caracteriza por ser una metodología:',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Empírica y no estructurada.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Exclusivamente financiera.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Sistémica, participativa y organizada.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Basada únicamente en información secundaria.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los conceptos relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
        },
        {
          id: 3,
          texto:
            '¿Cuál de las siguientes fases hace parte de la metodología de marco lógico?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Comercialización.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Ejecución financiera.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Identificación del problema.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Auditoría contable.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los conceptos relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
        },
        {
          id: 4,
          texto:
            'El análisis del contexto en torno a la problemática de la ruralidad permite:',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Determinar únicamente los costos del proyecto.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Comprender las condiciones sociales, económicas y ambientales del territorio.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Elaborar los contratos del proyecto.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Definir exclusivamente los indicadores financieros.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los conceptos relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
        },
        {
          id: 5,
          texto: 'La información secundaria corresponde a:',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Datos obtenidos mediante encuestas y entrevistas realizadas por el proyecto.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Información recolectada directamente en campo.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Información proveniente de documentos, estudios e investigaciones previas.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Opiniones informales de los productores.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los conceptos relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
        },
        {
          id: 6,
          texto: 'El análisis de actores involucrados tiene como finalidad:',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Determinar el presupuesto total del proyecto.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Calcular la rentabilidad del proyecto.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Elaborar los cronogramas de obra.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Identificar intereses, influencia y participación de los diferentes actores.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los conceptos relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
        },
        {
          id: 7,
          texto: 'El diagnóstico de la situación problémica busca:',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Identificar y comprender las causas y efectos de una problemática.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Elaborar únicamente el presupuesto del proyecto.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Contratar personal especializado.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Realizar auditorías financieras.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los conceptos relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
        },
        {
          id: 8,
          texto:
            '¿Cuál de las siguientes herramientas facilita la identificación de problemas a partir de información primaria?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Balance general.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Estado de resultados.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Inventario de maquinaria.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Encuestas y entrevistas.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los conceptos relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
        },
        {
          id: 9,
          texto: 'La matriz de Vester se utiliza para:',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Establecer indicadores financieros.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Priorizar problemas según sus relaciones de influencia y dependencia.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Elaborar presupuestos de inversión.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Diseñar estrategias de comercialización.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los conceptos relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
        },
        {
          id: 10,
          texto:
            'En la matriz de Vester, un problema altamente influyente sobre otros se considera:',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Pasivo.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Independiente.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Crítico o activo.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Secundario.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los conceptos relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
        },
        {
          id: 11,
          texto: 'El árbol de problemas permite representar:',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'La estructura organizacional de una empresa.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Los recursos financieros disponibles.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Las relaciones causa-efecto de una situación problemática.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Los costos operativos del proyecto.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los conceptos relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
        },
        {
          id: 12,
          texto: 'En el árbol de problemas, las raíces representan:',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Los objetivos del proyecto.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Las actividades del proyecto.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Las causas del problema central.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Los indicadores de gestión.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los conceptos relacionados con la agroecología y la evaluación ambiental de los sistemas agrícolas.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con la agroecología y la evaluación ambiental de los sistemas agrícolas.',
        },
        {
          id: 13,
          texto: 'El árbol de objetivos se construye a partir de:',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'La eliminación de actividades.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'La transformación de problemas en situaciones positivas deseadas.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Los estados financieros.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'El análisis de mercado.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los conceptos relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
        },
        {
          id: 14,
          texto: 'El análisis de alternativas permite:',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Escoger la mejor opción para solucionar la problemática identificada.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Determinar únicamente los costos del proyecto.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Elaborar informes financieros.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Realizar actividades de control interno.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los conceptos relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
        },
        {
          id: 15,
          texto: 'La matriz de marco lógico es una herramienta que:',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Organiza objetivos, indicadores, medios de verificación y supuestos.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Calcula exclusivamente costos de producción.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Determina el número de trabajadores requeridos.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Define los precios de venta.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los conceptos relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
        },
        {
          id: 16,
          texto: 'Los indicadores en la matriz de marco lógico sirven para:',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Medir el avance y cumplimiento de los objetivos.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Calcular únicamente impuestos.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Elaborar contratos laborales.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Determinar la ubicación del proyecto.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los conceptos relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
        },
        {
          id: 17,
          texto: 'Los medios de verificación corresponden a:',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Las actividades operativas del proyecto.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Las fuentes donde se obtiene la información para comprobar los indicadores.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Los recursos financieros disponibles.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Las estrategias de comercialización.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los conceptos relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
        },
        {
          id: 18,
          texto: 'En el marco lógico, los supuestos son:',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Recursos económicos asignados al proyecto.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Actividades programadas en el cronograma.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Condiciones externas necesarias para el logro de los objetivos.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Indicadores de rentabilidad.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los conceptos relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
        },
        {
          id: 19,
          texto: 'El análisis de riesgos permite:',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Identificar situaciones que pueden afectar el logro de los objetivos del proyecto.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Incrementar automáticamente el presupuesto.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Determinar el precio de los productos agropecuarios.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Elaborar únicamente informes administrativos.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los conceptos relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
        },
        {
          id: 20,
          texto:
            'El plan operativo y el presupuesto general del proyecto permiten:',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Organizar actividades, recursos, tiempos y costos requeridos para la ejecución.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Definir únicamente las fuentes de financiación.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Establecer exclusivamente indicadores de gestión.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Realizar auditorías externas.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los conceptos relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
        },
      ],
      mensaje_final_aprobado:
        'Ha superado la actividad y demuestra sólidos conocimientos sobre la formulación de proyectos agropecuarios bajo el enfoque metodológico de marco lógico.',
      mensaje_final_reprobado:
        'No ha superado la actividad. Le recomendamos volver a revisar el componente formativo e intentar nuevamente la actividad didáctica.',
    },
  }),
}
</script>

<style lang="sass"></style>
