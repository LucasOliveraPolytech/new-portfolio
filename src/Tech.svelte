<script>
  import Works from './components/Works.svelte'

  const features = [
    {
      title: "Lenguaje Natural",
      description: "<p></p>",
      outLink: "https://catalyticsound.com/quarterly/8/index.html",
      media: "images/cq-8.png",
    },
    {
      title: "Control de proceso",
      description: "<p></p>",
      outLink: "https://catalyticsound.com/quarterly/9/index.html",
      media: "images/cq-9.png"
    },
    {
      title: "Sugerencias Arquitectónicas",
      description: "<p> </p>",
      media: "images/catalyticsoundstream.png"
    },
    {
      title: "Simulación",
      description: "<p>Dentro de AgileTalk es posible recrear el flujo de eventos luego de haberse dado dentro del ambiente.</p>",
      media: "images/catalyticsoundstream.png"
    },
    {
      title: "Guía del Proceso",
      description: "<p>Como herramienta didáctica, AgileTalk permite entrenar a alguien en un nuevo proceso de desarrollo guiándolo a traves de las distintas ceremonias y artefactos.</p>",
      media: "images/catalyticsoundstream.png"
    },
    {
      title: "Personalizable",
      description: "<p>Aún en desarrollo. Manteniendo un monitoreo de las distintas acciones de un Team Memver a lo largo de un proyecto sería posible inferir en su personalidad y por ende personalizar sus respuestas y acciones en base a la misma cuando esté desconectado</p><p>Aún en desarrollo. Manteniendo un monitoreo de las distintas acciones de un Team Memver a lo largo de un proyecto sería posible inferir en su personalidad y por ende personalizar sus respuestas y acciones en base a la misma cuando esté desconectado</p><p>Aún en desarrollo. Manteniendo un monitoreo de las distintas acciones de un Team Memver a lo largo de un proyecto sería posible inferir en su personalidad y por ende personalizar sus respuestas y acciones en base a la misma cuando esté desconectado</p>",
      media: "images/catalyticsoundstream.png"
    },
  ]

  let uid = 1
  
  features.forEach((feat) => {
    feat.uid = uid++
  })
</script>

<Works works={features} />
